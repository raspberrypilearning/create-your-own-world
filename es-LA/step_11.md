## Puertas y llaves

Ahora vas a añadir código para que algunas de las puertas del mundo de tu juego estén bloqueadas, y el jugador debe encontrar la llave para abrirlas y llegar a la habitación siguiente.

--- task ---

Cambia al objeto `llave`. Haz clic en `mostrar`{:class="blocklooks"} en el menú Scripts para que el objeto aparezca en el Escenario.

--- /task ---

--- task ---

Edita el disfraz del objeto `llave` para que sea de color azul.

--- /task ---

--- task ---

¡Cambia al fondo de escenario a la habitación 3 y coloca el objeto `llave` en un lugar que sea difícil de alcanzar!

![captura de pantalla](images/world-key.png)

--- /task ---

--- task ---

Añade código al objeto `moneda` de manera que solamente aparezca en la habitación 3.

--- /task ---

--- task ---

Crea una nueva lista llamada `inventario`{:class="block3variables"} para almacenar los elementos que el objeto `jugador` recolecta.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

El código que necesitas agregar para recoger la llave es muy similar al código para recoger monedas. La diferencia es que se añade la llave al `inventario`{:class="block3variables"}.

![llave](images/key.png)

```blocks3
when flag clicked
wait until <touching (jugador v)?>
add [llave azul] to [inventario v]
hide
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

Agrega código a tu escenario para vaciar tu inventario al comienzo del juego.

```blocks3
delete all of [inventario v]
```

--- /task ---

--- task ---

Prueba tu juego para comprobar si puedes recoger el objeto `llave` y añadirlo a tu inventario.

--- /task ---

--- task ---

Ahora agrega la puerta cerrada. Seleccione el objeto `puerta azul` y haz clic en `mostrar`{:class="blocklooks} en el menú Scripts, y luego coloca el objeto en el espacio entre las dos paredes.

![captura de pantalla](images/world-door.png)

--- /task ---

--- task ---

Añade código al objeto `puerta azul` de manera que solamente aparezca en la habitación 3.

--- /task ---

--- task ---

Añade código al objeto `puerta azul` para que, cuando la llave esté en el `inventario`{:class="block3variables"}, el objeto se `esconda`{:class="block3looks"} para permitir que pase el objeto `jugador`.

![puerta](images/door.png)

```blocks3
when flag clicked
wait until <[inventario v] contains [llave azul]?>
stop [other scripts in sprite v]
hide
```

--- /task ---

--- task ---

¡Prueba tu juego y comprueba si puedes recoger la llave azul para abrir la puerta!

--- /task ---