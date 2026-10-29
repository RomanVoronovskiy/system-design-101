---
title: "Общая архитектура Netflix"
description: "Архитектура Netflix: от клиентских приложений до серверных сервисов."
image: 'https://assets.bytebytego.com/diagrams/0288-netflix-overal-arch.png'
createdAt: '2024-03-01'
draft: false
categories:
  - real-world-case-studies
tags:
  - Architecture
  - Streaming
---

![](https://assets.bytebytego.com/diagrams/0288-netflix-overal-arch.png)

Материал подготовлен по инженерным блогам Netflix и открытым проектам компании. Если заметите неточности, сообщите нам.

**Мобильные и веб-приложения:** нативные мобильные приложения разрабатываются на Swift и Kotlin, а веб-приложение — с использованием React.

**Взаимодействие фронтенда и сервера:** Netflix использует GraphQL.

**Серверные сервисы:** ZUUL, Eureka, Spring Boot и другие технологии.

**Базы данных:** EVCache, Cassandra, CockroachDB и другие решения.

**Сообщения и потоки:** Apache Kafka и Flink.

**Хранение видео:** S3 и Open Connect.

**Обработка данных:** Flink и Spark. Результаты визуализируются в Tableau. Redshift используется для обработки структурированных данных в хранилище.

**CI/CD:** JIRA, Confluence, PagerDuty, Jenkins, Gradle, Chaos Monkey, Spinnaker, Atlas и другие инструменты.
