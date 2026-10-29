---
title: "Технологический стек Netflix"
description: "Технологии, на которых построена потоковая инфраструктура Netflix."
image: 'https://assets.bytebytego.com/diagrams/0286-netflix-tech-stack.png'
createdAt: '2024-03-15'
draft: false
categories:
  - real-world-case-studies
tags:
  - Architecture
  - Streaming
---

Материал подготовлен по инженерным блогам Netflix и открытым проектам компании. Если заметите неточности, сообщите нам.

![](https://assets.bytebytego.com/diagrams/0286-netflix-tech-stack.png)

* **Мобильные и веб-приложения:** нативные мобильные приложения создаются на Swift и Kotlin, веб-приложение — с помощью React.
* **Взаимодействие фронтенда и сервера:** GraphQL.
* **Серверные сервисы:** ZUUL, Eureka, Spring Boot и другие технологии.
* **Базы данных:** EVCache, Cassandra, CockroachDB и другие решения.
* **Сообщения и потоки:** Apache Kafka и Flink.
* **Хранение видео:** S3 и Open Connect.
* **Обработка данных:** Flink и Spark, с последующей визуализацией в Tableau. Redshift применяется для обработки структурированных данных в хранилище.
* **CI/CD:** JIRA, Confluence, PagerDuty, Jenkins, Gradle, Chaos Monkey, Spinnaker, Atlas и другие инструменты.
