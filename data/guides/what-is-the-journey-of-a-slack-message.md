---
title: "Какой путь проходит сообщение в Slack?"
description: "Как сообщение Slack проходит от отправителя к получателю через серверную инфраструктуру."
image: 'https://assets.bytebytego.com/diagrams/0338-slack-message-journey.jpg'
createdAt: '2024-03-08'
draft: false
categories:
  - real-world-case-studies
tags:
  - System Design
  - Messaging
---

![](https://assets.bytebytego.com/diagrams/0338-slack-message-journey.jpg)

В инженерной статье Slack описала устройство своей системы обмена сообщениями в реальном времени. Ниже — краткое изложение.

Сообщение проходит через пять важных серверных компонентов:

* **WebApp:** предоставляет API для клиента Slack.
* **Admin Server (AS):** по идентификатору канала находит нужный Channel Server.
* **Channel Server (CS):** хранит историю сообщений канала.
* **Gateway Server (GS):** развёрнут в каждом географическом регионе и поддерживает подписки на каналы через WebSocket.
* **Envoy:** прокси для облачных приложений.

* Каналов очень много, поэтому для распределения миллионов каналов между серверами используется консистентное хеширование.
* Сообщение проходит через WebApp и Admin Server к нужному Channel Server.
* Channel Server отправляет сообщение получателям через Gateway Server и прокси Envoy.
* Получатели используют WebSocket — механизм двунаправленного обмена, благодаря которому обновления приходят в реальном времени.
