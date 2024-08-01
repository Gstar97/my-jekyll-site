---
layout: post
title: "Las principales características de Jekyll"
date: 2024-08-01 15:00:00 +0000
categories: jekyll tutorial
---

## Introducción

Jekyll es una herramienta de generación de sitios estáticos que se ha vuelto muy popular entre desarrolladores y bloggers por su simplicidad y flexibilidad. En este post, exploraremos las principales características de Jekyll y cómo puedes utilizarlas para crear un sitio web eficiente.

## Características de Jekyll

### 1. Generador de Sitios Estáticos

Jekyll toma tus archivos de texto sin formato (Markdown o Textile) y los convierte en un sitio web estático que puedes alojar en cualquier servidor web.

### 2. Compatible con GitHub Pages

Jekyll es la herramienta que impulsa GitHub Pages, lo que facilita la publicación de sitios directamente desde un repositorio de GitHub.

### 3. Plantillas Flexibles

Puedes personalizar el diseño de tu sitio utilizando layouts y includes. Aquí tienes un ejemplo de cómo se ve una estructura básica de layout en Jekyll:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ page.title }}</title>
  <link rel="stylesheet" href="{{ "/assets/main.css" | relative_url }}">
</head>
<body>
  <header>
    <h1>{{ site.title }}</h1>
  </header>
  <main>
    {{ content }}
  </main>
  <footer>
    <p>© {{ site.time | date: "%Y" }} {{ site.title }}</p>
  </footer>
</body>
</html>
