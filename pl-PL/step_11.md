## Drzwi i klucze

Teraz dodasz kod, aby niektóre drzwi w twoim świecie gry były zamknięte, a gracz musi znaleźć klucz, aby je otworzyć i przejść do następnego pokoju.

\--- task \--- Przełącz się na duszka `klucz`. Kliknij na `pokaż`{:class="block3looks"} w menu Skrypty, aby duszek pojawił się na scenie. \--- /task \---

\--- task \--- Zmień kostium duszka `klucz` tak, żeby był niebieski. \--- /task \---

\--- task \--- Przełącz tło sceny na pokój3 i umieść duszka `klucz`, gdzieś gdzie trudno będzie do niego dotrzeć!

![zrzut ekranu](images/world-key.png)

\--- /task \---

\--- task \--- Dodaj kod do duszka`klucz`, aby pojawiał się tylko w pokoju 3. \--- /task \---

\--- task \--- Utwórz nową listę o nazwie `inwentarz`{:class="block3variables"} do przechowywania przedmiotów, które Twój duszek `gracz` zbiera.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- task \--- Kod, który musisz dodać do zebrania klucza, jest bardzo podobny do kodu do zbierania monet. Różnica polega na tym, że dodajesz klucz do `inwentarza`{:class="block3variables"}.

![klucz](images/key.png)

```blocks3
kiedy kliknięto zieloną flagę
czekaj aż < dotyka [gracz v]?>
dodaj [niebieski klucz] do [inwentarz v]
ukryj
zatrzymaj [inne skrypty duszka v]
```

\--- /task \---

\--- task \--- Dodaj kod do Twojej sceny, aby opróżnić inwentarz na początku gry.

```blocks3
usuń (wszystko v) z [inwentarz v]
```

\--- /task \---

\--- task \--- Przetestuj swoją grę, aby sprawdzić, czy możesz zebrać duszka `klucz` i dodać go do swojego inwentarza. \--- /task \---

\--- task \--- Teraz dodaj zamknięte drzwi. Wybierz duszka " `niebieskie drzwi` i kliknij `pokaż`{:class="block3looks} w menu Skrypty, a następnie umieść duszka w szczelinie między dwiema ścianami.

![zrzut ekranu](images/world-door.png) \--- /task \---

\--- task \--- Dodaj kod do duszka `niebieskie drzwi`, aby był widoczny tylko w pokoju 3. \--- /task \---

\--- task \--- Dodaj kod do duszka `niebieskie drzwi` tak, że gdy klucz znajduje się w `inwentarzu`{:class="block3variables"}, duszek wykonuje polecenie `ukryj`{:class="block3looks "}, aby pozwolić Twojemu duszkowi `gracz` przejść.

![drzwi](images/door.png)

```blocks3
kiedy kliknięto zieloną flagę
czekaj aż <[inwentarz v] zawiera [niebieski klucz]?>
zatrzymaj [inne skrypty duszka v]
ukryj
```

\--- /task \---

\--- task \--- Sprawdź swoją grę i zobacz, czy możesz zabrać niebieski klucz, aby otworzyć drzwi! \--- /task \---