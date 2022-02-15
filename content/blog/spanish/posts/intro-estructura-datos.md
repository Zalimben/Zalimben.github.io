---
title: "Introducción a Estructuras de Datos"
date: 2022-02-16
draft: false
description: "Las estructuras de datos son el elemento fundamental de la computación, son construcciones utilizadas para almacenar colecciones de datos y manipularlos"
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/datos.svg']
blog_list_image: images/datos.svg
author: Saúl Zalimben
transform: -15%
slug: intro-estructura-datos
idiom: Español 
---

Uno de los aspectos más importantes de la ciencia de la computación es la creación de nuevos tipos de datos que sean apropiados para resolver problemas específicos del mundo real.

Las estructuras de datos son el elemento fundamental de la computación, son construcciones utilizadas para almacenar colecciones de datos y manipularlos. Todos los algoritmos manipulan datos, y éstos deben estar diseñados y estructurados adecuadamente para que puedan conectarse entre ellos.

---

## Preliminares
### Tipo
Un tipo es un conjunto de valores que puede poseer una variable, por ejemplo una variable del tipo booleano puede contener dos posibles valores, falso o verdadero, o bien una variable del tipo entero, como lo define su nombre son todos los números enteros _P(Z)_.

### Tipo de Dato
Un Tipo de Dato es un tipo junto a todas las operaciones elementales que manipulan dicho tipo, un conjunto de funciones básicas que uno puede aplicar a estos valores, _e.g._ para los números enteros se pueden aplicar las operaciones básicas de la aritmética (suma, resta, multiplicación y división).

> 
> #### Abstracción 
> Es el conocimiento que se tiene de una cosa prescindiendo de los detalles que están ligados a ella. Conocemos un objeto viéndolo, sabemos qué es sin necesidad de ver su interior, su implementación o la forma de construcción.
> La abstracción de datos consiste en ocultar las características de un objeto, de manera a que solamente utilizamos el nombre del objeto para hacer referencia a él. Es la capacidad para encapsular y aislar la información del diseño y ejecución.
> 
> #### Encapsulación
> Proceso de almacenar en un mismo compartimento los elementos de una abstracción, que constituyen su estructura y comportamiento.
> 

### Tipo de Dato Abstracto (TDA)
Un TDA es la definición de un tipo de dato como un componente que está definido en términos de su tipo y el conjunto de operaciones sobre ese tipo, en donde las operaciones no se encuentran implementadas, solo su comportamiento, es decir, se define qué debe hacer y no el cómo. Los detalles de implementación están ocultos y encapsulados para el usuario del TDA.

Generalmente, los TDA son conceptos matemáticos o lógicos que pueden ser implementados en diferentes máquinas usando diferentes lenguajes. Son muy flexibles y no dependen de ningún lenguaje ni máquina.

![TDA](https://dev-to-uploads.s3.amazonaws.com/i/4c02moocan9xt9tk0zei.png)

En cada lenguaje de programación, se implementan los TDA utilizando diferentes métodos y lógicas, es posible realizar todas las operaciones asociadas que están definidas para un TDA independientemente del lenguaje utilizado. Por ejemplo, en el Lenguaje C, los TDA se implementan principalmente con estructuras *(structure)*. Mientras que en los Lenguajes C++ o Java, se implementan mediante clases *(class)*. Sin embargo, **las operaciones son comunes en todos los lenguajes de programación**.


![Estructura de Datos](images/datos.svg)

---
¡Gracias por leer! 

Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido, puedes *[comprarme un café](https://www.buymeacoffee.com/szalimben)*.