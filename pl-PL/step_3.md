## Solidne ściany

\--- task \--- Ponownie sprawdź swój duszek `gracza`. Czy widzisz, że może przejść przez jasnoszare ściany?

![zrzut ekranu](images/world-walls.png) \--- /task \---

\--- task \--- Aby to naprawić, musisz sprawić, aby duszek `gracza` cofnął się, jeśli dotknie jasnoszarej ściany. Oto kod, który musisz dodać wewnątrz swojego bloku `zawsze`{:class="block3control"} poniżej bloków kierunku:

![gracz](images/player.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
    jeżeli <klawisz (strzałka w górę v) naciśnięty? > to
        ustaw kierunek na (0)
        przesuń o (4) kroki
    koniec
    jeżeli <klawisz (strzałka w lewo v) naciśnięty? > to
        ustaw kierunek na (-90)
        przesuń o (4) kroki
    koniec
        jeżeli <klawisz (strzałka w dół v) naciśnięty? > to
        ustaw kierunek na (-180)
        przesuń o (4) kroki
    koniec
        jeżeli <klawisz [strzałka w prawo v] naciśnięty? > to
        ustaw kierunek na (90)
        przesuń o (4) kroki
    koniec
+   jeżeli < dotyka koloru [#BABABA]? > to
    przesuń o (-4) kroków
    koniec
koniec
```

\--- /task \---

\--- task \---

Spróbuj przejść duszkiem `gracza` przez ścianę. Jeśli Twój nowy kod działa, nie powinno to być możliwe.

![zrzut ekranu](images/world-walls-test.png) \--- /task \---