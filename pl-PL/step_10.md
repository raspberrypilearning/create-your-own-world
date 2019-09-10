## Zbieranie monet

Twój duszek `gracza` powinien móc zbierać monety, gdy porusza się po świecie.

\--- task \--- Dodaj nową zmienną `monety`{:class="block3variables"} do swojego projektu. \--- /task \---

\--- task \--- Wybierz duszka `monety` i kliknij **pokaż**.

![zrzut ekranu](images/coin.png) \--- /task \---

\--- task \--- Dodaj kod do swojego duszka`monety`, aby pojawił się tylko w pokoju 1. ![zrzut ekranu](images/coin.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
jeżeli <(pokój :: zmienne) =[1]> to
pokaż
w przeciwnym razie
ukryj
```

\--- /task \---

\--- task \---

Dodaj kod do Twojego duszka `monety`, aby ten duszek `ukrywał się`{:class="block3looks"} i do zmiennej `moneta`{:class="block3variables"} dodane zostało `1`{:class="block3variables"}, gdy duszek `gracz` dotknie duszka `moneta`, aby ją "podnieść".

![moneta](images/coin.png)

```blocks3
kiedy kliknięto zieloną flagę
czekaj aż < dotyka [gracz v]?>
zmień [monety v] o (1)
ukryj
zatrzymaj [inne skrypty duszka v]
```

Kod `zatrzymaj inne skrypty duszka`{:class="block3control"} jest potrzebny, aby duszek `moneta` przestał być wyświetlany w pokoju 1 po jego zebraniu.

\--- /task \---

\--- task \--- Teraz dodaj kod do sceny, aby ustawić Twoją zmienną `monety`{:class="block3variables"} na `0`{:class="block3variables"} na początku gry.

![scena](images/stage.png)

```blocks3
kiedy kliknięto zieloną flagę
ustaw [monety v] na [0]
```

\--- /task \---

\--- task \--- Przetestuj swoją grę. Zebranie monety powinno zmienić ilość `monet` na `1`{:class="block3variables"}. \--- /task \---