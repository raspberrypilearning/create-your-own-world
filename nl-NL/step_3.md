## Stevige muren

\--- task \--- Test je `speler` sprite opnieuw. Zie je dat het door de lichtgrijze muren kan lopen.

![screenshot](images/world-walls.png) \--- /task \---

\--- task \--- Om dit te verhelpen, moet je de ` speler` Sprite zo maken dat deze terug beweegt als het een lichtgrijze muur raakt. Dit is de code die je moet toevoegen in je `herhaal`{:class = "block3control"} -blok onder de blokken voor de richting:

![player](images/player.png)

```blocks3
wanneer groene vlag wordt aangeklikt
herhaal 
  als <toets (pijltje omhoog v) ingedrukt? > dan
            richt naar (0) graden
            neem (4) stappen
        end
        als <toets (pijltje links v) ingedrukt? > dan
            richt naar (-90) graden
            neem (4) stappen
        end
        als <toets (pijltje omlaag v) ingedrukt? > dan
            richt naar (180) graden
            neem (4) stappen
        end
        als <toets (pijltje rechts v) ingedrukt? > dan
            richt naar (90) graden
            neem (4) stappen
        end
        als < raak ik kleur[#BARBARA]? > dan 
  neem (-4) stappen
  end
end
```

\--- /task \---

\--- task \---

Probeer de `speler` sprite door een muur te verplaatsen. Als je nieuwe code werkt, zou dit niet mogelijk zijn.

![screenshot](images/world-walls-test.png) \--- /task \---