## Señales

Añadamos señales a tu mundo para guiar al jugador en su viaje.

Tu proyecto incluye un objeto `señal`:

![captura de pantalla](images/world-sign.png)

--- task ---

El objeto `signo de bienvenida` sólo debe ser visible en la sala 1, así que añade un poco de código al objeto para asegurarte de que ocurre:

--- hints ---


--- hint ---

`Cuando se hace clic en la bandera`{:class="block3events"}, en un bucle `para siempre`{:class="block3control"}, marca `si`{:class="block3control"} la `habitación es 1`{:class="block3variables"} y en ese caso `muestra`{:class="block3looks"} el objeto `signo de bienvenida`, `en otro caso`{:class="block3control"} `ocultar`{:class="block3looks"} el objeto.

--- /hint ---

--- hint ---

Aquí están los bloques que necesitas:

![señal](images/sign.png)

```blocks3
<br />si < > entonces
en otro caso
fin

< (habitación :: variables) = [1] >

ocultar

mostrar

para siempre
fin

cuando se hace clic en la bandera

```

--- /hint ---

--- hint ---

Aquí está el programa completo:

![señal](images/sign.png)

```blocks3
al hacer click en la bandera
para siempre
    si < (habitación :: variables) = [1] > entonces
        mostrar
    en otro caso
        ocultar
    fin
fin
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Prueba el código para tu objeto `señal de bienvenida` moviendo entre las habitaciones. Tu señal solo debe ser visible en la habitación 1.

![captura de pantalla](images/world-sign-test.png)

--- /task ---

--- task ---

¡Una señal no es muy útil si no dice nada! Añade un poco más de código para mostrar un mensaje si el objeto `señal` es tocado por el objeto `jugador`:

![señal](images/sign.png)

```blocks3
al hacer click en la bandera
para siempre
 si < (habitación :: variables) = [1] > entonces
 mostrar
 en otro caso
 ocultar
 fin
+ si < tocando al (jugador v)? > entonces
decir [¡Bienvenido! ¿Puedes llegar al tesoro?]
más
decir []
fin
fin
```

--- /task ---

--- task ---

Prueba tu objeto `símbolo de bienvenida` de nuevo. Ahora deberías ver un mensaje cuando el objeto `jugador` toca el objeto `señal`.

![captura de pantalla](images/world-sign-test2.png)

--- /task ---