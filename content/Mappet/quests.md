---
title: Квесты
weight: -80
---

<p align="right">Автор: llama_orp</p>

# Создание Квестов в Mappet

## Вход в меню квестов
Чтобы зайти в меню квестов Mappet, нажмите клавишу `=`. В левой части экрана нажмите на иконку восклицательного знака.

## Создание нового квеста
Чтобы создать новый квест, нажмите на кнопку со знаком плюс (`+`). Дайте квесту подходящее название.

Название квеста отвечает за его название, которое будет показано:
* При его диалоге
* Справа сверху при принятии квеста
* В журнале квестов

В поле описания желательно подробно описать суть задания.

Описание видно только:
* В диалоге
* В журнале квестов

Кнопка "отменяемый" - если данная функция включена, то в журнале квестов, вы сможете удалить этот квест.

Кнопка "мгновенный" - если включён, то сразу выполняется квест, как только вы выполните все поставленные цели.

Если выключен, то нужно идти к НПС у которого вы брали этот квест, дабы завершить его

## Цели.

Категория "Цели" даёт задание игроку которую они должны выполнить. Есть четыре вида цели:
* Цель убийства
    * Даёт игроку задание, убить какую-либо сущность. В данной цели можно выбрать айди самой сущности, а так же количество убийц.
    * "Соответсвующий NBT" - позволяет настроить более тонкую настройку жертвы при убийстве, чтобы к примеру убивать не всех криперов, а с каким-то именем
    * "Сообщение пользовательской цели" - это краткое описание квеста, а так же его подсчёт. Если мы что-то впишем сюда. то данный текст будет написан везде:
        * При диалоге
        * При принятом квесте
        * В журнале квестов
* Цель сбора
    * Данная цель даёт игроку цель собрать определённое количество предметов.
    * "Сообщение пользовательской цели" - имеет ту же функцию, что и в других целях.
    * Белый квадратик: нам откроется наш инвентарь, где мы должны выбрать нужный предмет для сбора. 
* Цель состояние
    * Мы можем использовать редактирование состояний.
* Цель прочтения диалога
    * В данной цели можно настроить диалог с каким-либо персонажем. В редактировании условий уже будет одно условие "прочитан". В данном окне мы можем выбрать сам айди диалога, а так же маркер нужной фразы. Так же можно настроит цель которой нужно будет выполнить этот квест.

## Награды

Позволяет назначить награду в качестве предмета за удачное окончание квеста.

## Триггеры

### Принять квестовый триггер
Запускает установленный к нему триггер после принятия квеста в диалоге.

### Отклонить квестовый триггер
Запускает установленный к нему триггер после отклонения квеста в диалоге.

### Завершить квестовый триггер
Запускает установленный к нему триггер после завершения квеста.