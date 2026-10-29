---
title: "Событийная архитектура McDonald’s"
description: "Событийная архитектура McDonald’s: масштабируемость и эффективность."
image: 'https://assets.bytebytego.com/diagrams/0266-mcdonald-s-event-driven-architecture.png'
createdAt: '2024-02-18'
draft: false
categories:
  - real-world-case-studies
tags:
  - Event-Driven Architecture
  - Case Study
---

![](https://assets.bytebytego.com/diagrams/0266-mcdonald-s-event-driven-architecture.png)

Думаете, что знаете о McDonald’s всё? А что насчёт событийной архитектуры компании?

McDonald’s стандартизирует события с помощью следующих компонентов:

* **Реестр событий (Event Registry):** определяет стандартные схемы событий.
* **Собственные SDK:** обрабатывают события и ошибки.
* **Шлюз событий (Event Gateway):** выполняет аутентификацию и авторизацию.
* **Утилиты и инструменты:** помогают исправлять события, поддерживать работоспособность кластеров и выполнять административные задачи.

Для масштабирования обработки McDonald’s использует региональную архитектуру на AWS, обеспечивающую глобальную доступность. Внутри региона производители разделяют события по предметным областям, и каждую область обрабатывает отдельный кластер MSK. Он автоматически масштабируется по метрикам MSK, например загрузке процессора. Процесс автомасштабирования построен на Step Functions и задачах перераспределения.

Источник: [McDonald’s event-driven architecture](https://medium.com/mcdonalds-technical-blog/behind-the-scenes-mcdonalds-event-driven-architecture-51a6542c0d86)
