## Postacie

Dodaj inne osoby do swojego świata, którzy swoją `gracz` sprite może wchodzić w interakcje z.

\--- task \--- Przejdź do `duszka` osoby.

![duszek postać](images/person.png) \--- /task \---

\--- task \--- Dodaj trochę kodu do `osoby` duszka, aby ta osoba rozmawiała z `ikonką` graczy. Ten kod jest bardzo podobny do kodu dodanego do duszka `znak`:

![osoba](images/person.png)

```blocks3
kiedy flaga kliknęła
przejdź do x: (0) y: (-150)
zawsze
    jeśli < dotyka (gracz v)? > wtedy
        powiedz [Czy wiesz, że możesz przejść przez pomarańczowe i żółte drzwi?]
    inne
        powiedz []
    koniec
koniec
```

\--- /task \---

\--- zadanie \--- Pozwól `osoba` ikonki, aby przejść przez dodanie tych dwóch bloków w `indziej`{class = „block3control”} sekcji kodu:

![osoba](images/person.png)

```blocks3
kiedy flaga kliknęła
przejdź do x: (0) y: (-150)
zawsze
    jeśli < dotyka (gracz v)? > wtedy
        powiedz [Czy wiesz, że możesz przejść przez pomarańczowe i żółte drzwi?]
    inne
        powiedz []
+ ruch (1) kroki
+ jeśli na krawędzi, odbicie
    koniec
koniec

```

\--- /task \---

Twój duszek `postać` będzie się teraz poruszać, ale zatrzyma się aby porozmawiać z duszkiem `gracz`.

![zrzut ekranu](images/world-person-test.png)

\--- task \--- Dodaj kod do nowego `osobowego` duszka, tak aby duszek pojawił się tylko w pokoju 1. Kod, którego potrzebujesz, jest dokładnie taki sam jak kod, który sprawia, że ikonka `znak` widoczna tylko w pokoju 1.

Pamiętaj o przetestowaniu swojego nowego kodu. \--- /task \---