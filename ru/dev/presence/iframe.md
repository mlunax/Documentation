---
title: Класс iFrame
description:
published: true
date: 2020-05-03T20:17:51.982Z
tags:
---

# класс iFrame
> iframe система с PreMiD проблематична и может иметь неожиданное поведение, использовать с осторожностью. 
> 
> {.is-danger}

## Введение

В некоторых сценариях вашему присутствию может потребоваться доступ к элементам внутри `iframes`.

Код, который вы пишете внутри файла `iframe.ts` , вводится в каждый iframe на странице.

Как и присутствия, `iframes` имеют свои собственные классы, предназначенные для автоматического обновления данных.

```typescript
let iframe = new iFrame();

iframe.on("UpdateData", async () => {
    // Код идет здесь...
});
```

## Методы

### `send(Object)`
Отправляет данные в присутствие. С помощью этого метода можно сделать наличие `iFrameData`.

### `getUrl()`
Возвращает URL `iframe`.

## Событие
В `iframes`события работают аналогично тому, как они работают в классе `присутствия`.

```typescript
iframe.on("UpdateData", async () => {
    // Код идет здесь...
});
```

Список всех событий:

#### `UpdateData`

Это событие запускается каждый раз, когда iframe обновляется.