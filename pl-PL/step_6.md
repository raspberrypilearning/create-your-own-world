## Znaki

Dodajmy znaki do twojego świata, aby poprowadzić gracza w jego podróży.

+ Twój projekt zawiera duszka `znak-powitanie`:

![zrzut ekranu](images/world-sign.png)

+ Duszek `znak-powitanie` powinien być widoczny tylko w pokoju 1, więc dodajmy kod do duszka `znak-powitanie`, aby mieć pewność, że tak się stanie:

```blocks
    kiedy kliknięto zieloną flagę
    zawsze 
        jeżeli < (pokój) = [1] > to 
            pokaż
        w przeciwnym razie
            ukryj
        end
    end
```

+ Przetestuj duszka `znak-powitanie` przemieszczając się między pokojami. Twój znak powinien być widoczny tylko w pokoju 1.
    
    ![zrzut ekranu](images/world-sign-test.png)

+ Znak nie jest zbyt dobry, jeśli nic nie mówi! Dodaj więcej kodu, aby wyświetlić wiadomość, jeśli duszek `znak-powitanie` dotknie duszka `gracza`:

```blocks
    kiedy kliknięto zieloną flagę
    zawsze 
        jeżeli < (pokój) = [1] > to 
            pokaż
        w przeciwnym razie
            ukryj
        end
        jeżeli < dotyka [gracz v]? > to
             powiedz [Witaj! Czy potrafisz dotrzeć do skarbu?]
        w przeciwnym razie
            powiedz []
        end
    end
```

+ Przetestuj duszka `znak-powitania` — powinieneś zobaczyć wiadomość, kiedy duszek `gracza` go dotknie.

![zrzut ekranu](images/world-sign-test2.png)