## Muévete por tu mundo

El objeto `jugador` debe ser capaz de entrar en otras habitaciones por las puertas.

Tu proyecto contiene fondos para otras habitaciones:

![captura de pantalla](images/world-backdrops.png)

\--- task \---

Crea una nueva variable"para todos los objetos" y llámala `habitación`{:class="block3variables"} para poder ver en que habitación se encuentra el `jugador`.

[[[generic-scratch3-add-variable]]]

![captura de pantalla](images/world-room.png)

\--- /task \---

\--- task \---

Cuando el objeto `jugador` toca la puerta naranja en la primera habitación, se debe mostrar el fondo siguiente y el objeto `jugador` tiene que volver al lado izquierdo del escenario. Añade este código dentro del bucle `por siempre`{:class="block3control"} del `jugador`:

![jugador](images/player.png)

```blocks3
al hacer clic en la bandera verde
por siempre 
  si <¿tecla (flecha arriba v) presionada? > entonces 
    apuntar en dirección (0)
    mover (4) pasos
  end
  si <¿tecla (flecha izquierda v) está presionada? > entonces 
    apuntar en dirección (-90)
    mover (4) pasos
  end
  si <¿tecla (flecha abajo v) presionada? > then
        point in direction (180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > entonces 
        apuntar en dirección (90)
        mover (4) pasos
    fin
    si < toca el color [#BABABA]? > entonces
    mover (-4) pasos
    fin
    si < toca el color [# F2A24A] > entonces
    cambia el fondo a (siguiente fondo v)
    ve a x: (-200) y: (0)
    cambia [habitación v] por (1)
fin
fin
```

\--- /task \---

\--- task \---

Cada vez que el juego empieza, la sala, la posición del personaje y el fondo necesitan ser reiniciados.

Añade código al **principio** del código del objeto `jugador` encima del bucle `por siempre`{:class="block3control"} para asegurarte que todo se restablece cuando se hace clic en la bandera:

\--- hints \---

\--- hint \---

Cuando el juego inicia:

+ El valor de `habitación`{:class="block3variables"} debe establecerse en `1`{:class="block3variables"}
+ El valor de `telón de fondo`{:class="block3looks"} debe establecerse en `habitación1`{:class="block3looks"}
+ La posición del objeto `jugador` debe establecerse en `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Aquí están los bloques adicionales que necesitas:

![jugador](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

\--- /hint \---

\--- hint \---

Así es como debería verse tu código terminado:

![jugador](images/player.png)

```blocks3
when flag clicked
+set [room v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to (room1 v)
forever
    if <key (up arrow v) pressed? > entonces 
    apuntar en dirección (0)
    mover (4) pasos
  end
  si <¿tecla (flecha izquierda v) está presionada? > entonces 
    apuntar en dirección (-90)
    mover (4) pasos
  end
  si <¿tecla (flecha abajo v) presionada? > then
        point in direction (180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > entonces 
        apuntar en dirección (90)
        mover (4) pasos
    fin
    si < toca el color [#BABABA]? > entonces
    mover (-4) pasos
    fin
    si < toca el color [# F2A24A] > entonces
    cambia el fondo a (siguiente fondo v)
    ve a x: (-200) y: (0)
    cambia [habitación v] por (1)
fin
fin
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Haga clic en la bandera y luego mueve tu objeto `jugador` hasta que toque la puerta naranja. ¿Tu objeto se mueve a la pantalla siguiente? ¿La variable `Habitación`{:class="block3variables"} cambia a `2`?

![captura de pantalla](images/world-room-test.png)

\--- /task \---