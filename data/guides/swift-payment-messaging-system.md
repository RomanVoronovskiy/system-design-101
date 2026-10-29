---
title: "Система обмена платёжными сообщениями SWIFT"
description: "SWIFT: безопасный обмен банковскими сообщениями и трансграничные платежи."
image: "https://assets.bytebytego.com/diagrams/0348-swift-payment-messaging-system.png"
createdAt: "2024-02-28"
draft: false
categories:
  - payment-and-fintech
tags:
  - "Payments"
  - "Finance"
---

![](https://assets.bytebytego.com/diagrams/0348-swift-payment-messaging-system.png)

Вы наверняка слышали о SWIFT. Что это за система и какую роль она играет в международных платежах?

Society for Worldwide Interbank Financial Telecommunication (SWIFT) — защищённая **система обмена сообщениями**, связывающая банки по всему миру.

Система находится в Бельгии, управляется банками-участниками и ежедневно обрабатывает миллионы платёжных сообщений. На схеме показан путь сообщения от банка A в Нью-Йорке к банку B в Лондоне.

## Путь сообщения SWIFT

**Шаг 1:** банк A отправляет сведения о переводе региональному обработчику Regional Processor A в Нью-Йорке. Получатель — банк B.

**Шаг 2:** региональный обработчик проверяет формат и передаёт сообщение в Slice Processor A. Regional Processor отвечает за проверку входящих сообщений и очередь исходящих, а Slice Processor — за безопасное хранение и маршрутизацию.

**Шаг 3:** Slice Processor A сохраняет сообщение.

**Шаг 4:** он сообщает Regional Processor A, что сообщение сохранено.

**Шаг 5:** Regional Processor A отправляет банку A подтверждение ACK или отказ NAK. ACK означает, что сообщение будет отправлено банку B; NAK — что оно не будет отправлено.

**Шаг 6:** Slice Processor A передаёт сообщение Regional Processor B в Лондоне.

**Шаг 7:** Regional Processor B временно сохраняет сообщение.

**Шаг 8:** он назначает сообщению уникальный идентификатор MON (Message Output Number) и передаёт его в Slice Processor B.

**Шаг 9:** Slice Processor B проверяет MON.

**Шаг 10:** Slice Processor B разрешает Regional Processor B отправить сообщение банку B.

**Шаг 11:** Regional Processor B отправляет сообщение банку B.

**Шаг 12:** банк B получает и сохраняет сообщение.

**Шаг 13:** банк B отправляет Regional Processor B ответ UAK или UNK. UAK (User Positive Acknowledgment) подтверждает получение без ошибок, а UNK (User Negative Acknowledgment) означает ошибку контрольной суммы.

**Шаг 14:** Regional Processor B создаёт отчёт по ответу банка B и передаёт его в Slice Processor B.

**Шаг 15:** Slice Processor B сохраняет отчёт.

**Шаги 16 и 17:** Slice Processor B отправляет копию отчёта в Slice Processor A, который сохраняет её.
