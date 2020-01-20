## Personas

Añade otras personas a tu mundo con las que tu objeto `jugador` puede interactuar.

\--- task \---

Switch to the `person` sprite.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

Add some code to the `person` sprite so that the person talks to the `player` sprite. This code is very similar to the code you added to your `sign` sprite:

![persona](images/person.png)

```blocks3
al presionar la bandera verde
ir a x: (0) y: (-150)
por siempre 
  si <¿tocando (jugador v)? > entonces 
    decir [¿Sabías que puedes atravesar las puertas naranjas y amarillas?]
  en otro caso
    decir []
  end
end
```

\--- /task \---

\--- task \---

Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

```blocks3
al presionar la bandera verde
ir a x: (0) y: (-150)
por siempre 
  si <¿tocando (jugador v)? > entonces 
    decir [¿Sabías que puedes atravesar las puertas naranjas y amarillas?]
  en otro caso
    decir []
+       mover  (1) paso
+       si está en el borde, rebotar
  fin
fin
```

\--- /task \---

Your `person` sprite will now move, but will stop to talk to the `player` sprite.

![screenshot](images/world-person-test.png)

\--- task \---

Add code to your new `person` sprite so that the sprite only appears in room 1. The code you need is exactly the same as the code that makes the `sign` sprite only visible in room 1.

Make sure you test out your new code.

\--- /task \---