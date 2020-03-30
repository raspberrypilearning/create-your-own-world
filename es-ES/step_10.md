## Recoger monedas

Tu objeto `jugador` deberá ser capaz de recoger monedas a medida que se mueve por el mundo.

--- task ---

Añade una nueva variable a tu proyecto y llámala `monedas`{:class="block3variables"}.

--- /task ---

--- task ---

Haz clic derecho en el objeto `moneda` y elige **mostrar**.

![captura de pantalla](images/coin.png)

--- /task ---

--- task ---

Añade código al objeto `moneda` de manera que solamente aparezca en la habitación 1.

![screenshot](images/coin.png)

```blocks3
when flag clicked
forever
if <(habitación :: variables)=[1]> then
show
else
hide
```

--- /task ---

--- task ---

Agregue código al objeto `moneda` para que `desaparezca`{:class="block3looks"} y se sume `1`{:class="block3variables"} a la variable `monedas`{:class="block3variables"} cada vez que el objeto `jugador` toque el objeto `moneda` para 'recogerlo'.

![moneda](images/coin.png)

```blocks3
when flag clicked
wait until <touching (jugador v)?>
change [monedas v] by (1)
hide
stop [otros programas en el objeto v]
```

El código `detener otros programas en el objeto`{:class="block3control"} es necesario para que el objeto `moneda` deje de mostrarse en la habitación 1 una vez que haya sido recogido.

--- /task ---

--- task ---

Ahora agregue código al escenario para establecer su variable `monedas`{:class="block3variables"} a `0`{:class="block3variables"} al comienzo del juego.

![escenario](images/stage.png)

```blocks3
when flag clicked
dar a [monedas v] el valor [0]
```

--- /task ---

--- task ---

Prueba tu juego. Recolectar una moneda debe cambiar tu puntuación de `monedas` a `1`{:class="block3variables"}.

--- /task ---