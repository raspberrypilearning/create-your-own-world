## Recoger monedas

Tu ` jugador ` Sprite debería haber podido recoger monedas a medida que se mueve por el mundo.

Añade una nueva variable a tu proyecto y llámala `Monedas`{:class="block3variables"}. \--- /task \---

\--- Haz clic derecho en el objeto `moneda` y elige **mostrar**.

![captura de pantalla](images/coin.png) \--- /task \---

\--- Añade código al objeto `moneda` de manera que solamente aparezca en la habitación 1. ![captura de pantalla](images/coin.png)

```blocks3
cuando se hace click sobre la bandera
para siempre
si <(habitación :: variables)=[1]> entonces
mostrar
más
ocultar
```

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \--- Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \--- Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}. \--- /task \---