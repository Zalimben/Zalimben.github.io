---
title: "Vectores (Array o Arreglos)"
date: 2022-03-04
draft: false
description: "Estructuras estáticas lineales finitas ordenadas secuencialmente, y de datos homogéneos."
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/array/vector-simple.svg']
transform: 50%
blog_list_image: images/array/vector-simple.svg
author: Saúl Zalimben
slug: array
idiom: Español
---

Si acabas de encontrar esta publicación, antes de continuar te recomiendo que le des un vistazo a [Estructuras de Datos. Conceptos](blog/spanish/posts/estructura-datos-conceptos) el cual brinda conceptos claves para comprender las Estructuras de Datos.

---

Los **Vectores (Arrays o Arreglos)** son estructuras estáticas lineales finitas ordenadas secuencialmente, y de datos homogéneos, es decir, del mismo tipo de dato y se puede acceder directamente a cada elemento del mismo mediante el uso de índices, donde el índice de un elemento (1, 2, ..., n) designa su posición dentro del vector. Es una secuencia de posiciones de la memoria a las que se puede acceder directamente.

![Vector](images/array/vectores.svg)

>
> En general, los índices de un vector comienzan en 0, pero este puede diferir
> acorde al lenguaje de programación utilizado.
>

## Operaciones elementales sobre Vectores
- Asignar
- Leer
- Recorrer (Acceso secuencial)
- Insertar
- Eliminar
- Ordenar
- Buscar

Cabe resaltar que otras operaciones pueden ser definidas sobre esta estructura como mezclar, filtrar, copiar, etc., acorde a las necesidades del problema por resolver.


## Vector Multidimensional
Un vector multidimensional puede tener *n* cantidad de dimensiones, en consecuencia se dice que es *n*-dimensional. También se lo puede ver como un vector de vectores de vectores, cuyos elementos pueden ser referenciados por dos o más índices.

### Vector Bidimensional
Un vector multidimensional de 2 dimensiones, es decir, un vector bidimensional recibe el nombre de matriz o tabla, es un caso especial del vector multidimensional,

El mismo puede ser considerado como un vector de vectores. Por consiguiente, es un conjunto de elementos homogéneos, en el cual existe un orden y en el que se necesita especificar dos índices para poder identificar cada elemento, es decir, es necesario definir la fila y la columna en la matriz para poder acceder a cada elemento, **Matriz[fila][columna]**.

![Matriz](images/array/matriz.svg)

### Vector *n*-dimensional
Los conceptos de rango de índices y número de elementos se pueden ampliar directamente desde vectores de una y dos dimensiones a vectores de orden más alto. Un vector puede ser definido de tres, cuatro hasta de *n*-dimensiones. 
En general, un vector *n*-dimensional requiere que los valores de los *n* índices sean especificados a fin de identificar unívocamente un elemento. Si cada componente tiene *n* índices, se dice que el vector es de *n* dimensiones. En la figura se observa un vector de 3 dimensiones, un Cubo. 

**Cubo[0][0][0]** representa el elemento del cubo resaltado en azul; mientras que el elemento **Cubo[2][2][0]** esta resaltado en verde.

![Cubo](images/array/cubo.svg)


---

¡Gracias por leer! 

Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido puedes realizar una donación *[invitándome un café](https://www.buymeacoffee.com/szalimben)*.