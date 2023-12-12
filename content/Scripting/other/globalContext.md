---
title: Глобальный контекст
weight: -80
---

<p align="right">Автор: llama_orp</p>

С помощью некоторых манипуляций, вы можете сделать контекст(`c`) - глобальным во всём скрипте.
```js
function main(c) {
    this.c = c
    
    other()
}

function other() {
    c.send("hp: "+c.player.hp)
}
```

Это работает не только с контекстом, но и с другими значениями.

```js
function main(c){
    this.x = 5
    
    other(c)
}

function other(c){
    c.send(x)
}
```