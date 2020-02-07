## Przesuń duszka gracza

Zacznij od utworzenia duszka `gracz`, który będzie mógł poruszać się po świecie gry.

\--- task \---

Otwórz projekt startowy "Utwórz swój własny świat".

**Online**: otwórz projekt startowy online pod adresem [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"}.

Jeśli masz konto Scratch, możesz wykonać kopię klikając **Remiks**.

**Offline:** pobierz projekt startowy z [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go), i otwórz w programie Scratch Desktop. Jeśli chcesz pobrać i zainstalować edytor Scratch, znajdziesz go na stronie [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![zrzut ekranu](images/world-starter.png)

\--- /task \---

Naciskanie klawiszy strzałek powinno przesuwać duszka `gracz` wokół sceny. Po naciśnięciu strzałki w górę duszek `gracz` powinien przesunąć się w górę sceny.

\--- task \---

Dodaj poniższy kod do duszka `gracz`:

![gracz](images/player.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze 
 jeżeli <klawisz (strzałka w górę v) naciśnięty? > to
        ustaw kierunek na (0)
        przesuń o (4) kroki
    koniec
koniec
```

\--- /task \---

\--- task \---

Kliknij flagę, a następnie przytrzymaj strzałkę w górę. Czy duszek `gracz` przesuwa się w górę?

![zrzut ekranu](images/world-up.png)

\--- /task \---

\--- task \---

Aby poruszyć duszka `gracz` w lewo, musisz dodać do niego kolejny blok `jeżeli`{:class="block3control"} z kodem podobnym do tego:

![gracz](images/player.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
    jeżeli <klawisz (strzałka w górę v) naciśnięty? > to
        ustaw kierunek na (0)
        przesuń o (4) kroki
    koniec
+ jeżeli <klawisz (strzałka w lewo v) naciśnięty? > to
        ustaw kierunek na (-90)
        przesuń o (4) kroki
    koniec
koniec
```

\--- /task \---

\--- task \---

Dodaj więcej kodu do swojego duszka `gracz` tak, aby mógł poruszać się również w dół i w prawo. Użyj kodu, który już masz, aby sobie pomóc.

\--- hints \---

\--- hint \---

Aby poruszać się w górę, ustaw kierunek duszka `gracz` na `0` stopni. Co należałoby zrobić, aby ruszyć duszkiem w dół?

Aby poruszać się w lewo, ustaw kierunek duszka na `90` stopni. Co należałoby zrobić, aby ruszyć duszkiem w prawo?

\--- /hint \---

\--- hint \---

Musisz zmienić te dwa bloki:

![gracz](images/player.png)

```blocks3
< klawisz ( v) naciśnięty?>

ustaw kierunek na ()
```

Zduplikuj kod, który sprawia, że duszek `gracz` przesuwa się w górę i zmień te dwa bloki, aby duszek poruszał się w dół. Ponownie zduplikuj kod i zmień go, aby duszek przesunął się w prawo.

\--- /hint \---

\--- hint \---

Here is how your code should look:

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

+ jeżeli <klawisz (strzałka w dół v) naciśnięty? > then
        point in direction (180)
        move (4) steps
    end
+    if <key (right arrow v) pressed? > to
        ustaw kierunek na (90)
        przesuń o (4) kroki
    koniec
koniec
```

\--- /hint \---

\--- /hints \---

\--- /task \---