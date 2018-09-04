## Massive Wände

+ Prüfe deine `Spieler`-Figur, und du siehst wahrscheinlich, dass sie die Fähigkeit besitzt, durch die hellgrauen Wände hindurchzugehen.

![Screenshot](images/world-walls.png)

+ Um dies zu beheben, solltest du den `Spieler` zurückbewegen, wenn er eine hellgraue Wand berührt. Hier ist der Code, den du innerhalb des `wiederhole fortlaufend`{:class="blockcontrol"} -Blocks unter den Richtungs-Blöcken hinzufügen musst:

```blocks
    falls < wird Farbe [#BABABA] berührt? > dann 
  gehe (-4) er-Schritt
end
```

+ Test this new code: move the `player` sprite below the wall, and then see whether you can move them up into it. If your code works, this shouldn't be possible.

![Screenshot](images/world-walls-test.png)