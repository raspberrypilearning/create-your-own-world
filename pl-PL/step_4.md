## Solidne ściany

+ Przetestuj duszka `gracza` ponownie, a zapewne zauważysz, że ma zdolność przechodzenia przez jasnoszare ściany.

![screenshot](images/world-walls.png)

+ Aby to naprawić, należy cofnąć duszka `gracza`, jeśli dotyka jasnoszarej ściany. Oto kod, który musisz dodać wewnątrz bloku `zawsze`{:class="blockcontrol"} poniżej bloków kierunku:

```blocks
    if < touching color [#BABABA]? > to
         przesuń o (-4) kroków
     end
```

+ Test this new code: move the `player` sprite below the wall, and then see whether you can move them up into it. If your code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)