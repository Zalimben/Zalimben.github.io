---
title: "Grafos"
date: 2022-03-22T00:36:53-03:00
draft: true
description: "Son estructuras de datos no lineales, utilizadas para representar datos adyacentes."
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/graph/graph-bucle.svg']
blog_list_image: 'images/graph/graph.svg'
width: 57%
transform: 0%
author: Saúl Zalimben
slug: graph
idiom: Español
---

Si acabas de encontrar esta publicación, antes de continuar te recomiendo que le des un vistazo a [Estructuras de Datos. Conceptos](blog/spanish/posts/estructura-datos-conceptos) el cual brinda conceptos claves para comprender las Estructuras de Datos.

---

Los **grafos** son estructuras de datos no lineales, utilizadas para representar datos adyacentes. Se representa como el conjunto de vértices o nodos y de aristas o arcos. Esta estructura de datos es el principal foco de estudio de la Teoría de Grafos.

>
>**Teoría de Grafos.** Rama de las matemáticas y las ciencias de la computación que estudia las propiedades de los grafos.
>

Un grafo _G_ es un par ordenado _G = (V,E)_, donde:
- _V_ es un conjunto de vértices o nodos _V=\{v<sub>1</sub>, v<sub>2</sub>, ... , v<sub>n</sub>\}_, y 
- _E_ es un conjunto de aristas o arcos 
    _E = \{\{v<sub>1</sub>, v<sub>2</sub>\},\{v<sub>2</sub>, v<sub>4</sub>\} ... , \{v<sub>m</sub>, v<sub>n</sub>\}\}_, que relacionan los nodos.


![Ejemplo de Grafo](images/graph/graph-bucle.svg)

Un grafo no contempla las restricciones que existen para los árboles, es decir, no existe un máximo de nodos que pueden apuntar al mismo nodo, se los puede ver como una generalización de la estructura del tipo árbol.

Existen muchas analogías en el mundo real, la red de rutas de un país, la red de enlaces aéreos, red eléctrica, etc. En una red de rutas, los nudos o intersecciones representan los **vértices** del grafo y las rutas de unión los **arcos**, de modo que cada arco puede ser asociado a un dato específico tal como la distancia, el consumo de combustible, etc.

>
>_Los árboles son una especialización de un grafo, en el cual no existen ciclos, es decir, un árbol es un grafo conexo acíclico._
>

## Operaciones elementales sobre Grafos
- Insertar 
- Eliminar
- Buscar
- Recorrer

## Definiciones sobre Grafos
- Se denomina **grafo nulo o vacío** a aquel grafo que no tiene vértices ni arcos.
- El **orden** del grafo _G_ es igual al número de vértices, _|V|_.
- Un **grafo vacío** es de orden cero.
- El **grado** de un vértice se define como el número de vértices adyacentes que tiene el vértice.
- En grafos dirigidos el **grado de entrada** de un vértice o nodo _V_ es igual al número de arcos que lo tienen como extremo, es decir, igual al número de vértices adyacentes que tiene el vértice. Mientras que el **grado de salida** es el número de vértices adyacentes a un vértice dado.
- Dos o más arcos son **paralelas** si relacionan el mismo par de vértices.
- Se dice que dos vértices son **adyacentes** si existe un arco entre ambos vértices. Si el arco es **{K, L}**, entonces, K es adyacente a L, y L es adyacente a K.
- Un **camino** es una secuencia ordenada de vértices _\{v<sub>0</sub>, v<sub>1</sub>, v<sub>2</sub>, ..., v<sub>n</sub>\}_. Se conoce como el camino desde _v<sub>0</sub>_ hasta _v<sub>n</sub>_
- Un **camino simple** no tiene vértices repetidos excepto para el primer y último vértice.
- Si un camino simple donde el primer y último vértice son iguales se conoce como un **ciclo o bucle**, es decir, un arco que relaciona al mismo nodo.

![Ejemplo de grados en un grafo](images/graph/graph-grado.svg)


## Clasificación de Grafos
Los grafos pueden clasificarse acorde a sus propiedades, según su estructura, dirección y conectividad.

### Sencillo y Múltiple
Un grafo _G_ se denomina **sencillo** si se cumplen las siguientes condiciones:
- No tiene bucles, no existe un arco tal que _\{v<sub>i</sub>, v<sub>i</sub>\}_.
- No existe más que un arco para unir dos nodos, es decir, no existe más que un arco \{v<sub>i</sub>, v<sub>j</sub>\} para cualquier par de vértices _v<sub>i</sub>_, _v<sub>j</sub>_.

Un grafo que no es sencillo se denomina grafo **múltiple**.

![Grafo con bucle](images/graph/graph-bucle.svg)


### Dirigido y No Dirigido
La teoría de grafos considera los siguientes tipos de grafos según su dirección:

- **Dirigidos**, los vértices apuntan unos a otros; los arcos están dirigidos o tienen dirección, si existe un arco _\{v<sub>i</sub>, v<sub>j</sub>\}_, entonces se dice que existe un camino de _v<sub>i</sub>_ a _v<sub>j</sub>_, pero esto no implica que existe un camino de _v<sub>j</sub>_ a _v<sub>i</sub>_.
- **No Dirigidos**, los vértices están relacionados, pero no se apuntan unos a otros, si existe un arco _\{v<sub>i</sub>, v<sub>j</sub>\}_, entonces se dice que existe un camino de _v<sub>i</sub>_ a _v<sub>j</sub>_ y de _v<sub>j</sub>_ a _v<sub>i</sub>_ para cualquier par de vértices _v<sub>i</sub>_, _v<sub>j</sub>_.

![Grafo con bucle](images/graph/graph-no-dirigido.svg)

### Conexo y No Conexo
Finalmente, según la conectividad de los grafos, estos pueden ser:
- **Conexo o conectado**, si existe siempre un camino que une cualquier par de vértices, todos sus vértices están conectados por un camino. Se dice que un grafo es **fuertemente conexo** cuando es un grafo dirigido tal que para cualquier par de nodos existe un camino que los une.
- **No Conexo o desconectado**, existen vértices que no están unidos por un camino.

![Grafo con bucle](images/graph/graph-conexo.svg)

### Completos, Dispersos y Densos

Según el número de arcos que contiene, un grafo es **completo** si cuenta con todos los arcos posibles, es decir, todos los nodos están conectados con todos, es **disperso** si tiene relativamente pocos arcos y **denso** si le faltan pocos para ser completo.

## Grafos Ponderados

Tanto las arcos como los vértices pueden tener asociada una etiqueta. Si la etiqueta que se asocia es un número se le llama **peso, costo o longitud**. 
Un grafo cuyas arcos o vértices tienen pesos asociados recibe el nombre de grafo etiquetado o también conocido como **grafo con pesos o  ponderado**.
Un grafo donde las aristas no tienen costos o pesos asociados se conoce como grafo sin pesos. También podría considerarse a un grafo sin pesos
como un grafo con pesos donde cada arista tiene un peso igual a 1.

La longitud de un camino en un grafo con pesos es la suma de los pesos de todas las aristas que componen el camino.
Por ejemplo, la siguiente figura ilustra la longitud del camino $(1, 4, 7)$ donde $(1-4)$ = 5,1 + $(4-7)$ 3,7 = 8,8

![Grafo con bucle](images/graph/graph-peso.svg)

---

¡Gracias por leer! 

Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido puedes realizar una donación *[invitándome un café](https://www.buymeacoffee.com/szalimben)* que me será de mucha ayuda!