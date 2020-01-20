## Munten verzamelen

Je `speler` sprite zou in staat moeten zijn munten te verzamelen terwijl deze door de wereld beweegt.

\--- task \---

Add a new variable valled `coins`{:class="block3variables"} to your project.

\--- /task \---

\--- task \---

Select the `coin` sprite and click **show**.

![screenshot](images/coin.png)

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that it only appears in room 1.

![screenshot](images/coin.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal
als <(kamer :: variables)=[1]> dan
verschijn
anders
verdwijn
```

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
wanneer groene vlag wordt aangeklikt
wacht tot < raak ik (speler v)?>
verander [munten v] met (1)
verdwijn
stop [andere scripts in sprite v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \---

Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
wanneer groene vlag wordt aangeklikt
maak [munten v] [0]
```

\--- /task \---

\--- task \---

Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.

\--- /task \---