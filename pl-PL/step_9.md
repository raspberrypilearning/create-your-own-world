## Wyzwanie: dodaj wroga

Jeśli chcesz, możesz również dodać patrolujących wrogów do swojej gry. Jeżeli duszek `gracz` dotknie wroga, gra się kończy.

+ Gra zawiera już duszka `wróg`. Dodaj kod do duszka `wróg`, tak aby pojawił się tylko w pokoju 2.

+ Dodaj kod poruszający duszkiem `wróg` oraz kończący grę, jeżeli duszek `wróg` dotknie duszka `gracz`. Łatwiej to zrobić w oddzielnych blokach kodu. Oto jak kod Twojego duszka `wróg` może wyglądać:

```blocks3
kiedy kliknięto zieloną flagę
zawsze
jeżeli <(pokój :: zmienne) =[2]> to
pokaż
w przeciwnym razie
ukryj

kiedy kliknięto zieloną flagę
zawsze
jeżeli < dotyka (gracz v)?> to
zatrzymaj [wszystko v]

kiedy kliknięto zieloną flagę
idź do x: ( 170) y: (0)
zawsze
powtarzaj (130)
zmień x o (-1)
koniec
powtarzaj (130)
zmień x o (1)
```

+ Przetestuj swój nowy kod, aby się upewnić, że: 
    + Duszek `wróg` jest widoczny tylko w pokoju 2
    + Duszek `wróg` patroluje pokój
    + Gra kończy się, jeśli duszek `gracz` dotyka duszka `wróg`

Czy potrafisz stworzyć kolejnego duszka `wróg` w pokoju 3, który patroluje chodząc w górę i w dół w luce w ścianie?

![zrzut ekranu](images/world-enemy2.png)