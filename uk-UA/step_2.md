## Переміщення спрайта гравця

Почни зі створення спрайта `гравець`, що може рухатися в твоєму світу.

--- task ---

Відкрий початковий проєкт «Створи власний світ».

**Онлайн**: відкрий початковий проєкт на [rpf.io/create-your-own-world-on](https://rpf.io/create-your-own-world-on){:target="_blank"}.

Якщо у тебе є обліковий запис Скретч, ти можеш зробити копію проєкту, натиснувши **Ремікс**.

**Офлайн:** завантаж стартовий проєкт з [rpf.io/p/uk-UA/create-your-own-world-go](https://rpf.io/p/uk-UA/create-your-own-world-go), а потім відкрий його за допомогою офлайн-редактора. Якщо тобі треба завантажити та встановити офлайн-редактор Скретч, ти можеш його знайти на [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![знімок екрана](images/world-starter.png)

--- /task ---

Коли ти натискаєш на клавіші зі стрілками, спрайт `гравець` має переміщуватися. Коли натиснуто клавішу зі стрілкою вгору, спрайт `гравець` у відповідь має переміщуватися вгору по Сцені.

--- task ---

Додай такий код до спрайта `гравець`:

![гравець](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

--- /task ---

--- task ---

Натисни на прапор, а потім затисни клавішу зі стрілкою вгору. Чи рухається `гравець` вгору?

![знімок екрана](images/world-up.png)

--- /task ---

--- task ---

Для переміщення спрайта `гравець` вліво, тобі треба додати ще один блок `якщо`{:class="block3control"} з подібним кодом:

![гравець](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

--- /task ---

--- task ---

Додай такий код до свого спрайта `гравець`, щоб він також міг рухатися вниз та вправо. Використовуй уже наявний код, щоб полегшити собі справу.

--- hints ---

--- hint ---

Щоб перемістити спрайт `гравець` вгору, ти направляв(-ла) його на `0` градусів. Що треба зробити, щоб перемістити його вниз?

Для руху вліво ти направляв(-ла) спрайт в напрямку `-90` градусів. Що тобі треба зробити, щоб направити спрайт вправо?

--- /hint ---

--- hint ---

Тобі треба змінити ці два блоки:

![гравець](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Продублюй код, який змушує спрайт `гравець` рухатися вгору, і зміни ці два блоки, щоб він пішов вниз. Продублюй код знову і зміни його так, щоб спрайт рухався вправо.

--- /hint ---

--- hint ---

Ось як має виглядати твій код:

![гравець](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end

+    if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
+    if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

--- /hint ---

--- /hints ---

--- /task ---