## Borden

Laten we borden aan je wereld toevoegen om de speler op zijn reis te begeleiden.

Je project bevat een sprite `welkomstbord`:

![screenshot](images/world-sign.png)

\---task\--- De `Welkomstbord` sprite moeten alleen zichtbaar zijn in kamer 1, dus voeg code code aan de sprite toe om ervoor te zorgen dat dit gebeurt:

\--- hints \--- \--- hint \--- `Wanneer op de groene vlag wordt geklikt` {: class="block3events"}, in een `herhaal` {:class="block3control"} lus, controleer `als ` {:class="block3control"} de `kamer 1 is ` {:class="block3variables"} en activeer in dat geval het {:class="block3looks"} `welkomstbord`sprite` verschijn`, `anders` {:class="block3control"} `verdwijn` {:class="block3looks"} sprite. \--- /hint \--- \--- hint \--- Dit zijn de codeblokken die je nodig hebt:

![sign](images/sign.png)

```blocks3
<br />als &lt; &gt; dan
anders
end

&lt; (kamer:: variables) = [1] &gt;

verdwijn

verschijn

herhaal
end

wanneer op groene vlag wordt geklikt

```

\--- / hint \--- \--- hint \--- Dit is de complete code die je moet toevoegen:

![sign](images/sign.png)

```blocks3
wanneer op groene vlag wordt geklikt
herhaal
    als< (kamer :: variables) = [1] > dan
        verschijn
    anders
        verdwijn
    end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- taak \--- Test de code voor je `welkomstbord` sprite door tussen kamers te bewegen. Het bord mag alleen zichtbaar zijn in kamer 1.

![screenshot](images/world-sign-test.png) -- /task \---

\--- task \--- Een bord is niet veel als het niets zegt! Voeg code toe om een bericht weer te geven als de sprite `welkomstbord` wordt aangeraakt door de sprite `speler`:

![sign](images/sign.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal
als < (kamer :: variabelen) = [1] > dan
verschijn
anders
verberg
einde
+ als < raak ik (speler v)? > dan
zeg [Welkom! Kun je bij de schat komen?]
anders
zeg []
end
end
```

\--- /task \---

\--- taak \--- Test je `welkomstbord` sprite opnieuw. Je zou nu een bericht moeten zien wanneer de `speler` sprite het `welkomstbord` sprite raakt.

![screenshot](images/world-sign-test2.png) \--- /task \---