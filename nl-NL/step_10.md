## Munten verzamelen

Je `speler` sprite zou in staat moeten zijn munten te verzamelen terwijl deze door de wereld beweegt.

\--- task \--- Voeg een nieuwe variabele `munten`{:class="block3variables"} toe aan je project. \--- /task \---

\--- task \--- Selecteer de `munt` sprite en klik op **toon**.

![screenshot](images/coin.png) \--- /task \---

\--- task \--- Voeg code toe aan je nieuwe `munt` sprite zodat de sprite alleen in kamer 1 verschijnt. ![screenshot](images/coin.png)

```blocks3
wanneer op groene vlag wordt geklikt
herhaal
als <(kamer :: variables)=[1]> dan
verschijn
anders
verdwijn
```

\--- /task \---

\--- task \---

Voeg code toe aan de `munt` sprite zodat de spite `verdwijnt`{:class="block3looks"} en `1` wordt opgeteld bij de `munten`{:class="block3variables"} variabele als de `speler` sprite de `munt` sprite aanraakt om die 'op te pakken'.

![munt](images/coin.png)

```blocks3
wanneer op groene vlag wordt geklikt
wacht tot <touching (player v)?>
verander [munten v] met (1)
verdwijn
stop [andere scripts in sprite v]
```

De code `stop andere scripts in sprite`{:class="block3control"} is nodig, zodat de `munt` sprite niet meer is te zien in kamer 1 nadat het is opgepakt.

\--- /task \---

\--- task \--- Voeg nu code toe aan het speelveld om je `munten`{:class="block3variabeles"} variabele aan het begin van het spel in te stellen op `0`{:class="block3variables"}.

![speelveld](images/stage.png)

```blocks3
wanneer op groene vlag wordt geklikt
maak [munten v] [0]
```

\--- /task \---

\--- task \--- Test je spel. Het verzamelen van een munt moet je `munten` score met `1`{:class="block3variables"} verhogen. \--- /task \---