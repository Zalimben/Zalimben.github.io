---
title: "Árboles"
date: 2022-03-22T11:34:06-03:00
draft: false
description: "Los árboles son estructuras de datos no lineales, donde cada elemento del árbol es una estructura del tipo nodo."
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/tree/tree-double-example.svg', 'images/tree/tree-example.svg']
transform: -3%
blog_list_image: images/tree/tree-example.svg
author: Saúl Zalimben
slug: tree
idiom: Español
---

Los árboles son estructuras de datos no lineales, donde cada elemento del árbol es una estructura del tipo **nodo (_node_)**, y hace referencia a otros nodos dentro del árbol, las conexiones entre nodos se denominan **aristas o ramas o arcos (_edge_)**.

Las estructuras del tipo árbol se usan principalmente para representar datos con una relación jerárquica entre sus elementos, como son árboles genealógicos, jerarquías y agrupaciones militares, dependencias de tareas, etc.

Un árbol _A_ es un conjunto finito de uno o más nodos (_n_), tales que:
- Existe un nodo especial denominado **raíz** _(n<sub>0</sub>)_ del árbol.
- Los nodos restantes _(n<sub>1</sub>, n<sub>2</sub>, ..., n<sub>n</sub>)_ se dividen en _m >= 0_ conjuntos disjuntos denominado _A<sub>1</sub>, A<sub>2</sub>, ..., A<sub>m</sub>_, cada uno de los cuales es, a su vez, **un árbol**. Estos árboles se llaman **subárboles** de la raíz.

>
> La definición de árbol implica una estructura recursiva, es decir, un árbol es el conjunto de subárboles.
>  

## Definiciones sobre Árboles
Las definiciones a tener en cuenta son:
- **Raíz del árbol**, todos los árboles que no están vacíos tienen un único nodo raíz. Todos los demás elementos o nodos se derivan o descienden de él. El nodo raíz no tiene padre, es decir, no es hijo de ningún otro nodo.
- **Nodo**, son los vértices o elementos del árbol. 
- **Nodo terminal o nodo hoja**, son los nodos que no contienen ningún subárbol.
- **Nodo no terminal**, todo nodo que no es hoja se asocia a uno o varios subárboles llamados descendientes o hijos. De igual forma, cada nodo tiene asociado un antecesor o ascendiente llamado **padre**. También se los conoce como nodos **interiores o internos**.

![Árbol. Ancestros y Descendientes](images/tree/tree-olds.svg)

- Un árbol con ningún nodo es un árbol **nulo o vacío**; no tiene raíz.
- Todos los nodos tienen un solo **padre**, excepto el nodo raíz, que no tiene padre.
- Los nodos de un mismo padre se llaman **nodos hermanos**.

![Árbol. Padres & Hijos](images/tree/tree-root-child.svg)

- Se denomina **camino** a una secuencia de nodos.
- Existe un camino de longitud 0 de un nodo a sí mismo que se conoce como **camino trivial**.
- Cada nodo tiene asociado un número de **nivel** que determina la longitud del camino desde el nodo raíz al nodo específico.
- Por cada nodo en un árbol, existe un camino único de la raíz a dicho nodo. La longitud de este camino es conocida como la **profundidad o altura** del nodo.
- La **altura** de un árbol es definida como la máxima profundidad de cualquier nodo del árbol. La altura de un árbol con un solo nodo es 0 (solo la raíz), mientras que la altura de un árbol vacío es –1, por conveniencia.

![Árbol. Niveles & Profundidad](images/tree/tree-level.svg)

- El **peso** de un árbol es el número de nodos terminales.
- El **grado de un nodo** es definido como el número de sus hijos directos.
- Un nodo hoja tiene **grado cero**.
- Una colección de dos o más árboles se llama **bosque**.

## Operaciones elementales sobre Árboles 
- Insertar 
- Eliminar
- Buscar
- Recorrer

## Árbol Binario

Un árbol binario es un conjunto finito de cero o más nodos, tales que:
- Existe un nodo denominado raíz del árbol.
- Cada nodo puede tener 0, 1 o 2 subárboles, conocidos como subárbol izquierdo y subárbol derecho. 

> Un árbol binario es una especialización dentro de las estructuras del tipo árbol.

### Árboles Binarios de Búsqueda
Un árbol binario de búsqueda, es un árbol binario que cumple que el subárbol izquierdo de cualquier nodo (si no está vacío) contiene valores menores que el que contiene dicho nodo, y el subárbol derecho (si no está vacío) contiene valores mayores, donde existe una relación de orden establecida entre los elementos de los nodos.


El árbol binario de búsqueda se construye teniendo en cuenta las siguientes premisas:
- El primer elemento se utiliza para crear el nodo raíz.
- Los elementos del árbol deben ser tales que pueda existir un orden dentro del mismo.
- Todos los elementos del subárbol izquierdo son menor o igual al valor del nodo padre.
- Todos los elementos del subárbol derecho son mayores que el valor del nodo padre.

> Un árbol binario de búsqueda es una especialización de los árboles binarios.

![Árbol Binario](images/tree/tree-binary.svg)
> Ejemplo de árbol binario de búsqueda

---

¡Gracias por leer! 

Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido puedes realizar una donación *[invitándome un café](https://www.buymeacoffee.com/szalimben)* que me será de mucha ayuda!