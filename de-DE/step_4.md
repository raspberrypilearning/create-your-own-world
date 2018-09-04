## Massive Wände

+ Prüfe deine `Spieler`-Figur, und du siehst wahrscheinlich, dass sie die Fähigkeit besitzt, durch die hellgrauen Wände hindurchzugehen.

![Screenshot](images/world-walls.png)

+ To fix this, you should move the `player` sprite back if they're touching a light grey wall. Here's the code you'll need to add inside your `forever`{:class="blockcontrol"} block below the direction blocks:

```blocks
    if < touching color [#BABABA]? > then
        move (-4) steps
    end
```

+ Test this new code: move the `player` sprite below the wall, and then see whether you can move them up into it. If your code works, this shouldn't be possible.

![Screenshot](images/world-walls-test.png)