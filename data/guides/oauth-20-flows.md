---
title: "Сценарии авторизации OAuth 2.0"
description: "Сценарии OAuth 2.0: Authorization Code, Client Credentials, Implicit и Password Grant."
image: "https://assets.bytebytego.com/diagrams/0112-oauth-flows.png"
createdAt: "2024-03-10"
draft: false
categories:
  - security
tags:
  - "OAuth 2.0"
  - "Authorization"
---

![](https://assets.bytebytego.com/diagrams/0112-oauth-flows.png)

## Поток с кодом авторизации — Authorization Code Flow

Самый распространённый сценарий OAuth. После аутентификации пользователя клиент получает код авторизации и обменивает его на токен доступа и токен обновления.

## Поток с учётными данными клиента — Client Credentials Flow

Конфиденциальный клиент получает токен доступа, аутентифицируясь с помощью собственных учётных данных. Он действует от своего имени, без отдельного запроса авторизации пользователя.

Примечание русской редакции: в оригинале в этом разделе ошибочно повторено описание Implicit Flow. Здесь оно исправлено в соответствии с [RFC 6749, раздел 4.4](https://datatracker.ietf.org/doc/html/rfc6749#section-4.4).

## Неявный поток — Implicit Flow

Предназначен для одностраничных приложений. Токен доступа возвращается непосредственно клиенту, без промежуточного кода авторизации.

## Поток с паролем владельца ресурса — Resource Owner Password Grant

Пользователь передаёт имя и пароль непосредственно клиенту, который обменивает их на токен доступа.
