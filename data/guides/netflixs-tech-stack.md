---
title: "Технологический стек Netflix"
description: "Изучайте технологии, лежащие в основе инфраструктуры потоков Netflix."
image: 'https://assets.bytebytego.com/diagrams/0286-netflix-tech-stack.png'
createdAt: '2024-03-15'
draft: false
categories:
  - real-world-case-studies
tags:
  - Architecture
  - Streaming
---

Эта статья основана на исследованиях многих блогов Netflix и проектов с открытым исходным кодом. Если вы найдёте какие-либо неточности, пожалуйста, не стесняйтесь сообщить нам.

![](https://assets.bytebytego.com/diagrams/0286-netflix-tech-stack.png)

*   Мобильный и веб: Netflix принял Swift и Kotlin для создания местных мобильных приложений. Для своего веб-приложения он использует React.

*   Передняя связь/сервер: графа QL.

*   Услуги на основе резервного финансирования: Netflix опирается на ZUUL, Eureka, Spring Boot Framework и другие технологии.

*   Базы данных: Netflix использует EV-каче, C4andra, CockroachDB и другие базы данных.

*   Пересылание/передача сообщений: Netflix использует Apache Kafka и Fink для обмена сообщениями и потоков.

*   В видеохранилище: Netflix используют S3 и Open Connect для видеохранилищ.

*   Обработка данных: Netflix использует Flink и Spark для обработки данных, которые затем отображаются с помощью Tableau. Для обработки структурированной информации о хранилищах данных используется система " Redchredchange ".

*   CI/CD: Netflix использует различные инструменты, такие как JIARA, Confluence, PagerDuty, Jenkins, Gradle, Chaos Onekey, Spinnaaker, Altas и т.д.
