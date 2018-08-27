## Solidne ściany

+ Przetestuj duszka `gracza` ponownie, a zapewne zauważysz, że ma zdolność przechodzenia przez jasnoszare ściany.

![zrzut ekranu](images/world-walls.png)

+ Aby to naprawić, należy cofnąć duszka `gracza`, jeśli dotyka jasnoszarej ściany. Oto kod, który musisz dodać wewnątrz bloku `zawsze`{:class="blockcontrol"} poniżej bloków kierunku:

```blocks
    jeżeli < dotyka koloru [#BABABA]? > to
         przesuń o (-4) kroków
     end
```

+ Przetestuj ten nowy kod: przemieść duszka `gracza` pod ścianę, a następnie zobacz, czy możesz poruszyć się w górę. Jeśli twój kod działa, nie powinno być to możliwe.

![zrzut ekranu](images/world-walls-test.png)