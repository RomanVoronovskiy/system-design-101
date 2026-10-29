---
title: "Архитектура платформы экспериментов"
description: "Архитектура платформы экспериментов и её основные компоненты."
image: "https://assets.bytebytego.com/diagrams/0189-experiment-framework.jpg"
createdAt: "2024-03-08"
draft: false
categories:
  - how-it-works
tags:
  - "A/B Testing"
  - "Experimentation"
---

[![Архитектура платформы экспериментов](https://assets.bytebytego.com/diagrams/0189-experiment-framework.jpg)](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Fd79ea50e-e386-41c9-9f66-e28006ed1115_1677x1536.jpeg)

На схеме показан один из вариантов архитектуры платформы экспериментов. Содержание взято из книги «Trustworthy Online Controlled Experiments»; иллюстрация перерисована автором материала. Платформа включает четыре основных компонента.

## Основные компоненты

* **Определение, настройка и управление экспериментами через пользовательский интерфейс.** Эти сведения сохраняются в конфигурации системы экспериментов.
* **Развёртывание экспериментов** на серверной и клиентской стороне, включая назначение вариантов и настройку параметров.
* **Инструментирование экспериментов** — сбор необходимых данных о ходе их выполнения.
* **Анализ результатов экспериментов.**
