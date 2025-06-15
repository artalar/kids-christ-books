---
title: Расширенные функции Markdown
published: 2025-04-25
tags:
  - Руководство
toc: false
lang: ru
abbrlink: markdown-extended-features
---

Здесь представлены некоторые расширенные функции Markdown, поддерживаемые темой Retypeset, включая примеры синтаксиса и их стилистические эффекты.

## Подписи к изображениям

Для создания автоматических подписей к изображениям используйте стандартный синтаксис изображений Markdown `![alt](src)`. Чтобы скрыть подпись, добавьте подчёркивание `_` перед текстом `alt` или оставьте текст `alt` пустым.

### Синтаксис

```
![Описание изображения](https://image.example.com/image-01.webp)

![_Описание изображения](https://image.example.com/image-01.webp)
```

### Результат

![Описание изображения](https://image.radishzz.cc/image/gallery/06.webp)

![_Описание изображения](https://image.radishzz.cc/image/gallery/06.webp)

## Карточки репозиториев Github

Для создания карточки репозитория Github используйте листовую директиву `::github{repo="owner/repo"}`. Данные репозитория в режиме реального времени загружаются из API GitHub после загрузки страницы.

### Синтаксис

```
::github{repo="radishzzz/astro-theme-retypeset"}
```

### Результат

::github{repo="radishzzz/astro-theme-retypeset"}

## Примечания

Для создания блоков примечаний используйте синтаксис GitHub `> [!TYPE]` или контейнерную директиву `:::type`. Поддерживаются пять типов: `note`, `tip`, `important`, `warning` и `caution`.

### Синтаксис

```
> [!NOTE]
> Полезная информация, которую пользователи должны знать, даже при беглом просмотре.

> [!TIP]
> Полезные советы, как делать что-то лучше или проще.

> [!IMPORTANT]
> Ключевая информация, которую пользователи должны знать для достижения своей цели.

:::warning
Срочная информация, требующая немедленного внимания пользователя для предотвращения проблем.
:::

:::caution
Предупреждает о рисках или негативных последствиях определённых действий.
:::

:::note[ПОЛЬЗОВАТЕЛЬСКИЙ ЗАГОЛОВОК]
Это примечание с пользовательским заголовком.
:::
```

### Результат

> [!NOTE]
> Полезная информация, которую пользователи должны знать, даже при беглом просмотре.

> [!TIP]
> Полезные советы, как делать что-то лучше или проще.

> [!IMPORTANT]
> Ключевая информация, которую пользователи должны знать для достижения своей цели.

:::warning
Срочная информация, требующая немедленного внимания пользователя для предотвращения проблем.
:::

:::caution
Предупреждает о рисках или негативных последствиях определённых действий.
:::

:::note[ПОЛЬЗОВАТЕЛЬСКИЙ ЗАГОЛОВОК]
Это примечание с пользовательским заголовком.
:::

## Видео

Для добавления видео скопируйте код для встраивания с YouTube или другой видеоплатформы и вставьте его в markdown файл. Не нужно сохранять параметры `width` и `height`.

### Синтаксис

```html
<!-- Youtube -->
<iframe src="https://www.youtube.com/embed/9pP0pIgP2kE?si=Rlk4C4ltaVPHXZ80" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<!-- Bilibili -->
<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=930327443&bvid=BV1sK4y1Z7KG&cid=329802177&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
```

### Результат

<iframe src="https://www.youtube.com/embed/9pP0pIgP2kE?si=Rlk4C4ltaVPHXZ80" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=930327443&bvid=BV1sK4y1Z7KG&cid=329802177&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
