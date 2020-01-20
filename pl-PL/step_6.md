## Znaki

Teraz dodaj znaki do swojego świata, aby poprowadzić graczy w ich podróży.

Twój projekt zawiera duszka `znak powitalny`:

![zrzut ekranu](images/world-sign.png)

\--- task \---

The `welcome sign` sprite should only be visible in room 1, so add some code to the sprite to make sure that this happens:

\--- hints \---

\--- hint \---

`When the flag is clicked`{:class="block3events"}, in a `forever`{:class="block3control"} loop, check `if`{:class="block3control"} the `room is 1`{:class="block3variables"} and in that case `show`{:class="block3looks"} `welcome sign` sprite, `else`{:class="block3control"} `hide`{:class="block3looks"} the sprite.

\--- /hint \---

\--- hint \---

Here are the blocks you need:

![sign](images/sign.png)

```blocks3
<br />jeżelili < > to
w przeciwnym razie
koniec

< (pokój :: zmienne) = [1] >

ukryj

pokaż

zawsze
koniec

kiedy kliknięto zieloną flagę

```

\--- /hint \---

\--- hint \---

Here is the complete code:

![sign](images/sign.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
    jeżeli < (pokój :: zmienne) = [1] > to
        pokaż
    w przeciwnym razie
        ukryj
    koniec
koniec
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Test the code for your `welcome sign` sprite by moving between rooms. The sign should only be visible in room 1.

![screenshot](images/world-sign-test.png)

\--- /task \---

\--- task \---

A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
jeżli < (pokój :: zmienne) = [1] > to
pokaż
w przeciwnym razie
ukryj
koniec
+ jeżeli < dotyka (gracz v)? > to
powiedz [Witamy! Czy uda Ci się dotrzeć do skarbu?]
w przeciwnym razie
powiedz []
koniec
koniec
```

\--- /task \---

\--- task \---

Test your `welcome sign` sprite again. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![screenshot](images/world-sign-test2.png)

\--- /task \---