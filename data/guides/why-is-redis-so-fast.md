---
title: "Почему Redis работает так быстро?"
description: "Основные причины высокой скорости Redis."
image: "https://assets.bytebytego.com/diagrams/0422-why-is-redis-so-fast.png"
createdAt: '2024-03-07'
draft: false
categories:
  - caching-performance
tags:
  - "Redis"
  - "Performance"
---

![](https://assets.bytebytego.com/diagrams/0422-why-is-redis-so-fast.png)

На схеме выше показаны три основные причины.

* Redis хранит данные в оперативной памяти. Доступ к ней как минимум в 1000 раз быстрее случайного доступа к диску.

* Redis использует мультиплексирование ввода-вывода и однопоточный цикл выполнения, чтобы эффективно обрабатывать операции.

* Redis использует несколько эффективных низкоуровневых структур данных.
