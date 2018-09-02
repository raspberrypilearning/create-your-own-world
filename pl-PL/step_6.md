## Znaki

Dodajmy znaki do twojego świata, aby poprowadzić gracza w jego podróży.

+ Twój projekt zawiera duszka `znak-powitanie`:

![screenshot](images/world-sign.png)

+ Duszek `znak-powitanie` powinien być widoczny tylko w pokoju 1, więc dodajmy kod do duszka `znak-powitanie`, aby mieć pewność, że tak się stanie:

```blocks
    kiedy kliknięto zieloną flagę
    zawsze 
        jeżeli <(pokój) = [1]> to 
            pokaż
        w przeciwnym razie
            ukryj
        end
    end
```

+ Przetestuj duszka `znak-powitanie` przemieszczając się między pokojami. Twój znak powinien być widoczny tylko w pokoju 1.
    
    ![screenshot](images/world-sign-test.png)

+ Znak nie jest zbyt dobry, jeśli nic nie mówi! Dodaj więcej kodu, aby wyświetlić wiadomość, jeśli duszek `znak-powitanie` dotknie duszka `gracza`:

```blocks
    when flag clicked
    forever
        if < (room) = [1] > then
            show
        else
            hide
        end
        if < touching [player v]? > then
            say [Welcome! Can you get to the treasure?]
        else
            say []
        end
    end
```

+ Test out your `welcome sign` sprite — you should now see a message when the `player` sprite touches it.

![screenshot](images/world-sign-test2.png)