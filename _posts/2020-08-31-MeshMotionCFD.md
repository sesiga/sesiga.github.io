---
title: "Desarrollo de una Estrategia de Selección de Aglomerados para la Transferencia de Deformaciones entre mallas CFD"
date: 2020-08-31
tages: [mesh motion, CFD, computation fluid dynamics]
excerpt: "Bachelor's final degree project. Bachelors Degree in Aerospace Engineering."
---



This post contains the bachelor's end of degree project I worked on to finish the Bachelor's Degree in Aerospace Engineering at the Technical University of Madrid. The summary
of the paper is presented below, and the full paper is available from [Github](https://github.com/sesiga/sesiga.github.io/raw/master/papers/TransferenciaDeformacionesMallasCFD.pdf). 
This project has been developed in Spanish.

La transferencia de deformaciones entre mallas CFD es un problema que aparece cuando
se modifica la geometría del objeto estudiado. Para un objeto dado, se utilizan códigos de
generación de mallas para crear una malla optimizada en función de la geometría. Cuando
se produce una modificación en la geometría original, lo ideal sería generar otra malla a partir
de la nueva geometría para así poder mantener una buena calidad en la malla. Sin embargo, la generación de mallas conlleva un elevado coste computacional por lo que es necesario pensar
en otras alternativas con las que se consigan resultados similares, en un tiempo aceptable y
manteniendo una buena calidad de la malla.
Una de las opciones (y la que se va a desarrollar en este trabajo) consiste de modificar la
malla original. Para ello se utiliza la deformación conocida de varios nodos y posteriormente
se deforma el resto de la malla utilizando métodos de interpolación.