---
title: "Как работают Apple Pay и Google Pay?"
description: "Изучите механизмы Apple Pay и Google Pay для обеспечения безопасных транзакций."
image: "https://assets.bytebytego.com/diagrams/0002-apple-pay.jpg"
createdAt: "2024-03-12"
draft: false
categories:
  - payment-and-fintech
tags:
  - "Payment Systems"
  - "Mobile Payments"
---

![](https://assets.bytebytego.com/diagrams/0002-apple-pay.jpg)

На диаграмме выше показаны различия. Оба подхода очень безопасны, но реализации разные. Чтобы понять разницу, мы разобьем процесс на два потока.

## Регистрация потока вашей кредитной карты

## Основной поток платежей

1. Процесс регистрации в обоих случаях представлен шагами 1–3. Разница в следующем:

* **Apple Pay:** Apple не хранит данные карты. Он передает данные карты в банк. Банк возвращает на iPhone токен под названием DAN (номер учетной записи устройства). Затем iPhone сохраняет DAN в специальный аппаратный чип.

* **Google Pay.** Когда вы регистрируете кредитную карту в Google Pay, данные карты сохраняются на сервере Google. Google возвращает на телефон платежный токен.

2. Когда вы нажимаете кнопку «Оплатить» на своем телефоне, запускается основной процесс оплаты. Вот различия:

* **Apple Pay:** для iPhone сервер электронной коммерции передает DAN в банк.

* **Google Pay.** В случае Google Pay сервер электронной коммерции передает платежный токен на сервер Google. Сервер Google ищет информацию о кредитной карте и передает ее в банк.

На схеме красная стрелка означает, что информация о кредитной карте доступна в общедоступной сети, хотя и зашифрована.

Ссылки:

[1] [Обзор безопасности и конфиденциальности Apple Pay](https://support.apple.com/en-us/101554)

[2] [Google Pay для платежей](https://developers.google.com/pay/api/android/overview)

[3] [Apple Pay против Google Pay: как они работают](https://www.investopedia.com/articles/personal-finance/010215/apple-pay-vs-google-wallet-how-they-work.asp)