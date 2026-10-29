---
title: "URL, URI и URN: в чём различия"
description: "Различия между URL, URI и URN с понятными примерами."
image: 'https://assets.bytebytego.com/diagrams/0401-url-uri-urn.png'
createdAt: '2024-02-21'
draft: false
categories:
  - api-web-development
tags:
  - Networking
  - Web
---

![](https://assets.bytebytego.com/diagrams/0401-url-uri-urn.png)

Схема выше сравнивает URL, URI и URN.

* **URI**

  URI означает Uniform Resource Identifier — унифицированный идентификатор ресурса. Он идентифицирует логический или физический ресурс в сети. URL и URN — разновидности URI: URL указывает расположение ресурса, а URN задаёт его имя.

URI состоит из следующих частей:

```
scheme:[//authority]path[?query][#fragment]
```

* **URL**

  URL означает Uniform Resource Locator — унифицированный указатель ресурса. Это одно из ключевых понятий HTTP: адрес уникального ресурса в сети. URL применяются и с другими протоколами, например FTP и JDBC.

* **URN**

  URN означает Uniform Resource Name — унифицированное имя ресурса. Он использует схему urn и не предназначен для определения расположения ресурса. Простой пример на схеме состоит из пространства имён и строки, определяемой этим пространством.
