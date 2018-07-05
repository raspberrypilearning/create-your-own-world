## Stevige muren

+ Test de sprite `speler` opnieuw, je zult waarschijnlijk merken dat die door de lichtgrijze muren kan lopen.

![screenshot](images/world-walls.png)

+ Om dit te verhelpen moet de de sprite `speler` teruggaan als een lichtgrijze muur wordt geraakt. Dit is de code die je moet toevoegen in je `herhaal`{:class="blockcontrol"} -blok onder de blokken voor de richting:

```blocks
    als < raak ik kleur [#BABABA]? > dan 
  neem (-4) stappen
end
```

+ Test deze nieuwe code: verplaats de sprite `speler` onder de muur en kijk dan of die erdoorheen kan komen. Als de code werkt zou dit niet mogelijk moeten zijn.

![screenshot](images/world-walls-test.png)