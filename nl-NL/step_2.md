## De sprite van de speler verplaatsen

Laten we beginnen met het maken van een sprite voor de`speler` die zich in jouw wereld kan bewegen.

\--- task \---

Open de 'Maak je eigen wereld' Scratch startersproject.

**Online**: open het online startersproject op [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"}.

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline**: download het startersproject [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_ blank"} en open het vervolgens met behulp van de offline editor. Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![schermafdruk](images/world-starter.png)

\--- /task \---

Door op de pijltjestoetsen te drukken zou de `speler` sprite moeten bewegen. Wanneer de pijl-omhoog toets wordt ingedrukt, zou de `speler` sprite omhoog moeten bewegen.

\--- task \---

Voeg deze code toe aan de `speler` sprite:

![speler](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje omhoog v) ingedrukt? > dan 
    richt naar (0) graden
    neem (4) stappen
  einde
einde
```

\--- /task \---

\--- task \---

Klik op de vlag en houd vervolgens de pijl-omhoog ingedrukt. Beweegt de `speler` sprite omhoog?

![schermafdruk](images/world-up.png)

\--- /task \---

\--- task \---

Om de `speler` sprite naar links te verplaatsen moet je er nog een `als`{:class="block3control"} -blok met vergelijkbare code aan toevoegen:

![speler](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje omhoog v) ingedrukt? > dan
            richt naar (0) graden
            neem (4) stappen
        einde
+ als <toets (pijltje links v) ingedrukt? > dan 
    richt naar (-90) graden
    neem (4) stappen
  einde
einde
```

\--- /task \---

\--- task \---

Voeg meer code toe aan de `speler` sprite zodat die ook nog naar beneden en naar rechts kan bewegen. Gebruik de code die je al hebt om je te helpen.

\--- hints \---

\--- hint \---

Om omhoog te gaan, richt je de `speler` sprite in de richting `0` graden. Wat zou je moeten doen om de sprite naar beneden te verplaatsen?

Om naar links te gaan, richt je de speler sprite in de richting `-90` graden. Wat zou je moeten doen om de sprite naar rechts te verplaatsen?

\--- /hint \---

\--- hint \---

Je moet deze twee blokken veranderen:

![speler](images/player.png)

```blocks3
< toets ( v) ingedrukt?>

richt naar () graden
```

Dupliceer de code die de `speler` sprite naar boven beweegt en verander deze twee blokken om de sprite omlaag te laten bewegen. Dupliceer de code opnieuw en wijzig deze om de sprite naar rechts te verplaatsen.

\--- /hint \---

\--- hint \---

Here is how your code should look:

![player](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje omhoog v) ingedrukt? > dan
            richt naar (0) graden
            neem (4) stappen
        einde
        als <toets (pijltje links v) ingedrukt? > dan
            richt naar (-90) graden
            neem (4) stappen
        einde

+ als <toets (pijltje omlaag v) ingedrukt? > dan
            richt naar (180) graden
            neem (4) stappen
        einde
+        als <toets (pijltje rechts v) ingedrukt? > dan
            richt naar (180) graden
            neem (4) stappen
        einde
einde
```

\--- /hint \---

\--- /hints \---

\--- /task \---