---
title: Recursividad
date: 2020-05-03
draft: false
description: Herramienta para solucionar problemas que se encuentran definidos en términos iterativos.
tags: #spanish #español #principiante #fundamentos
images: ['https://dev-to-uploads.s3.amazonaws.com/i/gtii7l9u8jy8m5qtolrh.jpg']
blog_list_image: https://dev-to-uploads.s3.amazonaws.com/i/gtii7l9u8jy8m5qtolrh.jpg
author: Saúl Zalimben
slug: recursividad
idiom: Español
---

>
> Iterar es humano, recursivar es divino
>

**Recurrencia**, **recursión** o **recursividad** es la forma en la cual se especifica un proceso basado en su propia definición, por ejemplo las muñecas rusas, si las vemos como procesos podemos observar que cada una contiene una instancia más pequeña de sí misma.
En ciencias de la computación, se la utiliza como herramienta para solucionar dichos problemas, que se encuentran definidos en términos iterativos.

### Algoritmos iterativos

Recordando que un algoritmo es la secuencia de instrucciones que realizadas en orden conducen a obtener la solución de un problema, cuando existen problemas que se encuentran definidos en torno a sí mismos, se utilizan ciclos iterativos que consiste en repetir una instrucción muchas veces sin escribir código una y otra vez.

![Iteración](https://dev-to-uploads.s3.amazonaws.com/i/rkqm6zouu47fv8tgogx8.png)

Donde cada iteración resuelve una instancia más pequeña del problema hasta el punto que el problema ya no pueda dividirse.

### Algoritmos recursivos
Para resolver estos problemas, también se puede optar por utilizar algoritmos recursivos, realizando llamadas iterativas a la misma función.

 ![Recursividad](https://dev-to-uploads.s3.amazonaws.com/i/68ihr48kcb6qhyvc5w6e.png)

La definición de recursividad debe incluir un conjunto de condiciones para que la recursión sea exitosa:
- Un **componente base** o **caso base**, es decir, una condición de salida de la iteración, una instancia del problema que pueda ser resuelta sin recursión.

![Componente Base](https://dev-to-uploads.s3.amazonaws.com/i/8rxi0dtalsm8dx0jwfkp.png)

- Toda llamada recursiva debe realizar algún progreso hacia el caso base.

![Camino al caso base](https://dev-to-uploads.s3.amazonaws.com/i/dplzexzpbavbvgasre86.png)

- "Siempre debemos asumir que la recursión funciona"
- Nunca duplicar la tarea resolviendo la misma instancia del problema de forma recursiva.

Si bien los dos primeros puntos son suficientes, el tercer punto cobra sentido cuando se trata con problemas grandes, compuestos de muchas instancias y que hace casi imposible de seguir el rastro. 
Mientras que el último punto, está ligado a la optimización de la recursión, con el fin de evitar resolver la misma instancia del problema gastanto recursos de forma innecesaria. 

Un ejemplo clásico para entender la recursión es calcular el factorial de un número *n*. 

#### Ejemplo: Factorial

> El factorial es el producto de todos los números enteros positivos desde 1 hasta n, y se define como *factorial(n) = n!*. 

> Entonces, factorial(5) = 5! = 5 * 4 * 3 * 2 * 1 = 120

Se observa que existe un ciclo iterativo constante, donde cada llamada resuelve una instancia más pequeña del problema.

> factorial(n) = n * factorial(n - 1)

![Factorial](https://dev-to-uploads.s3.amazonaws.com/i/k4ofjzxixq6gut765evq.png)

En la imagen se observa como se realizan las llamadas recursivas, resolviendo instancias más pequeñas del problema en cada paso hasta llegar al caso base de factorial, *factorial(1) = 1! = 1*.

#### Ventaja & Desventaja
Una importante ventaja es que el código luce más prolijo y elegante, al mismo tiempo que se escribe menos para resolver el mismo problema.
Pero como principal desventaja se encuentra el tiempo de llamada a la función, puesto que se consume tiempo de procesamiento y en simultáneo espacio de almacenamiento extra por cada llamada, ya que se necesita guardar el resultado de cada recursión junto con los parámetros que son enviados en cada instancia del problema.

### Reflexiones finales
Si bien la recursión ayuda a resolver problemas de forma elegante y prolija, es importante mencionar que cualquier problema que se pueda resolver de forma recursiva, también se puede resolver de forma iterativa, esto significa que no se debe utilizar recursión para sustituir iteraciones simples. 

No se debe pensar que la recursión es la mejor herramienta para resolver todos los problemas iterativos, ya que existen problemas que no pueden resolverse de forma recursiva, pero si iterativa o que la complejidad es menor de forma iterativa que recursiva, es por ello que siempre se debe analizar el problema en cuestión con el fin de entender su naturaleza y seleccionar la mejor herramienta para resolverlo. 

### Referencias
- Weiss, Mark Allen (2010). Recursion. Data structures & problem solving using Java (pp. 293 - 351). Fourth edition. Addison-Wesley
- Aguilar Joyanes, Luis (2008). Recursividad. Fundamentos De Programación. Algoritmos, estructura de datos y objetos (pp. 519 - 550). Cuarta edición. McGraw-Hill.
- Shaffer, Clifford A. (2010). Mathematical Preliminaries. A Practical Introduction to Data Structures and Algorithm Analysis. (Java Version) (pp. 36 – 46). Third Edition.

