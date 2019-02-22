## Drzwi i klucze

Nie, masz zamiar dodać kod, aby niektóre drzwi w świecie gry były zablokowane, a gracz musi znaleźć klucz, aby je otworzyć i dostać się do następnego pokoju.

\--- task \--- Przełącz na `duszek z` klawiszami. Kliknij `show`{: class = "blocklooks"} w menu Skrypty, aby ikonka pojawiła się na stole montażowym. \--- /task \---

\--- zadanie \--- edytować `klucz` kostium Sprite, tak, że jest niebieski. \--- /task \---

\--- task \--- Zmień tło stołu montażowego na pokój 3 i umieść `duszek z` klawiszami w trudno dostępnym miejscu!

![zrzut ekranu](images/world-key.png)

\--- /task \---

\--- task \--- Dodaj kod do `przycisku` duszka, aby był widoczny tylko w pokoju 3. \--- /task \---

\--- zadanie \--- Utwórz nową listę o nazwie `zapasów`{: class = "block3variables"} do przechowywania przedmiotów Twój `gracz` sprite zbiera.

[[[generic-scratch3-make-list]]] \--- / zadanie \---

\--- task \--- Kod, który musisz dodać do zebrania klucza, jest bardzo podobny do kodu do zbierania monet. Różnica polega na tym, że dodajesz klucz do `inwentarza`{: class = "block3variables"}.

![klawisz](images/key.png)

```blocks3
kiedy flaga kliknęła
czekaj aż <touching (player v)?>
dodaj [niebieski klucz] do [zapasy v]
ukryj
zatrzymaj [inne skrypty w sprite v]
```

\--- /task \---

\--- task \--- Dodaj kod do stołu montażowego, aby opróżnić ekwipunek na początku gry.

```blocks3
usuń (wszystko v) z [ekwipunek v]
```

\--- /task \---

\--- task \--- Przetestuj swoją grę, aby sprawdzić, czy możesz zebrać `klawisz` sprite i dodać go do swojego ekwipunku. \--- /task \---

\--- zadanie \--- Teraz dodaj zamknięte drzwi. Wybierz ikonkę " `drzwi-niebieski` i kliknij `show`{: class = "blocklooks} w menu Skrypty, a następnie umieść duszek w szczelinie między dwiema ścianami.

![zrzut ekranu](images/world-door.png) \--- /task \---

\--- task \--- Dodaj kod do `duszka-niebieskiego` duszka, aby był widoczny tylko w pokoju 3. \--- /task \---

\--- task \--- Dodaj kod do `duszka-niebieskiego` duszka, tak, że gdy klucz znajduje się w `inwentarzu`{: class = "block3variables"}, sprite `ukrywa`{: class = "block3looks "}, aby pozwolić twojemu `graczowi na` duszków.

![drzwi](images/door.png)

```blocks3
kiedy flaga kliknęła
czekaj aż <[zapasy v] zawiera [niebieski klawisz]?>
zatrzymaj [inne skrypty w sprite v]
ukryj
```

\--- /task \---

\--- task \--- Sprawdź swoją grę i sprawdź, czy możesz zabrać niebieski klucz, aby otworzyć drzwi! \--- /task \---