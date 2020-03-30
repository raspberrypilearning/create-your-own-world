## Таблички

Теперь добавь таблички в свой мир, которые бы помогали игрокам во время их путешествий.

Твой проект включает в себя спрайт `табличка Добро пожаловать`:

![снимок экрана](images/world-sign.png)

\--- task \---

Спрайт `табличка Добро пожаловать` должен быть виден только в комнате 1, поэтому добавьте код к спрайту, чтобы убедиться, что это происходит:

\--- hints \---

\--- hint \---

`Когда зеленый флаг нажат`{:class="block3events"}, в цикле `повторять всегда`{:class="block3control"} проверь, `если`{:class="block3control"} `комната номер 1`{:class="block3variables"}, и в этом случае `покажи`{:class="block3looks"} спрайт `табличка Добро пожаловать`, `иначе`{:class="block3control"} `спрячь`{:class="block3looks"} спрайт.

\--- /hint \---

\--- hint \---

Here are the blocks you need:

![sign](images/sign.png)

```blocks3
<br />if < > then
else
end

< (room :: variables) = [1] >

hide

show

forever
end

when flag clicked

```

\--- /hint \---

\--- hint \---

Here is the complete code:

![sign](images/sign.png)

```blocks3
when flag clicked
forever
    if < (room :: variables) = [1] > then
        show
    else
        hide
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Test the code for your `welcome sign` sprite by moving between rooms. The sign should only be visible in room 1.

![screenshot](images/world-sign-test.png)

\--- /task \---

\--- task \---

A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

```blocks3
when flag clicked
forever
if < (room :: variables) = [1] > then
show
else
hide
end
+if < touching (player v)? > then
say [Welcome! Can you get to the treasure?]
else
say []
end
end
```

\--- /task \---

\--- task \---

Test your `welcome sign` sprite again. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![screenshot](images/world-sign-test2.png)

\--- /task \---