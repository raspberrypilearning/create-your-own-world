## Znaki

Teraz dodaj znaki do swojego świata, aby poprowadzić graczy w ich podróży.

Twój projekt zawiera duszka `znak-powitanie`:

![zrzut ekranu](images/world-sign.png)

\--- zadanie \--- `zadowoleniem powitać` ikonki powinny być widoczne tylko w pokoju 1, więc dodać trochę kodu do ikonki, aby upewnić się, że tak się dzieje:

\--- wskazówki \--- \--- wskazówka \--- `Kiedy flaga zostanie kliknięta`{: class = "block3events"}, w pętli `zawsze`{: class = "block3control"}, sprawdź `jeśli`{: class = "block3control"} `pokój to 1`{: class = "block3variables"} iw takim przypadku `show`{: class = "block3looks"} `znak powitalny` ikonki, `innych`{: class = "block3control"} `hide`{: class = "block3looks"} duszek. \--- / wskazówka \--- \--- wskazówka \--- Oto bloki, których potrzebujesz:

![znak](images/sign.png)

```blocks3
<br />jeśli &lt; &gt; to

koniec

&lt; (pokój :: zmienne) = [1] &gt;

ukryj

pokaż

zawsze
koniec

po kliknięciu flagi

```

\--- / wskazówka \--- \--- podpowiedź \--- Oto pełny kod:

![znak](images/sign.png)

```blocks3
kiedy flaga kliknęła
zawsze
    jeśli < (pokój :: zmienne) = [1] > a następnie
        pokazuje
    inne
        ukryj
    koniec
końca
```

-- /hint \--- \--- hints \---

\--- /task \---

\--- task \--- Przetestuj kod dla swojego `duszka` znaku powitalnego, przechodząc między pokojami. Znak powinien być widoczny tylko w pokoju 1.

![zrzut ekranu](images/world-sign-test.png) \--- /task \---

\--- task \--- Znak nie jest zbyt dobry, jeśli nic nie mówi! Dodaj więcej kodu, aby wyświetlić wiadomość, jeśli duszek `znak-powitanie` dotknie duszka `gracz`:

![znak](images/sign.png)

```blocks3
kiedy flaga kliknęła
zawsze
jeśli < (pokój :: zmienne) = [1] > a następnie
pokazuje
jeszcze
ukryć
koniec
+ czy < dotyka (gracz v)? > a następnie
powiedz [Witamy! Czy możesz dostać się do skarbu?]
else
say []
end
end
```

\--- /task \---

\--- task \--- Ponownie sprawdź swoją `duszpasterkę` znaku powitalnego. Teraz powinieneś zobaczyć komunikat, gdy `gracz` sprite dotyka `powitalny znak` ikonki.

![zrzut ekranu](images/world-sign-test2.png) \--- /task \---