## Kierowanie duszkiem `gracza`

Zacznijmy od utworzenia duszka `gracza`, który będzie mógł poruszać się po świecie gry.

+ Jeżeli używasz Scratcha w wersji online, otwórz projekt 'Stwórz swój własny świat' spod adresu <http://jumpto.cc/world-go>{:target="_blank"}. Jeżeli używasz Scratcha w wersji offline, pobierz projekt [stąd](http://jumpto.cc/world-get){:target="_blank"} i nastepnie otwórz go w edytorze offline. 

![zrzut ekranu](images/world-starter.png)

Osoba grająca w grę będzie używać klawiszy strzałek do poruszania duszkiem `gracza`. Kiedy gracz naciśnie strzałkę w górę, musisz przekazać duszkowi `gracza`, aby w odpowiedzi poruszył się we właściwym kierunku.

+ Dodaj poniższy kod do duszka `gracza`:

```blocks
    kiedy kliknięto zieloną flagę
    zawsze        
        jeżeli <klawisz [strzałka w górę v] naciśnięty? > to
            ustaw kierunek na (0)
            przesuń o (4) kroków
        end
    end
```

+ Przetestuj zachowanie duszka `gracza` klikając na zieloną flagę i wciskając strzałkę w górę. Czy duszek `gracza` porusza się do góry?
    
    ![zrzut ekranu](images/world-up.png)

+ Aby poruszyć duszka `gracza` w lewo, musisz dodać do niego kolejny blok `jeżeli` {:class="blockcontrol"} z podobnym kodem:

```blocks
    kiedy kliknięto zieloną flagę
    zawsze        
        jeżeli <klawisz [strzałka w górę v] naciśnięty? > to
            ustaw kierunek na (0)
            przesuń o (4) kroków
        end
        jeżeli <klawisz [strzałka w lewo v] naciśnięty? > to
            ustaw kierunek na (-90)
            przesuń o (4) kroków
        end
    end
```

+ Dodaj więcej kodu do swojego duszka `gracza` tak, aby mógł poruszać się również w dół i w prawo. Użyj kodu, który już masz, aby sobie pomóc.

\--- hints \--- \--- hint \--- Aby poruszać się w górę, ustawiłeś kierunek duszka `gracza` na `0` stopni. Co musiałbyś zrobić, aby ruszyć duszkiem w dół?

Aby poruszyć się w lewo, ustawiłeś kierunek duszka na `-90` stopni. Co musiałbyś zrobić, aby ruszyć duszkiem w prawo? \--- /hint \--- \--- hint \--- Będziesz musiał zmienić te dwa bloki:

```blocks
< klawisz [ v] naciśnięty? >
```

```blocks
ustaw kierunek na ()
```

Powiel kod, którego używałeś do poruszania się w górę, ale zmień te dwa bloki, aby sprawić, że duszek `gracza` pójdzie w dół. Zrób to samo, aby poruszać się w prawo. \--- /hint \--- \--- hint \--- Tak powinien wyglądać twój kod:

![Poruszanie się w dół i w prawo](images/finished-move-down-right.png) \--- /hint \--- \--- /hints \---