---
title: "Estructura Datos. Conceptos"
date: 2022-02-23
draft: false
description: "La estructura de datos es el elemento fundamental de la ciencia de computación, son un medio para manejar grandes cantidades de datos de manera eficiente."
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/datos.svg']
blog_list_image: images/datos.svg
author: Saúl Zalimben
slug: estructura-datos-conceptos
idiom: Español
---

Si acabas de encontrar esta publicación, antes de continuar te recomiendo que le des un vistazo a [Introducción a Estructuras de Datos](blog/spanish/posts/intro-estructura-datos) el cual brinda una introducción a los conceptos preliminares para comprender las Estructuras de Datos.

---

Una Estructura de Dato es una colección de datos que pueden ser caracterizados por su
organización y las operaciones que se definen en ella, es la implementación de un TDA en
algún lenguaje de programación, es decir, la representación de algún tipo de dato y de sus
operaciones asociadas.

![Estructura de Datos](images/datos.svg)

### Simples y Compuestos
Se dice que son tipos simples o primitivos cuando se definen sobre sí mismos, es decir,
no están compuestos de otras estructuras de datos, *e.g.* números enteros, reales y carácter
(char). Mientras que aquellas estructuras que se definen en función a otros se denominan
compuestos o agregados, es decir, están construidos basados en tipos de datos primitivos,
*e.g*. el tipo cadena (string) basado en caracteres.

![Datos Simples y Compuestos](images/simplesycompuestos.JPG)

>
> Cada lenguaje de programación dispone de su propio conjunto de tipos primitivos y compuestos
>

### Estáticos y Dinámicos
Las estructuras de datos estáticas son aquellas en las que el tamaño ocupado en memoria es fijo, este se define antes de que el programa se ejecute y el tamaño reservado de memoria no puede ser modificado durante la ejecución del programa.

Mientras que las estructuras de datos dinámicas se pueden ampliar y comprimir a medida
que se requieran durante la ejecución del programa, es decir, pueden reservar y liberar
espacios de memoria de forma dinámica.

En la siguiente figura se observa que la estructura *Vector*, tiene un tamaño igual a la cantidad de letras del abecedario, por lo tanto ya no se pueden agregar más elementos, esta estructura es estática. Por otro lado, la estructura *Grafo* está compuesta por otras estructuras de datos dinámicas denominadas *Nodos*, que pueden ser instanciadas en cualquier momento, es decir, se pueden agregar más elementos en tiempo de ejecución del programa, esta estructura es dinámica.

![Estáticos y Dinámicos](images/estatica-dinamica.png)

### Lineales y No lineales
Las estructuras de datos lineales son aquellas donde los elementos ocupan lugares
sucesivos en la estructura y cada uno de ellos tiene un único sucesor y un único predecesor, e.g. un vector. Sin embargo las estructuras de datos no lineales no cumplen con esta restricción, e.g. los grafos.

![Lineales y No Lineales](images/lineales-no-lineales.png)

---
¡Gracias por leer! 

Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido, puedes *[invitarme un café](https://www.buymeacoffee.com/szalimben)*.