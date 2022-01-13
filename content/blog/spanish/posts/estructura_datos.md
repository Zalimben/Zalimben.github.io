---
title: "Estructura Datos"
date: 2020-03-27
draft: false
author: Saúl Zalimben
description: La estructura de datos es el elemento fundamental de la ciencia de computación, son un medio para manejar grandes cantidades de datos de manera eficiente.
tags: #spanish #español #principiante #fundamentos
blog_list_image: https://dev-to-uploads.s3.amazonaws.com/i/4c02moocan9xt9tk0zei.png
author: Saúl Zalimben
slug: estructura-datos
idiom: Español
---

>
> _“El estudio de estructura de datos y algoritmos que los manipulan es el corazón de la ciencia de la computación”_ 
>
> -- Clifford A. Shaffer
> 

Siguiendo la reflexión de Shaffer, la estructura de datos es el elemento fundamental de la ciencia de computación, pero qué realmente es una estructura de dato, para definirlo tenemos que descomponerlo aún más, partiendo desde su componente más básico, un tipo.


Un **tipo** es un conjunto de valores que puede poseer una variable, por ejemplo el tipo booleano con dos posibles valores, de falso o verdadero o bien los números enteros. 


Se dice que son **tipos simples o primitivos** cuando se definen sobre sí mismos, mientras que aquellos datos que se definen en función a otros se denominan **compuestos o agregados**, por ejemplo si deseamos definir el tipo *Persona*, este tipo podría estar formado por tipos primitivos para representar cada una de sus característica; su nombre, su apellido, edad y así sucesivamente.


Cada lenguaje de programación dispone de su propio conjunto de tipos primitivos, a continuación los tipos primitivos presentes en el lenguaje programación Python y Java.

| Tipos primitivos  | Despliega                                 | Ejemplos/Rango  |
| -----------------:|------------------------------------------:|----------:|
| int               | números enteros                           | 42        |
| float             | números de punto flotante                 | 1.0       |
| complejos         | números complejos                         | 2 + 3j    |
| boolean           | valores lógicos                           | TRUE o FALSE|
| cadenas           | texto                                     | 'Bienvenido a Python'|
| lista             | colección de objetos                      | [1, 2, 3, 4]     |
| tupla             | colección de objetos de distinto tipo     | ("A", 1.2, 0, -2)|
| diccionario       | colección de objetos del tipo clave-valor | \{"mantisa":5.81, "exponente":1.4\}|
>Tipos de datos primitivos en Python

| Tipos primitivos  | Despliega                                 | Ejemplos/Rango  |
| -----------------:|------------------------------------------:|----------:|
| byte              | números enteros de 8-bit                  | –128 a 127 |
| short             | números enteros de 16-bit                 | –32,768 a 32,767       |
| int               | números enteros de 32-bit                 | –2,147,483,648 a 2,147,483,647    |
| long              | números enteros de 64 bit                 | –2 <sup> 63</sup> a 2<sup>63</sup> – 1|
| float             | números de punto flotante                 | 10<sup> -46</sup> a 10<sup>38</sup>|
| double            | colección de objetos                      | 10<sup> -324</sup> a 10<sup>308</sup>|
| char              | caracteres Unicode                        | "A", "c", "P"|
| boolean           | valores lógicos                           | TRUE o FALSE|
>Tipos de datos primitivos en JAVA

Si bien existen tipos compartidos por varios lenguajes de programación estos pueden variar acorde la orientación y el propósito del lenguaje, como es el caso de Python y Java.

Un **tipo de dato** es un tipo junto a todas las operaciones elementales que manipulan dicho tipo, un conjunto de funciones básicas que uno puede aplicar a estos valores, por ejemplo para los números enteros se pueden aplicar las operaciones básicas de la aritmética (suma, resta, multiplicación y división).

Mientras que un **tipo de dato abstracto (TDA)** es la definición de un tipo de dato como un componente que está definido en términos de su tipo y el conjunto de operaciones sobre ese tipo, en donde las operaciones no se encuentran implementadas, solo su comportamiento, es decir, se define **qué debe hacer y no el cómo hacer**.

Y finalmente la **estructura de dato** es la implementación de un TDA en algún lenguaje de programación, es decir, la representación de algún tipo de dato y de sus operaciones asociadas.

Un TDA define la forma lógica de un tipo de dato, mientras que una estructura de dato implementa la forma física del tipo de dato.

![TDA](https://dev-to-uploads.s3.amazonaws.com/i/4c02moocan9xt9tk0zei.png)

Cuando se desea resolver un problema es importante seleccionar una estructura de datos adecuada, para dicho efecto se debe analizar los recursos disponibles y utilizar la que mejor se adecua a las necesidades del problema.


### Referencias:
- Shaffer, Clifford A. (2010). *A Practical Introduction to Data Structures and Algorithm.  (3rd ed. Java Version).*
-  Cormen, Thomas H.; Leiserson, Charles E.; Rivest, Ronald L.; Stein, Clifford (2009). *Introduction to Algorithms, Third Edition (3rd ed.)*. The MIT Press

