---
title: "Listas"
date: 2022-03-09
draft: false
description: "Son estructuras de datos lineales ordenadas secuenciales de 0 o más elementos homogéneos almacenados en memoria."
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/list/lista-simple.svg']
blog_list_image: images/list/lista-simple.svg
transform: 50%
author: Saúl Zalimben
slug: list
idiom: Español
---

Si acabas de encontrar esta publicación, antes de continuar te recomiendo que le des un vistazo a [Estructuras de Datos. Conceptos](blog/spanish/posts/estructura-datos-conceptos) el cual brinda conceptos claves para comprender las Estructuras de Datos.

---

Las listas son estructuras de datos lineales ordenadas secuenciales de 0 o más elementos homogéneos almacenados en memoria. Donde cada elemento de la lista, excepto el primero, tiene un único predecesor y cada elemento de la lista, excepto el último, tiene un único sucesor.

Se denomina **lista vacía** a una lista con 0 elementos, mientras que la cantidad de elementos que posee la lista, es el **tamaño** de ella. El inicio de la lista se denomina **cabecera**, mientras que el final de la misma es el **fin**.

Existen dos enfoques para implementar las listas, la primera basada en vectores y la segunda basada en listas enlazadas.

## Listas: Estáticas y Dinámicas
Una lista puede ser estática o dinámica dependiendo de cómo es implementada, si es implementada como un **vector unidimensional**, la lista es estática.

Sin embargo, si es implementada utilizando una **lista enlazada**, la lista es dinámica. Esta implementación hace uso de la memoria de forma dinámica, es decir, utiliza memoria acorde a su necesidad.

## Operaciones elementales sobre Listas
- Leer
- Recorrer
- Insertar 
- Eliminar
- Ordenar
- Buscar

## Tipos de Listas
Acorde su implementacin, pueden existir muchas variaciones, donde las operaciones son las mismas pero los detalles de implementación son diferentes.

### Listas No Enlazadas
La listas no enlazadas se implementan utilizando un vector unidimensional. El primer paso para implementar este tipo de lista, es definir el tamaño del vector, que será el tamaño de la lista, una vez definido este no puede ser alterado. 

Los elementos se almacenan de forma contigua en posiciones consecutivas de la memoria y para acceder a ellos se utiliza el índice, como si fuese un vector.

El principal problema de esta implementación es que se debe definir el tamaño del vector de forma *a priori*, si el vector se llena, no será posible agregar más elementos, entonces es necesario crear un vector más grande y migrar todos los elementos del vector original, y finalmente liberar el espacio en la memoria.

En general, los vectores no son buenos para implementar listas, considerando que las operaciones de actualización (insertar/eliminar) son costosas, además que la cantidad total de elementos a insertar suele ser desconocida.

![Lista utilizando un vector](images/list/lista-vector.svg)

### Listas Enlazadas
Una lista enlazada es un conjunto de elementos donde cada elemento debe tener al menos dos campos: un campo que almacena el valor o dato del elemento y un campo (puntero) que contiene la posición del siguiente elemento de la lista, esta estructura recibe el nombre de **nodo**.

![Nodo](images/list/nodo.svg)

Las listas simplemente enlazadas nos permiten a partir de un elemento acceder directamente a cualquiera de los elementos que le preceden.

Existe un puntero inicial denominado **cabecera (o _head_)**, que marca el comienzo de la lista, este almacena la posición del primer nodo de la lista, mientras que el puntero del último elemento no almacena ninguna dirección, es decir, es _nulo_, esto denota el final de la lista, y que ya no existen más elementos por recorrer.

Si se conoce la dirección al primer elemento de la lista, es posible realizar todas las operaciones sobre la misma, considerando que solo debemos navegar entre los diferentes nodos conectados por punteros.

![Lista utilizando Nodos](images/list/lista-simple.svg)

En la figura se ilustra una lista enlazada utilizando los nodos para enlazar cada elemento de la lista.

### Listas Doblemente Enlazadas
Las listas doblemente enlazadas son listas que pueden recorrerse en ambas direcciones, donde cada nodo contiene el campo de dato y a la vez dos campos punteros; uno apunta al nodo anterior, y el otro al nodo siguiente.  

![Nodo con doble enlace](images/list/nodo-doble.svg)

Como cada elemento tiene dos punteros, en consecuencia una lista doblemente enlazada ocupa más espacio en memoria que una lista simplemente enlazada para una misma cantidad de información.

Además, la lista necesita dos punteros _cabecera y fin_, que apuntan al primer y último nodo, respectivamente.
La variable _cabecera_ y el puntero _sig_ permiten recorrer la lista en el sentido normal y la variable _fin_ y el puntero _ant_ permiten recorrerla en sentido inverso.

![Lista doblemente enlazada](images/list/lista-doble.svg)

### Listas Circulares
Las listas circulares o listas en anillo, a diferencia de las listas enlazadas donde el último elemento apunta a _nulo_, en estas estructuras el último puntero del último elemento apunta al primer elemento de la lista, de forma que es posible iterar sobre la lista, sin necesidad de volver acceder desde la cabecera.

![Lista Circular](images/list/lista-circular.svg)


---

¡Gracias por leer! 

Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido puedes realizar una donación *[invitándome un café](https://www.buymeacoffee.com/szalimben)*  que me será de mucha ayuda!