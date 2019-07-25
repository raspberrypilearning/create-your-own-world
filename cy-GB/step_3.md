## Waliau cadarn

--- task --- Profa dy `chwaraewr` eto. A weli di ei fod yn gallu cerdded trwy'r waliau llwyd golau.

![sgrinlun](images/world-walls.png) --- /task ---

--- task --- I ddatrys hyn, bydd angen i ti wneud i'r `chwaraewr` symud yn ôl os yw'n cyffwrdd wal llwyd. Dyma'r côd sydd angen ei osod o fewn y bloc `am byth`{:class="block3control"} o dan y blociau cyfeiriad:

![chwaraewr](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
    os <bysell (saeth i fyny v) wedi ei phwyso? > yna 
        pwyntio i gyfeiriad (0)
        symud (4) cam
    end
    os <bysell (saeth chwith v) wedi ei phwyso? > yna 
        pwyntio i gyfeiriad (-90)
        symud (4) cam
    end
        os <bysell (saeth i lawr v) wedi ei phwyso? > yna 
        pwyntio i gyfeiriad (-180)
        symud (4) cam
    end
        os <bysell [saeth de v] wedi ei phwyso? > yna 
        pwyntio i gyfeiriad (90)
        symud (4) cam
    end
+   os <cyffwrdd lliw [#BABABA] ? > yna 
    symud (-4) cam
    end
end
```

--- /task ---

--- task ---

Ceisia wneud i'r `chwaraewr` symud trwy wal. Os yw'r côd newydd yn gweithio, ni ddylai hyn fod yn bosib.

![sgrinlun](images/world-walls-test.png) --- /task ---