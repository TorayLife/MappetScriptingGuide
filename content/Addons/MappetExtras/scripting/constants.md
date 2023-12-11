---
title: Константы
weight: -80
---

<p align="right">Автор: llama_orp</p>

В MappetExtras вы можете использовать константы! Константы - это неизменные значения, которые в нашем случае будут содержать полезную информацию для методов.

# ***Первый пример:***
```js
function main(c){
    c.player.swingArm(0); // MAIN
    c.player.swingArm(1); // OFF
}
```
Здесь в комментариях приходится пояснять числовые значения.

## Лучше так:
```js
function main(c) {
    const constants = mappet.getConstants();

    c.player.swingArm(constants.MAIN); 
    c.player.swingArm(constants.OFF);
}
```

Теперь мы вызываем именованные константы вместо "магических" чисел. Это позволяет:
* Избавиться от лишних комментариев
* Повысить читабельность кода
* Не запоминать числовые значения

# ***Второй пример:***
```js
function main(c) {
    c.player.setSetting(mappet.getConstants().ATTACK, 0);
}
```
Здесь константа ATTACK возвращает строку "keyBindAttack", которую мы передаем в метод.

Таким образом, константы упрощают работу с методами и делают код более понятным.