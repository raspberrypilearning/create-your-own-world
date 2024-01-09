## Paredes sólidas

\--- task \---

Prueba de nuevo tu objeto `jugador`. ¿Ves que puede atravesar las paredes de color gris claro?

![captura de pantalla](images/world-walls.png)

\--- /task \---

\--- task \---

Para arreglar esto, tendrás que hacer que tu `jugador` retroceda si toca una pared de color gris claro. Este es el código que necesitas añadir dentro de tu bloque `para siempre`{:class="block3control"} debajo de los bloques de dirección:

![jugador](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

\--- /task \---

\--- task \---

Intenta hacer que el objeto `jugador` se mueva a través de una pared. Si tu nuevo código funciona, esto no debería ser posible.

![captura de pantalla](images/world-walls-test.png)

\--- /task \---