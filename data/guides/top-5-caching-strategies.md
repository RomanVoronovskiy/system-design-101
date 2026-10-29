---
title: "Пять стратегий кеширования"
description: "Стратегии синхронизации данных между кешем и базой данных."
image: "https://assets.bytebytego.com/diagrams/0374-top-5-caching-strategies.png"
createdAt: "2024-02-22"
draft: false
categories:
  - caching-performance
tags:
  - "Caching"
  - "Data Synchronization"
---

![](https://assets.bytebytego.com/diagrams/0374-top-5-caching-strategies.png)

После добавления кеша в архитектуру неизбежно возникает задача его синхронизации с базой данных.

Рассмотрим пять распространённых стратегий поддержания согласованности данных.

## Стратегии чтения

* Загрузка в кеш по запросу — Cache Aside
* Сквозное чтение — Read-Through

## Стратегии записи

* Запись в обход кеша — Write-Around
* Отложенная запись — Write-Back
* Сквозная запись — Write-Through

Эти стратегии часто комбинируют. Например, Write-Around нередко используют вместе с Cache Aside, чтобы поддерживать актуальность кеша.
