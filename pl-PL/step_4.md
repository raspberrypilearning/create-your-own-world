## Poruszaj się po swoim świecie

Duszek `gracz` powinien móc przejść przez drzwi do innych pomieszczeń.

Twój projekt zawiera tła dla dodatkowych pokoi:

![zrzut ekranu](images/world-backdrops.png)

\--- task \---

Utwórz nową zmienną 'dla wszystkich duszków' o nazwie `pokój`{:class="block3variables"}, aby śledzić w którym pomieszczeniu znajduje się duszek `gracz`.

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

\--- /task \---

\--- task \---

When the `player` sprite touches the orange door in the first room, the game should display the next backdrop, and the `player` sprite should move back to the left side of the Stage. Add this code inside the `player` sprite's `forever`{:class="block3control"} loop:

![player](images/player.png)

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
    jeżeli < dotyka koloru [#BABABA]? > to
    przesuń o (-4) kroki
    koniec
+   jeżeli < dotyka koloru [#F2A24A] > to
    przełącz tło na (następne tło v)
    idź do x: (-200) y: (0)
    zmień [pokój v] o (1)
    koniec
koniec
```

\--- /task \---

\--- task \---

Every time the game starts, the room, character position, and backdrop need to be reset.

Add code to the **start** of your `player` sprite code above the `forever`{:class="block3control"} loop, to reset everything when the flag is clicked:

\--- hints \---

\--- hint \---

When the game starts:

+ Wartość zmiennej `pokój`{:class="block3variables"} powinna być ustawiona na `1`{:class="block3variables"}
+ `Tło`{:class="block3looks"} powinno być ustawione na `pokój1`{:class="block3looks"}
+ The position of the `player` sprite should be set to `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Here are the extra blocks you need:

![player](images/player.png)

```blocks3
idź do x: (-200) y: (0)

ustaw [pokój v] na (1)

przełącz tło na (pokój1 v)
```

\--- /hint \---

\--- hint \---

Here's what your finished script should look like:

![player](images/player.png)

```blocks3
kiedy kliknięto zieloną flagę
+ustaw [pokój v] na (1)
+Idź do x: (-200) y: (0)
+zmień tło na (pokój1 v)
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
    jeżeli < dotyka koloru [#BABABA]? > to
    przesuń o (-4) kroki
    koniec
    jeżeli < dotyka koloru [#F2A24A] > to
    przełącz tło na (następne tło v)
    idź do x: (-200) y: (0)
    zmień [pokój v] o (1)
    koniec
koniec
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Click the flag, and then move your `player` sprite until it touches the orange door. Does the sprite move to the next screen? Does the `room`{:class="block3variables"} variable change to `2`?

![screenshot](images/world-room-test.png)

\--- /task \---