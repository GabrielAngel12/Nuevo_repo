---
title: 'Funcion de los estilos'
charset: utf-8
pubDate: 2023-09-27
description: 'Esta es la forma en que conoceremos como funcionan y como implementamos css dentro de una pagibb¿na creadacon astro'
---

# Como implentar css dentro del entorno de ***Astro*** para la creacion de la pagina web
Published on: 2023-09-27

Veremos como implementar css o declarar las variables de css en este entorno

## Declaracion dentro script frontmatter
``const skillColor = "navy";`` 

Este pedaso de codigo lo implementaremos para poder cambiar el color de las plabras que ya declaramos como ``<h1>``. Para continuar insertaremos las siguiente etiqueta ``<style>`` con los siguientes terminos:

    ``<style define:vars = {{skillColor}}>
        h1 {
            color: purple;
            font-size: 4rem;
        }
        .skill {
            color: var(--skillColor);
            font-weight: bold;
        }
    
    </style>``
Al igual que haremos que todos los elementos tengan el mismo color, a lo cual haremos lo siguiente:

``<li class="skill">``

