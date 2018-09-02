## Oprogramuj swój świat

Pozwólmy duszkowi `gracza` przechodzić przez drzwi do innych pomieszczeń.

Twój projekt zawiera tła dla dodatkowych pokoi:

![zrzut ekranu](images/world-backdrops.png)

+ Utwórz nową zmienną 'dla wszystkich duszków' o nazwie `pokój`{:class="blockdata"}, aby śledzić w którym pomieszczeniu znajduje się duszek `gracza`.

[[[generic-scratch-add-variable]]]

![zrzut ekranu](images/world-room.png)

+ Kiedy duszek `gracza` dotknie pomarańczowych drzwi w pierwszym pomieszczeniu, kolejne tło powinno być wyświetlone, a duszek `gracza` powinien wrócić na lewą stronę sceny. Dodaj ten kod do duszka `gracza` wewnątrz pętli `zawsze`{:class="blockcontrol"}:

```blocks
    jeżeli < dotyka koloru [#F2A24A]?> to 
        zmień tło na [następne tło v]
        idź do x: (-200) y: (0)
        zmień [pokój v] o (1)        
    end
```

+ Dodaj ten kod na **początku** kodu twojego duszka `gracza` (powyżej pętli `zawsze`{:class="blockcontrol"}), aby mieć pewność, że wszystko zostanie ustawione od nowa po kliknięciu flagi:
    
    ```blocks
        ustaw [pokój v] na (1)
        idź do x: (-200) y: (0)
        zmień tło na [pokój1 v]
    ```

+ Kliknij flagę i przejdź duszkiem `gracza` przez pomarańczowe drzwi. Czy twój duszek przechodzi do następnego ekranu? Czy zmienna `pokój` {:class="blockdata"} zmienia się na `2`?

![zrzut ekranu](images/world-room-test.png)

\--- challenge \---

### Wyzwanie: przejście do poprzedniego pokoju

+ Czy potrafisz wrócić duszkiem swojego `gracza` do poprzedniego pokoju, kiedy dotknie on żółtych drzwi? Kod potrzebny do tego jest bardzo podobny do kodu, który już dodałeś, aby przejść do następnego pokoju.

\--- /challenge \---