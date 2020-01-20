## Presuňte sa okolo sveta

Hráč `hráč` by mal byť schopný prejsť dverami do iných miestností.

Váš projekt obsahuje pozadie ďalších izieb:

![snímka obrazovky](images/world-backdrops.png)

\--- úloha \---

Vytvorenie nového, pre všetky škriatkov 'premenné nazvané `izba`{: class = "block3variables"}, aby mohli sledovať, ktorá izbe `hráč` sprite nachádza.

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

\--- /task \---

\--- task \---

When the `player` sprite touches the orange door in the first room, the game should display the next backdrop, and the `player` sprite should move back to the left side of the Stage. Add this code inside the `player` sprite's `forever`{:class="block3control"} loop:

![player](images/player.png)

```blocks3
keď sa vlajka preklikne
navždy
    ak <stlačíte tlačidlo (šípka nahor v)? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
    ak je stlačené tlačidlo <(šípka doľava v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec
        ak stlačíte klávesu <(šípka dole v)? > potom
        bod v smere (-180)
        posunúť (4) kroky
    koniec
        ak je stlačené tlačidlo <[šípka vpravo v]? > potom
        bod v smere (90)
        posunúť (4) kroky
    koniec
    ak < dotýkať farbu [#BABABA]? > potom
    ťah (-4), kroky
    koniec
+ v prípade < dotýkať farieb [# F2A24A] > potom
    prepínač pozadia k (ďalší v pozadí)
    prejdite na X: (-200) y: (0)
    zmena [izbu v] od (1)
    koniec
konca
```

\--- /task \---

\--- task \---

Every time the game starts, the room, character position, and backdrop need to be reset.

Add code to the **start** of your `player` sprite code above the `forever`{:class="block3control"} loop, to reset everything when the flag is clicked:

\--- hints \---

\--- hint \---

When the game starts:

+ Hodnota `miestnosti`{: class = "block3variables"} by mala byť nastavená na `1`{: class = "block3variables"}
+ `pozadie`{: class = "block3looks"} by malo byť nastavené na `miestnosti1`{: class = "block3looks"}
+ The position of the `player` sprite should be set to `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Here are the extra blocks you need:

![player](images/player.png)

```blocks3
prejdite na x: (-200) y: (0)

nastavte [miestnosť v] na (1)

spínaciu plochu do (miestnosť v)
```

\--- /hint \---

\--- hint \---

Here's what your finished script should look like:

![player](images/player.png)

```blocks3
keď príznak kliknutí
+ sada [miestnosti] pre (1)
+ prejsť na x: (-200) y: (0)
+ prepnúť kulisu (pokoj1 v)
navždy
    , pokiaľ <tlačidlo (šípka hore V) stlačené ? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
    ak je stlačené tlačidlo <(šípka doľava v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec
        ak stlačíte klávesu <(šípka dole v)? > potom
        bod v smere (-180)
        posunúť (4) kroky
    koniec
        ak je stlačené tlačidlo <[šípka vpravo v]? > potom
        bod v smere (90)
        posunúť (4) kroky
    koniec
    ak < dotýkať farbu [#BABABA]? > potom
    ťah (-4), kroky
    koniec
    v prípade, < dotýkať farba [# F2A24A] > potom
    prepínač pozadia k (ďalší v pozadí)
    prejdite na X: (-200) y: (0),
    zmena [miestnosti V ] do (1)
konca
konca
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Click the flag, and then move your `player` sprite until it touches the orange door. Does the sprite move to the next screen? Does the `room`{:class="block3variables"} variable change to `2`?

![screenshot](images/world-room-test.png)

\--- /task \---