## Сбор монет

Твой спрайт `игрок` должен иметь возможность собирать монеты, когда он путешествует по миру.

\--- task \---

Добавь новую переменную `монеты`{:class="block3variables"} в свой проект.

\--- /task \---

\--- task \---

Выбери спрайт `монета` и нажми **показать**.

![снимок экрана](images/coin.png)

\--- /task \---

\--- task \---

Добавь код к своему спрайту `монета` так, чтобы спрайт появлялся только в комнате 1.

![снимок экрана](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

Добавь код к спрайту `монета` так, чтобы спрайт `прятался`{:class="block3looks"} и переменная `монеты`{:class="block3variables"}увеличивалась на `1`{:class="block3variables"} как только спрайт `игрок` коснётся спрайта `монета`, чтобы «собрать её».

![монета](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \---

Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.

\--- /task \---