## Personen

Lass uns ein paar Personen in deine Welt setzen, mit denen dein `Spieler` in interagieren kann.

\--- task \---

Switch to the `person` sprite.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

Add some code to the `person` sprite so that the person talks to the `player` sprite. This code is very similar to the code you added to your `sign` sprite:

![person](images/person.png)

```blocks3
Wenn die grüne Flagge angeklickt
gehe zu x: (0) y: (-150)
wiederhole fortlaufend 
  falls <wird (Spieler v) berührt?> , dann      sage [Wusstest du schon, dass du durch orangene und gelbe Türen gehen kannst?]
  sonst 
    sage []
  end
end
```

\--- /task \---

\--- task \---

Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

```blocks3
Wenn die grüne Flagge angeklickt
gehe zu x: (0) y: (-150)
wiederhole fortlaufend 
  falls <wird (Spieler v) berührt?> , dann      sage [Wusstest du schon, dass du durch orangene und gelbe Türen gehen kannst?]
  sonst 
    sage []
    + gehe (1) er Schritt
    + pralle vom Rand ab
  end
end
```

\--- /task \---

Your `person` sprite will now move, but will stop to talk to the `player` sprite.

![screenshot](images/world-person-test.png)

\--- task \---

Add code to your new `person` sprite so that the sprite only appears in room 1. The code you need is exactly the same as the code that makes the `sign` sprite only visible in room 1.

Make sure you test out your new code.

\--- /task \---