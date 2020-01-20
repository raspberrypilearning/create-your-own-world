## Zbierať mince

Váš `hráč` by mal byť schopný zbierať mince pri pohybe po celom svete.

\--- task \---

Add a new variable valled `coins`{:class="block3variables"} to your project.

\--- / úloha \---

\--- task \---

Select the `coin` sprite and click **show**.

![screenshot](images/coin.png)

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that it only appears in room 1.

![screenshot](images/coin.png)

```blocks3
keď vlajka klikne
navždy
ak <(miestnosť :: premenné) =[1]> potom
zobraziť
iný
skryť
```

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
keď vlajka klikne
počká, až <touching (player v)?>
zmení [mince v] podľa (1)
skryť
stop [iné skripty v sprite v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \---

Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
keď príznakom kliknete na
nastavíte [mince v] na hodnotu [0]
```

\--- /task \---

\--- task \---

Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.

\--- /task \---