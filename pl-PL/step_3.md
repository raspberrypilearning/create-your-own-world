## Solidne ściany

\--- task \--- Ponownie sprawdź swój `duszek` gracza. Czy widzisz, że może przejść przez jasnoszare ściany.

![zrzut ekranu](images/world-walls.png) \--- /task \---

\--- task \--- Aby to naprawić, musisz zmusić sprite'a `gracza` powrotu, jeśli dotknie on jasnoszarej ściany. Oto kod, który musisz dodać do swojego bloku `forever`{: class = "block3control"} poniżej bloków kierunku:

![gracz](images/player.png)

```blocks3
kiedy flaga kliknęła
zawsze
    jeśli naciśnięty został <przycisk (strzałka w górę v)? > to
        punkt w kierunku (0)
        ruch (4) kroki
    koniec
    jeśli naciśnięto <przycisk (lewa strzałka v)? > następnie
        punkt w kierunku (-90)
        ruch (4) kroki
    koniec
        jeśli naciśnięto <przycisk (strzałka w dół v)? > następnie
        punkt w kierunku (-180)
        ruch (4) kroki
    koniec
        jeśli naciśnięty został <przycisk [prawa strzałka v]? > to
        punkt w kierunku (90)
        ruch (4) kroki
    koniec
+ czy < dotyka koloru [#BABABA]? > następnie
    ruch (-4) kroki
    koniec
koniec
```

\--- /task \---

\--- task \---

Postaraj się, aby grzesznik `gracza` poruszał się po ścianie. Jeśli twój nowy kod działa, nie powinno być to możliwe.

![screenshot](images/world-walls-test.png) \--- /task \---