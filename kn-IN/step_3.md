## ಘನ ಗೋಡೆಗಳು

--- task ---

ನಿಮ್ಮನ್ನು ಪರೀಕ್ಷಿಸಿ `player` ಸ್ಪ್ರೈಟ್ ಮತ್ತೆ. ಇದು ತಿಳಿ ಬೂದು ಗೋಡೆಗಳ ಮೂಲಕ ನಡೆಯಬಲ್ಲದು ಎಂದು ನೀವು ನೋಡುತ್ತೀರಾ?

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-walls.png)

--- /task ---

--- task ---

ಇದನ್ನು ಸರಿಪಡಿಸಲು, ನೀವು ಇದನ್ನು ಮಾಡಬೇಕಾಗಿದೆ `player` ಸ್ಪ್ರೈಟ್ ತಿಳಿ ಬೂದು ಗೋಡೆಗೆ ಮುಟ್ಟಿದರೆ ಹಿಂದಕ್ಕೆ ಸರಿಯುತ್ತದೆ. ನಿಮ್ಮೊಳಗೆ ನೀವು ಸೇರಿಸಬೇಕಾದ ಕೋಡ್ ಇಲ್ಲಿದೆ `forever`{:class="block3control"} ದಿಕ್ಕಿನ ಬ್ಲಾಕ್ಗಳ ಕೆಳಗೆ ನಿರ್ಬಂಧಿಸಿ:

![ಆಟಗಾರ](images/player.png)

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
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

--- /task ---

--- task ---

ಮಾಡಲು ಪ್ರಯತ್ನಿಸಿ `player` ಸ್ಪ್ರೈಟ್ ಗೋಡೆಯ ಮೂಲಕ ಚಲಿಸುತ್ತದೆ. ನಿಮ್ಮ ಹೊಸ ಕೋಡ್ ಕಾರ್ಯನಿರ್ವಹಿಸಿದರೆ, ಇದು ಸಾಧ್ಯವಾಗಬಾರದು.

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-walls-test.png)

--- /task ---