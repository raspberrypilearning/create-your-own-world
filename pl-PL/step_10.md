## Zbierać monety

Twój `gracz` sprite powinien być w stanie zbierać monety, jak porusza się po świecie.

\--- task \--- Dodaj nową zmienną valled `coins`{: class = "block3variables"} do swojego projektu. \--- /task \---

\--- task \--- Kliknij na ikonkę `monetę` i wybierz **pokaż**.

![zrzut ekranu](images/coin.png) \--- /task \---

\--- task \--- Dodaj kod do swojego `duszka` monet, aby pojawił się tylko w pokoju 1. ![zrzut ekranu](images/coin.png)

```blocks3
kiedy flaga kliknęła
zawsze
jeśli <(pokój :: zmienne) =[1]> a następnie
pokazuje
inny
ukryj
```

\--- /task \---

\--- task \---

Dodanie kodu do `monety` ikonki, aby ikonki `ukrywa`{: klasa = "block3looks"} i `1`{: klasa = "block3variables"} dodaje się do `monet`{: klasa = "block3variables"} Zmienna, gdy `graczy z` ikon dotknie `monet` ikonek, aby "podnieść".

![moneta](images/coin.png)

```blocks3
kiedy flaga kliknęła
czekając aż <touching (player v)?>
zmieni się [monety v] o (1)
ukryj
zatrzymaj [inne skrypty w sprite v]
```

Kod `zatrzymuje inne skrypty w sprite`{: class = "block3control"} jest potrzebny, aby `kostki` sprite przestały wyświetlać się w pokoju 1 po ich zebraniu.

\--- /task \---

\--- task \--- Teraz dodaj kod do stołu montażowego, aby ustawić `monetę`{: class = "block3variables"} zmienną na `0`{: class = "block3variables"} na początku gry.

![etap](images/stage.png)

```blocks3
kiedy flaga kliknęła
ustaw [monety v] na [0]
```

\--- /task \---

\--- task \--- Przetestuj swoją grę. Zbieranie monet powinno zmienić `punktów` na `1`{: class = "block3variables"}. \--- /task \---