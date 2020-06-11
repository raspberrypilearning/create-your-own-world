## Borden

Laten we borden aan je wereld toevoegen om de speler op zijn reis te begeleiden.

Je project bevat een sprite `welkomstbord`:

![screenshot](images/world-sign.png)

--- task --- De `Welkomstbord` sprite moeten alleen zichtbaar zijn in kamer 1, dus voeg code code aan de sprite toe om ervoor te zorgen dat dit gebeurt:

--- hints ---
 --- hint --- `Wanneer op de groene vlag wordt geklikt`{:class="block3events"}, in een `herhaal`{:class="block3control"} lus, controleer `als`{:class="block3control"} de `kamer 1 is`{:class="block3variables"} en activeer in dat geval `verschijn`{:class="block3looks"} van de `welkomstbord` sprite, `anders`{:class="block3control"} `verdwijn`{:class="block3looks"} van de sprite.
--- /hint ---
 --- hint --- Dit zijn de codeblokken die je nodig hebt:

![bord](images/sign.png)

```blocks3
if < > then
else
end

< (kamer :: variables) = [1] >

hide

show

forever
end

when flag clicked

```

--- /hint --- --- hint --- Dit is de complete code die je moet toevoegen:

![bord](images/sign.png)

```blocks3
when flag clicked
forever
	if < (kamer :: variables) = [1] > then
		show
	else
		hide
	end
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task --- Test de code voor je `welkomstbord` sprite door tussen kamers te bewegen. Het bord mag alleen zichtbaar zijn in kamer 1.

![screenshot](images/world-sign-test.png) --- /task ---

--- task --- Een bord is niet veel waard als het niets zegt! Voeg code toe om een bericht weer te geven als de sprite `welkomstbord` wordt aangeraakt door de sprite `speler`:

![bord](images/sign.png)

```blocks3
when flag clicked
forever
if < (kaer :: variables) = [1] > then
show
else
hide
end
+if < touching (speler v)? > then
say [Welkom! Kun je bij de schat komen?]
else
say []
end
end
```

--- /task ---

--- task --- Test je `welkomstbord` sprite opnieuw. Je zou nu een bericht moeten zien wanneer de `speler` sprite de `welkomstbord` sprite raakt.

![screenshot](images/world-sign-test2.png) --- /task ---