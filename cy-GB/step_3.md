## Waliau cadarn

\--- task \--- Profa dy `chwaraewr` eto. A weli di ei fod yn gallu cerdded trwy'r waliau llwyd golau.

![sgrinlun](images/world-walls.png) \--- /task \---

\--- task \--- I ddatrys hyn, bydd angen i ti wneud i'r `chwaraewr` symud yn ôl os yw'n cyffwrdd wal llwyd. Dyma'r côd sydd angen ei osod o fewn y bloc `am byth` {:class="block3control"} o dan y blociau cyfeiriad:

![chwaraewr](images/player.png)

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
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
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

Ceisia wneud i'r `chwaraewr` symud trwy wal. Os yw'r côd newydd yn gweithio, ni ddylai hyn fod yn bosib.

![sgrinlun](images/world-walls-test.png) \--- /task \---