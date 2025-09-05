## Waliau cadarn

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls?

![sgrinlun](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Dyma'r côd sydd angen ei osod o fewn y bloc `am byth` {:class="block3control"} o dan y blociau cyfeiriad:

![chwaraewr](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
  os <bysell (up arrow v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (0)
    symud (4) cam
  end
  os <bysell (left arrow v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (-90)
    symud (4) cam
  end
  os <bysell (down arrow v) wedi ei phwyso? > then
        point in direction (180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > yna 
    pwyntio i gyfeiriad (90)
    symud (4) cam
  end
  + os <cyffwrdd lliw [#BABABA] ? > yna 
  +   symud (-4) cam
  + end
end
```

\--- /task \---

\--- task \---

Ceisia wneud i'r `chwaraewr` symud trwy wal. Os yw'r côd newydd yn gweithio, ni ddylai hyn fod yn bosib.

![sgrinlun](images/world-walls-test.png)

\--- /task \---