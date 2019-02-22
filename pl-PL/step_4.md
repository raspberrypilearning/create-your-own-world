## Poruszaj się po swoim świecie

Gospoda `graczy` powinna móc przejść przez drzwi do innych pomieszczeń.

Twój projekt zawiera tła dla dodatkowych pokoi:

![zrzut ekranu](images/world-backdrops.png)

\--- task \---

Utwórz nowy „dla wszystkich ikonek” zmiennej o nazwie `pokój`{: class = „block3variables”}, aby śledzić, które pokojach `gracz` Sprite jest w.

[[[generic-scratch3-add-variable]]]

![zrzut ekranu](images/world-room.png) \--- /task \---

\--- task \--- Kiedy `gracz` sprite dotknie pomarańczowych drzwi w pierwszym pokoju, gra powinna wyświetlić następne tło, a sprite `gracza` powrócić na lewą stronę stołu montażowego. Dodaj ten kod wewnątrz pętli `gracza` sprite'a ``{: class = "block3control"}:

![gracz](images/player.png)

```blocks3
kiedy flaga kliknęła
zawsze
    jeśli naciśnięty został <przycisk (strzałka w górę v)? > to
        punkt w kierunku (0)
        ruch (4) kroki
    koniec
    jeśli naciśnięto <przycisk (lewa strzałka v)? > następnie
        punkt w kierunku (-90)
        ruch (4) kroki
    koniec
        jeśli naciśnięto <przycisk (strzałka w dół v)? > następnie
        punkt w kierunku (-180)
        ruch (4) kroki
    koniec
        jeśli naciśnięty został <przycisk [prawa strzałka v]? > to
        punkt w kierunku (90)
        ruch (4) kroki
    koniec
    jeśli < dotyka koloru [#BABABA]? > następnie
    ruch (-4) kroki
    koniec
+ jeśli < dotyka kolor [# F2A24A] > następnie
    przełącz tło na (następne tło v)
    przejdź do x: (-200) Y: (0)
    zmień [pokój v] przez koniec (1)
    końca

```

\--- /task \---

\--- task \--- Za każdym razem, gdy gra się rozpocznie, należy zresetować pomieszczenie, pozycję postaci i tło.

Dodaj kod do **rozpocznij** od `kodu` duszków powyżej `pętli`{: class = "block3control"}, aby zresetować wszystko po kliknięciu flagi:

\--- wskazówki \--- \--- wskazówka \--- Kiedy gra się rozpoczyna:

+ Wartość `room`{: class = "block3variables"} powinna być ustawiona na `1`{: class = "block3variables"}
+ `backdrop`{: class = "block3looks"} powinno być ustawione na `room1`{: class = "block3looks"}
+ Pozycja ikonki `gracza` powinna być ustawiona na `x: -200 y: 0`{: class = "block3motion"} \--- / wskazówka \--- \--- podpowiedź \--- Tutaj są dodatkowe bloki, których potrzebujesz:

![gracz](images/player.png)

```blocks3
przejdź do x: (-200) y: (0)

ustaw [pokój v] na (1)

przełącz tło na (pokój1 v)
```

\--- / hint \--- \--- hint \--- Oto, jak powinien wyglądać ukończony skrypt:

![gracz](images/player.png)

```blocks3
kiedy flaga kliknęła
+ ustaw [pokój v] na (1)
+ przejdź do x: (-200) y: (0)
+ przełącz tło na (pokój1 v)
zawsze
    jeśli <klawisz (strzałka w górę v) naciśnięty ? > to
        punkt w kierunku (0)
        ruch (4) kroki
    koniec
    jeśli naciśnięto <przycisk (lewa strzałka v)? > następnie
        punkt w kierunku (-90)
        ruch (4) kroki
    koniec
        jeśli naciśnięto <przycisk (strzałka w dół v)? > następnie
        punkt w kierunku (-180)
        ruch (4) kroki
    koniec
        jeśli naciśnięty został <przycisk [prawa strzałka v]? > to
        punkt w kierunku (90)
        ruch (4) kroki
    koniec
    jeśli < dotyka koloru [#BABABA]? > następnie
    ruch (-4) kroki
    koniec
    jeśli < dotyka kolor [# F2A24A] > następnie
    przełącz tło na (następne tło v)
    przejdź do x: (-200) Y: (0)
    zmiana [pokój v ] przez (1)
koniec
koniec
```

-- /hint \--- \--- hints \---

\--- /task \---

\--- task \--- Kliknij flagę, a następnie przesuń swój `duszek` gracza, aż dotknie pomarańczowych drzwi. Czy sprite przesuwa się do następnego ekranu? Czy zmienna `room`{: class = "block3variables"} zmienia się na `2`?

![zrzut ekranu](images/world-room-test.png) \--- /task \---