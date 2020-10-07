---
title: "Geo-Economic Clustering"
date: 2020-10-07
tages: [clustering, data science]
excerpt: "Classification of countries based on their GDP per capita and 
the distance among them."
---

In this project we classify all the countries in the world in 10 different groups by means of their GDP per capita and the distance among them.
The process of data gathering, the mathematical formulation and the results can be found in this file available from [Github](https://github.com/sesiga/geo_economic_clustering/blob/main/task.pdf). The code is written in Python and it is also available from [Github](https://github.com/sesiga/geo_economic_clustering/blob/main/task.py). A custom model of *clustering* has been developed, in order to compute the distance among countries given that they lie 
on the surface of a sphere. Click [here](https://github.com/sesiga/geo_economic_clustering) and check out the repository. The file
**geo_economic_clustering.csv** contains the results and it has 6 columns:

* **country**: the name of the country.
* **cluster**: the group it belongs to.
* **av_gdp**: the average GDP per capita of the cluster.
* **gdp**: the GDP per capita of the country.
* **gdpt**: the total GDP of the cluster. It is the sum of all the GDPs.
* **cum_gdp**: the fraction of the total GDP that the country has on the group.

## Results
Below we present a table containing the clusters and their countries and one plot with the average GDP of each cluster. 

From a geo-economic point of view, we can see that the algorithm has found a good
solution. In general, countries that are relatively close in physical distance and in GDP
per capita belong to the same cluster. For example, Cluster 7 has the highest average
GDP per capita and we can find countries that are not very far away. Although USA is a
bit far in physical distance from the rest of the countries, it is quite similar in terms of
GDP per capita. Cluster 2 has the lowest average GDP per capita and we can find
countries that are extremely poor in terms of economics and that are quite close in
terms of physical distance, since all of them are located in the south of Africa. Cluster 5
also has a low GDP per capita but it is located at the north part of Africa. Another
example is Cluster 8, that contains many of the healthiest countries in Europe. Poorer
countries in Europe are found in Cluster 6 together with some middle east countries.
Cluster 1 contains the countries of South America, whose GDPs per capita are not quite
different. Perhaps, the biggest differences can be found in Cluster 0 which contains
countries located around the west Pacific. However, some of them are a bit far from
each other and there are important differences in terms of GDP per capita for some of
them. For instance, the GDP per capita of Australia is 54907 US$ meanwhile the GDP per
capita of Tuvalu is just 4049 US$. However, we have to keep in mind that there are many
solutions, and this is just the one that we have obtained after randomly initializing the
center of the clusters. Thus, we will always have some discrepancies with the results.

<figure>
  <img src="/images/GeoEconomicClustering1.png" alt="This is a placeholder image">
  <figcaption>Classification of the countries in clusters.</figcaption>
</figure>

<figure>
  <img src="/images/GeoEconomicClustering2.png" alt="This is a placeholder image">
  <figcaption>Cluster's average GDP per capita.</figcaption>
</figure>