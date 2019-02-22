## Przenieś sprite gracza

Zacznij od stworzenia sprite'a `gracza` który może poruszać się po Twoim świecie.

\--- task \---

Otwórz projekt startowy "Utwórz swój własny świat".

**Online**: otwórz projekt online startowy o [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){: target = "_ blank"}. Jeśli posiadasz konto Scratch, możesz kliknąć **Remix** w prawym górnym rogu, aby zapisać kopię projektu na swoim koncie.

**Offline**: pobierz projekt startowy [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){: target = "_ blank"}, a następnie otwórz go za pomocą edytora offline. Jeśli musisz pobrać i zainstalować edytor Scratcha, znajdziesz go na stronie [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![zrzut ekranu](images/world-starter.png)

\--- /task \---

Naciśnięcie klawiszy strzałek powinno przesunąć ikonkę `gracza` dookoła. Po naciśnięciu strzałki w górę, ikonka `gracza` powinna przesunąć się w górę na stole montażowym w odpowiedzi.

\--- task \---

Dodaj poniższy kod do duszka `gracz`:

![gracz](images/player.png)

```blocks3
kiedy flaga kliknęła
zawsze
    jeśli naciśnięty został <przycisk (strzałka w górę v)? > a następnie
        punkt w kierunku (0)
        ruch (4) kroki
    koniec
koniec
```

\--- /task \---

\--- task \---

Kliknij flagę, a następnie przytrzymaj strzałkę w górę. Czy `gracz` sprite poruszać się w górę?

![zrzut ekranu](images/world-up.png)

\--- /task \---

\--- task \---

Aby przesunąć ikonkę `gracza` na lewo, musisz dodać kolejny blok `jeśli`{: class = "block3control"} z podobnym kodem:

![gracz](images/player.png)

```blocks3
kiedy flaga kliknęła
zawsze
    jeśli naciśnięty został <przycisk (strzałka w górę v)? > to
        punkt w kierunku (0)
        ruch (4) kroki
    koniec
+ jeśli naciśnięto <przycisk (lewa strzałka v)? > następnie
        punkt w kierunku (-90)
        ruch (4) kroki
    koniec
koniec
```

\--- /task \---

\--- task \---

Dodaj więcej kodu do `player` ikonki więc może poruszać się w dół i na prawo, jak również. Użyj kodu, który już masz, aby sobie pomóc.

\--- wskazówka \---

\--- hint \---

Aby przejść do góry, należy wskazać ikonkę `gracza` w kierunku `0` stopni. Co musisz zrobić, aby przesunąć duszka w dół?

Aby przejść w lewo, kierujesz duszkiem w kierunku `-90 o` stopień. Co musisz zrobić, aby przenieść duszka w prawo?

\--- /wskazówka \---

\--- hint \---

Musisz zmienić te dwa bloki:

![gracz](images/player.png)

```blocks3
<key ( v) pressed>

punkt w kierunku ()
```

Powiel kod, który sprawia, że grzebień `gracza` porusza się w górę, i zmień te dwa bloki, aby sprite przesunąć w dół. Ponownie skopiuj kod i zmień go, aby sprite przesuwał się w prawo.

\--- /hint \--- \--- hint \--- Tak powinien wyglądać twój kod:

![gracz](images/player.png)

```blocks3
kiedy flaga kliknęła
zawsze
    jeśli naciśnięty został <przycisk (strzałka w górę v)? > to
        punkt w kierunku (0)
        ruch (4) kroki
    koniec
    jeśli naciśnięto <przycisk (lewa strzałka v)? > to
        punkt w kierunku (-90)
        ruch (4) kroki
    koniec

+ czy naciśnięto <przycisk (strzałka w dół v)? > to
        punkt w kierunku (180)
        ruch (4) kroki
    koniec
+ jeśli naciśnięty jest <przycisk [prawa strzałka v]? > następnie
        punkt w kierunku (90)
        ruch (4) kroki
    koniec
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---