## Puertas y llaves

Ahora vas a añadir código para que algunas de las puertas del mundo de tu juego estén bloqueadas, y el jugador debe encontrar la llave para abrirlos y llegar a la habitación siguiente.

\--- Cambia al objeto `llave`. Haz click en `mostrar`{:class="blocklooks"} en el menú Scripts para que el sprite aparezca en el Escenario. \--- /task \---

\--- Edita el disfraz del objeto `llave` para que sea de color azul. \--- /task \---

¡Cambia al fondo de escenario a la habitación 3 y coloca el objeto `llave` en un lugar que sea difícil de alcanzar!

![screenshot](images/world-key.png)

\--- /task \---

\--- Añade código al objeto `moneda` de manera que solamente aparezca en la habitación 3. \--- /task \---

\--- Tarea \--- Crear una nueva lista llamada `inventario`{:class="block3variables"} para almacenar los elementos que el objeto `jugador` recolecta.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- Tarea \--- El código que necesitas agregar para recoger la llave es muy similar al código para recoger monedas. La diferencia es que se añade la llave al `inventario`{:class="block3variables"}.

![llave](images/key.png)

```blocks3
al presionar la bandera verde
esperar hasta que <touching (player v)?>
añade la [llave azul] al [Inventario v]
esconder
detener [otros programas en el objeto v]
```

\--- /task \---

\--- tarea \--- Agrega código a tu escenario para vaciar tu inventario al comienzo del juego.

```blocks3
borrar (todos v) de [Inventario v]
```

\--- /task \---

\--- Tarea \--- Prueba tu juego para comprobar si puedes recoger el objeto `llave ` y añadirlo a tu inventario. \--- /task \---

\--- tarea \--- Ahora agregue la puerta cerrada. Seleccione el objeto ` puerta azul ` y haz clic en ` mostrar ` {: class = "blocklooks} en el menú Scripts, y luego coloca el obketo en el espacio entre las dos paredes.

![captura de pantalla](images/world-door.png) \--- /task \---

\--- Tarea \--- Añadir código al objeto `puerta azul` para que sólo sea visible en la sala 3. \--- /task \---

\--- Tarea \--- Añadir código al objeto `puerta azul` para que, cuando la llave esté en el `inventario`{:class="block3variables"}, el objeto se `esconde`{:class="block3looks"} para permitir que pase el objeto de tu`jugador`.

![puerta](images/door.png)

```blocks3
al presionar la bandera verde
esperar hasta que <[Inventario v] contenga [llave azul]>
detener [otros programas en el objeto v]
esconder
```

\--- /task \---

\--- Tarea \--- ¡Prueba tu juego y comprueba si puedes recoger la llave azul para abrir la puerta! \--- /task \---