## Збирання монет

Твій спрайт `гравець` повинен мати можливість збирати монети, коли він рухається по світу.

--- task ---

Додай у свій проєкт нову змінну з назвою `монети`{:class="block3variables"}.

--- /task ---

--- task ---

Вибери спрайт `монета` і клацни **показати**.

![знімок екрана](images/coin.png)

--- /task ---

--- task ---

Додай код до спрайта `монета` так, щоб він з’являвся лише в кімнаті 1.

![знімок екрана](images/coin.png)

```blocks3
when flag clicked
forever
if <(кімната :: variables)=[1]> then
show
else
hide
```

--- /task ---

--- task ---

Додай код до свого спрайта `монета`, щоб, коли спрайт `гравець` торкався його, щоб «підібрати», той `сховався`{:class="block3looks"}, і до змінної `монети`{:class="block3variables"} додавалось `1`{:class="block3variables"}.

![монета](images/coin.png)

```blocks3
when flag clicked
wait until <touching (гравець v)?>
change [монети v] by (1)
hide
stop [other scripts in sprite v]
```

Код `зупинити інші скрипти цього спрайту`{:class="block3control"} потрібен, щоб спрайт `монета` перестав відображатися в кімнаті 1, коли його підібрали.

--- /task ---

--- task ---

Тепер додай код до Сцени, щоб надати змінній `монети`{:class="block3variables"} значення `0`{:class="block3variables"} на початку гри.

![сцена](images/stage.png)

```blocks3
when flag clicked
set [монети v] to [0]
```

--- /task ---

--- task ---

Протестуй свою гру. Підбирання монети має збільшити кількість `монет` до `1`{:class="block3variables"}.

--- /task ---