## Postacie

Add other people to your world who your `player` sprite can interact with.

\--- task \--- Switch to the `person` sprite.

![duszek postać](images/person.png) \--- /task \---

\--- task \--- Add some code to the `person` sprite so that the person talks to the `player` sprite. Ten kod jest bardzo podobny do kodu dodanego do duszka `znak`:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
    end
end
```

\--- /task \---

\--- task \--- Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
+       move (1) steps
+       if on edge, bounce
    end
end

```

\--- /task \---

Twój duszek `postać` będzie się teraz poruszać, ale zatrzyma się aby porozmawiać z duszkiem `gracz`.

![zrzut ekranu](images/world-person-test.png)

\--- task \--- Add code to your new `person` sprite so that the sprite only appears in room 1. The code you need is exactly the same as the code that makes the `sign` sprite only visible in room 1.

Pamiętaj o przetestowaniu swojego nowego kodu. \--- /task \---