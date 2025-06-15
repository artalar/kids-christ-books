---
title: Características Extendidas de Markdown
published: 2025-04-25
tags:
  - Guía
toc: false
lang: es
abbrlink: markdown-extended-features
---

Aquí presentamos algunas características extendidas de Markdown compatibles con Retypeset, incluyendo ejemplos de sintaxis y sus efectos estilísticos.

## Leyendas de Figuras

Para crear leyendas automáticas para figuras, utilice la sintaxis estándar de imágenes de Markdown `![alt](src)`. Para ocultar la leyenda, añada un guion bajo `_` antes del texto `alt` o deje el texto `alt` vacío.

### Sintaxis

```
![Descripción de la imagen](https://image.example.com/image-01.webp)

![_Descripción de la imagen](https://image.example.com/image-01.webp)
```

### Resultado

![Descripción de la imagen](https://image.radishzz.cc/image/gallery/06.webp)

![_Descripción de la imagen](https://image.radishzz.cc/image/gallery/06.webp)

## Tarjetas de Repositorios de Github

Para crear una tarjeta de repositorio de Github, utilice la directiva hoja `::github{repo="owner/repo"}`. Los datos del repositorio se obtienen en tiempo real de la API de GitHub después de que la página se carga.

### Sintaxis

```
::github{repo="radishzzz/astro-theme-retypeset"}
```

### Resultado

::github{repo="radishzzz/astro-theme-retypeset"}

## Advertencia

Para crear bloques de advertencia, utilice la sintaxis de GitHub `> [!TYPE]` o la directiva contenedor `:::type`. Se admiten cinco tipos: `note`, `tip`, `important`, `warning` y `caution`.

### Sintaxis

```
> [!NOTE]
> Información útil que los usuarios deben conocer, incluso al leer por encima.

> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.

> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.

:::warning
Información urgente que requiere atención inmediata del usuario para evitar problemas.
:::

:::caution
Advierte sobre riesgos o resultados negativos de ciertas acciones.
:::

:::note[TÍTULO PERSONALIZADO]
Esta es una nota con un título personalizado.
:::
```

### Resultado

> [!NOTE]
> Información útil que los usuarios deben conocer, incluso al leer por encima.

> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.

> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.

:::warning
Información urgente que requiere atención inmediata del usuario para evitar problemas.
:::

:::caution
Advierte sobre riesgos o resultados negativos de ciertas acciones.
:::

:::note[TÍTULO PERSONALIZADO]
Esta es una nota con un título personalizado.
:::

## Videos

Para incrustar videos, copie el código de inserción de YouTube u otras plataformas de video y péguelo en su archivo markdown. No necesita mantener los parámetros `width` y `height`.

### Sintaxis

```html
<!-- Youtube -->
<iframe src="https://www.youtube.com/embed/9pP0pIgP2kE?si=Rlk4C4ltaVPHXZ80" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<!-- Bilibili -->
<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=930327443&bvid=BV1sK4y1Z7KG&cid=329802177&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
```

### Resultado

<iframe src="https://www.youtube.com/embed/9pP0pIgP2kE?si=Rlk4C4ltaVPHXZ80" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=930327443&bvid=BV1sK4y1Z7KG&cid=329802177&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
