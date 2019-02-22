## Wyzwanie: dodaj wroga

Jeśli chcesz, możesz również dodać patrolujących wrogów do swojej gry. Jeżeli `gracz` sprite dotyka wroga, gra kończy się.

+ Gra zawiera już `wroga` sprite. Dodaj kod do duszka `wróg`, tak aby pojawił się tylko w pokoju 2.

+ Dodaj kod, aby przesunąć ikonkę `wrogów` i zakończyć grę, jeśli `wrogi` duszek dotknie `ikonki` graczy. Łatwiej to zrobić w oddzielnych blokach kodu. Oto jak kod Twojego duszka `wróg` może wyglądać:

```blocks3
kiedy flaga kliknęła
zawsze
jeśli <(pokój :: zmienne) =[2]> a następnie
pokazuje
inne
ukryć

gdy flaga kliknęła
zawsze
jeśli <touching (player v)?> następnie
zatrzymało [wszystkie v]

gdy flaga kliknęła
przejdź do x: ( 170) y: (0)
zawsze
powtórzeń (130)
zmiana x przez (-1)
koniec
powtórzeń (130)
zmiana x przez (1)
```

+ Przetestuj swój nowy kod, aby się upewnić, że: 
    + Gniew `wrogów` widoczny tylko w pokoju 2
    + Ghost `wrogów` patroluje pokój
    + Gra kończy się, jeśli `gracz` sprite dotyka `wróg` ikonki

Czy potrafisz stworzyć kolejnego duszka `wróg` w pokoju 3, który patroluje chodząc góra-dół w luce w ścianie?

![zrzut ekranu](images/world-enemy2.png)