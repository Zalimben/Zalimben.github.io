---
title: "Pilas y Colas"
date: 2022-03-15
draft: false
description: "Las pilas y colas son estructuras de datos lineales, donde existen restricciones para insertar y eliminar elementos."
tags: ['spanish', 'español','fundamentos', 'estructura de datos']
images: ['images/stack-queue/stackAndQueue.svg']
transform: -16%
blog_list_image: images/stack-queue/stackAndQueue.svg
author: Saúl Zalimben
slug: stack-queue
idiom: Español
---

Si acabas de encontrar esta publicación, antes de continuar te recomiendo que le des un vistazo a [Estructuras de Datos. Conceptos](blog/spanish/posts/estructura-datos-conceptos) el cual brinda conceptos claves para comprender las Estructuras de Datos.

---

Las pilas y colas son estructuras de datos lineales, donde existen restricciones para insertar y eliminar elementos. Son casos particulares de la estructura lista, y se pueden implementar mediante vectores o listas enlazadas.

### Operaciones elementales sobre Pilas y Colas
- Insertar: Push -> apilar (Pila), Enqueue -> encolar (Cola)
- Eliminar: Pop  -> desapilar (Pila),  Dequeue -> desencolar (Cola)

## Pilas
Una Pila o Stack es un caso particular de la lista donde la inserción y eliminación de elementos se realizan solo por un extremo que se denomina cima o tope _(top)_. Funciona exactamente como su nombre lo indica, y con numerosas analogías en la vida real: una pila de libros, una pila de monedas, pila de platos, etc.

Este comportamiento está basado en el principio _"último en entrar, primero en salir"_, también conocido como **LIFO**, por su nombre en inglés _"last-in, first-out"_, que dicta que el primer elemento que fue añadido a la pila será el último en ser removido de la misma.

![Pila](images/stack-queue/stack.svg)

## Colas
Una **Cola o Queue** es un caso particular de la lista donde la inserción y eliminación de elementos se realizan por los extremos de la lista; las eliminaciones se realizan al principio de la lista, o el frente _(front)_ de la misma, y las inserciones se realizan en el otro extremo, el final _(rear)_. Algunas analogías en la vida real:  cola de personas en el banco, cola de vehículos en el semáforo, etc.

Este comportamiento está basado en el principio _"primero en entrar, primero en salir"_, también conocido como **FIFO**, por su nombre en inglés _"first-in, first-out"_, que dicta que el primer elemento que fue añadido a la cola será el primero en ser removido.

![Cola](images/stack-queue/queue.svg)

---

¡Gracias por leer!
Puedes ver otras entradas relacionadas en el tag [estructura-de-datos](tags/estructura-de-datos/).


Ponte en contacto en Twitter [@sZalimben](https://twitter.com/sZalimben), y si te gusta mi contenido puedes realizar una donación *[invitándome un café](https://www.buymeacoffee.com/szalimben)* que me será de mucha ayuda!