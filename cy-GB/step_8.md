## Pobl

Fe awn ati i ychwanegu pobl arall i dy fyd mae modd i dy `chwaraewr` ryngweithio â nhw.

\--- task \---

Switch to the `person` sprite.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

Add some code to the `person` sprite so that the person talks to the `player` sprite. This code is very similar to the code you added to your `sign` sprite:

![person](images/person.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
mynd i x: (0) y: (-150)
am byth 
  os <cyffwrdd (player v) ? > yna 
    dweud [Oeddet ti'n gwybod dy fod di'n gallu mynd trwy drysau oren a melyn?]
  fel arall 
    dweud []
  end
end
```

\--- /task \---

\--- task \---

Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
mynd i x: (0) y: (-150)
am byth 
  os <cyffwrdd (player v) ? > yna 
    dweud [Oeddet ti'n gwybod dy fod di'n gallu mynd trwy drysau oren a melyn?]
  fel arall 
    dweud []
    + symud (1) cam
    + os ar ymyl, bowndio
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