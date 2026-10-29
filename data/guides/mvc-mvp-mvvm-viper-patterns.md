---
title: "Шаблоны MVC, MVP, MVVM и VIPER"
description: "Сравнение архитектурных шаблонов MVC, MVP, MVVM и VIPER."
image: "https://assets.bytebytego.com/diagrams/0143-client-arch-patterns.png"
createdAt: "2024-03-12"
draft: false
categories:
  - software-architecture
tags:
  - "architectural patterns"
  - "software design"
---

![Шаблоны MVC, MVP, MVVM и VIPER](https://assets.bytebytego.com/diagrams/0143-client-arch-patterns.png)

Чем отличаются архитектурные шаблоны MVC, MVP, MVVM, MVVM-C и VIPER?

Они широко применяются при разработке приложений для iOS и Android. Новые шаблоны появлялись, чтобы преодолеть ограничения предыдущих. В чём их различия?

* Самому старому шаблону, MVC, уже почти 50 лет.
* В каждом шаблоне есть представление — View (V), которое отображает содержимое и принимает пользовательский ввод.
* В большинстве есть модель — Model (M), отвечающая за бизнес-данные.
* Controller, Presenter и ViewModel выступают посредниками между представлением и моделью; в VIPER роль модели выполняет Entity.
* Код таких посредников может быть довольно сложным. Разные шаблоны предлагают способы упростить его сопровождение.
