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

Agregue código al objeto `moneda ` para que el sprite ` se esconda ` {: class = "block3looks"} y se sume` 1 ` {: class = "block3variables"} a la variable` monedas ` {: class = "block3variables"} cada vez que el objeto` jugador ` toque el objeto ` moneda` para 'recogerlo'.

![moneda](images/coin.png)

```blocks3
al presionar bandera verde
esperar hasta que <touching (player v)?>
cambiar [Monedas v] por (1)
esconder
detener [otros programas en el objeto v]
```

El código `detener otros programas en el objeto`{:class="block3control"} es necesario para que el objeto `moneda` deje de mostrarse en la habitación 1 una vez que haya sido recogido.

\--- /task \---

\--- tarea \--- Ahora agregue código al escenario para establecer su variable ` monedas ` {: class = "block3variables"} a ` 0 ` {: class = "block3variables"} al comienzo del juego.

![escenario](images/stage.png)

```blocks3
al hacer clic en la bandera
dar a [monedas v] el valor [0]
```

\--- /task \---

\--- task \--- Prueba tu código. Recolectar una moneda debe cambiar tu puntuación de `monedas` a `1`{:class="block3variables"}. \--- /task \---