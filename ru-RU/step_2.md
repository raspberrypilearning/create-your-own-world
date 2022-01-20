## Перемещение спрайта игрока

Начни с создания спрайта `игрока`, способного двигаться по всему миру.

--- task ---

Открой начальный проект Scratch под названием "Создай свой собственный мир".

**Онлайн**: открой стартовый проект по адресу [scratch.mit.edu/projects/396456937](https://scratch.mit.edu/projects/396456937){:target="_blank"}.

Если у тебя есть учетная запись в Scratch, то ты можешь сделать копию проекта, нажав **Ремикс**.

**Оффлайн**: скачай стартовый проект с [rpf.io/p/ru-RU/create-your-own-world-go](https://rpf.io/p/ru-RU/create-your-own-world-go){:target="_blank"} и затем открой его с помощью оффлайн редактора. Если тебе нужно скачать и установить оффлайн редактор Скретч, ты можешь найти его по адресу [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![снимок экрана](images/world-starter.png)

--- /task ---

Нажатие клавиш со стрелками должно перемещать спрайт `игрока` в пределах мира. При нажатии стрелки вверх спрайт `игрок` должен двигаться вверх на Сцене.

--- task ---

Добавь этот код в спрайт `игрока`:

![игрок](images/player.png)

```blocks3
when flag clicked
forever
	if <key (стрелка вверх v) pressed? > then
		point in direction (0)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Нажми на флажок и удерживай клавишу вверх. Двигается ли спрайт `игрока` вверх?

![снимок экрана](images/world-up.png)

--- /task ---

--- task ---

Чтобы переместить спрайт `игрока` влево, тебе нужно добавить другой блок `если`{:class="block3control"} с похожим кодом:

![игрок](images/player.png)

```blocks3
when flag clicked
forever
	if <key (стрелка вверх v) pressed? > then
		point in direction (0)
		move (4) steps
	end
+	if <key (стрелка влево v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Добавьте ещё код к спрайту `игрока`, чтобы он мог двигаться вниз и вправо. Код, который у тебя уже есть, должен тебе помочь в этом.

--- hints ---


--- hint ---

Для того, чтобы двигаться вверх, ты двигаешь спрайт `игрока` в направлении `0` градусов. Что нужно сделать, чтобы переместить спрайт вниз?

Чтобы двигаться влево, ты двигаешь спрайт в направлении `-90` градусов. Что нужно сделать, чтобы переместить спрайт вправо?

--- /hint ---

--- hint ---

Тебе нужно изменить эти два блока:

![игрок](images/player.png)

```blocks3
<клавиша ( v) нажата?>

повернуться в направлении ()
```

Скопируй код, который заставляет спрайт `игрока` двигаться вверх и измени эти два блока, чтобы заставить спрайт двигаться вниз. Снова скопируй код и измени его так, чтобы спрайт переместился вправо.

--- /hint ---

--- hint ---

Вот как должен выглядеть твой код:

![игрок](images/player.png)

```blocks3
when flag clicked
forever
	if <key (стрелка вверх v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (стрелка влево v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
+    if <key (стрелка вниз v) pressed? > then
		point in direction (180)
		move (4) steps
	end
+    if <key (стрелка вправо v) pressed? > then
		point in direction (90)
		move (4) steps
	end
end
```

--- /hint ---

--- /hints ---

--- /task ---
