## De sprite van de speler verplaatsen

Laten we beginnen met het maken van een sprite voor de `speler` die zich in jouw wereld kan bewegen.

--- task ---

Open de 'Maak je eigen wereld' Scratch startersproject.

**Online**: open het online startersproject op [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"}.

Als je een Scratch-account hebt, kun je een kopie maken door op **Remix** te klikken.

**Offline**: download het startersproject [rpf.io/p/nl-NL/create-your-own-world-go](http://rpf.io/p/nl-NL/create-your-own-world-go){:target="_blank"} en open het vervolgens met behulp van de offline editor. Als je de Scratch offline editor wilt downloaden en installeren dan kan je die vinden op [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![schermafdruk](images/world-starter.png)

--- /task ---

Door op de pijltjestoetsen te drukken zou de `speler` sprite moeten bewegen. Wanneer de pijl-omhoog toets wordt ingedrukt, zou de `speler` sprite omhoog moeten bewegen.

--- task ---

Voeg deze code toe aan de `speler` sprite:

![speler](images/player.png)

```blocks3
when flag clicked
forever
	if <key (up arrow v) pressed? > then
		point in direction (0)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Klik op de vlag en houd vervolgens de pijl-omhoog ingedrukt. Beweegt de `speler` sprite omhoog?

![schermafdruk](images/world-up.png)

--- /task ---

--- task ---

Om de `speler` sprite naar links te verplaatsen moet je er nog een `als`{:class="block3control"} -blok met vergelijkbare code aan toevoegen:

![speler](images/player.png)

```blocks3
when flag clicked
forever
	if <key (up arrow v) pressed? > then
		point in direction (0)
		move (4) steps
	end
+	if <key (left arrow v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Voeg meer code toe aan de `speler` sprite zodat die ook nog naar beneden en naar rechts kan bewegen. Gebruik de code die je al hebt om je te helpen.

--- hints ---


--- hint ---

Om omhoog te gaan, richt je de `speler` sprite in de richting `0` graden. Wat zou je moeten doen om de sprite naar beneden te verplaatsen?

Om naar links te gaan, richt je de speler sprite in de richting `-90` graden. Wat zou je moeten doen om de sprite naar rechts te verplaatsen?

--- /hint ---

--- hint ---

Je moet deze twee blokken veranderen:

![speler](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Dupliceer de code die de `speler` sprite naar boven beweegt en verander deze twee blokken om de sprite omlaag te laten bewegen. Dupliceer de code opnieuw en wijzig deze om de sprite naar rechts te verplaatsen.

--- /hint --- --- hint --- Zo zou de code eruit moeten zien:

![speler](images/player.png)

```blocks3
when flag clicked
forever
	if <key (up arrow v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (left arrow v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
+    if <key (down arrow v) pressed? > then
		point in direction (180)
		move (4) steps
	end
+    if <key (right arrow v) pressed? > then
		point in direction (90)
		move (4) steps
	end
end
```

--- /hint --- --- /hints ---

--- /task ---