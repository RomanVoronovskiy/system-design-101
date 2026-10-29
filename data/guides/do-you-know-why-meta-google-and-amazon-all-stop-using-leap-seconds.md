---
title: "Почему Meta, Google и Amazon перестают использовать високосные секунды"
description: "Узнайте, почему технологические гиганты отказываются от дополнительных секунд."
image: "https://assets.bytebytego.com/diagrams/0363-do-you-know-why-meta-google-and-amazon-all-stop-using-leap-seconds.jpeg"
createdAt: "2024-02-04"
draft: false
categories:
  - cloud-distributed-systems
tags:
  - "Time Synchronization"
  - "Leap Seconds"
---

![Почему Meta, Google и Amazon перестают использовать високосные секунды](https://assets.bytebytego.com/diagrams/0363-do-you-know-why-meta-google-and-amazon-all-stop-using-leap-seconds.jpeg)

Каждые несколько лет происходит особый феномен: второе после «23:59:59» идет не «00:00:00», а «23:59:60». Это называется дополнительной секундой, которая может легко вызвать ошибки обработки времени, если с ней не обращаться осторожно.

Всегда ли нам нужно обрабатывать дополнительные секунды? Это зависит от того, какое представление времени используется. Обычно используемые представления времени включают UTC, GMT, TAI, временную метку Unix, время Epoc, TrueTime и время GPS.