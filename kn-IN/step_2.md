## ಆಟಗಾರ ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಸರಿಸಿ

ರಚಿಸುವ ಮೂಲಕ ಪ್ರಾರಂಭಿಸಿ `player` ನಿಮ್ಮ ಪ್ರಪಂಚದಾದ್ಯಂತ ಚಲಿಸಬಲ್ಲ ಸ್ಪ್ರೈಟ್.

--- task ---

'ನಿಮ್ಮ ಸ್ವಂತ ಪ್ರಪಂಚವನ್ನು ರಚಿಸಿ' ಸ್ಕ್ರ್ಯಾಚ್ ಸ್ಟಾರ್ಟರ್ ಯೋಜನೆಯನ್ನು ತೆರೆಯಿರಿ.

**ಆನ್‌ಲೈನ್**: ನಲ್ಲಿ ಆನ್‌ಲೈನ್ ಸ್ಟಾರ್ಟರ್ ಯೋಜನೆಯನ್ನು ತೆರೆಯಿರಿ [rpf.io/create-your-own-world-on](https://rpf.io/create-your-own-world-on){:target="_blank"}.

ನೀವು ಸ್ಕ್ರ್ಯಾಚ್ ಖಾತೆಯನ್ನು ಹೊಂದಿದ್ದರೆ ಕ್ಲಿಕ್ ಮಾಡುವ ಮೂಲಕ ನೀವು ನಕಲನ್ನು ಮಾಡಬಹುದು **ರಿಮಿಕ್ಸ್**.

**ಆಫ್‌ಲೈನ್**: ಸ್ಟಾರ್ಟರ್ ಯೋಜನೆಯನ್ನು ಡೌನ್‌ಲೋಡ್ ಮಾಡಿ [rpf.io/p/kn-IN/create-your-own-world-go](https://rpf.io/p/kn-IN/create-your-own-world-go){:target="_blank"}, ತದನಂತರ ಅದನ್ನು ಆಫ್‌ಲೈನ್ ಸಂಪಾದಕವನ್ನು ಬಳಸಿ ತೆರೆಯಿರಿ. ನೀವು ಡೌನ್‌ಲೋಡ್ ಮಾಡಿ ಸ್ಥಾಪಿಸಬೇಕಾದರೆ Scratch ಆಫ್‌ಲೈನ್ ಸಂಪಾದಕ, ನೀವು ಅದನ್ನು ಕಾಣಬಹುದು [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-starter.png)

--- /task ---

ಬಾಣದ ಕೀಲಿಗಳನ್ನು ಒತ್ತುವುದರಿಂದ ಚಲಿಸಬೇಕು `player` ಸ್ಪ್ರೈಟ್ಸು ತ್ತಲೂ. ಮೇಲಿನ ಬಾಣ ಒತ್ತಿದಾಗ, `player` ಸ್ಪ್ರೈಟ್ ಪ್ರತಿಕ್ರಿಯೆಯಾಗಿ ವೇದಿಕೆಯ ಮೇಲೆ ಮೇಲಕ್ಕೆ ಚಲಿಸಬೇಕು.

--- task ---

ಈ ಕೋಡ್ ಅನ್ನು ಸೇರಿಸಿ `player` ಸ್ಪ್ರೈಟ್:

![ಆಟಗಾರ](images/player.png)

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

ಧ್ವಜವನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ನಂತರ ಮೇಲಿನ ಬಾಣವನ್ನು ಹಿಡಿದುಕೊಳ್ಳಿ. ಮಾಡುತ್ತದೆ `player` ಸ್ಪ್ರೈಟ್ ಮೇಲಕ್ಕೆ ಚಲಿಸುತ್ತದೆಯೇ?

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-up.png)

--- /task ---

--- task ---

ಸರಿಸಲು `player` ಸ್ಪ್ರೈಟ್ ಎಡಕ್ಕೆ, ನೀವು ಇನ್ನೊಂದನ್ನು ಸೇರಿಸುವ ಅಗತ್ಯವಿದೆ `if`{:class="block3control"} ಒಂದೇ ರೀತಿಯ ಕೋಡ್‌ನೊಂದಿಗೆ ನಿರ್ಬಂಧಿಸಿ:

![ಆಟಗಾರ](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

--- /task ---

--- task ---

ನಿಮ್ಮ ಹೆಚ್ಚಿನ ಕೋಡ್ ಅನ್ನು ಸೇರಿಸಿ `player` ಸ್ಪ್ರೈಟ್ ಆದ್ದರಿಂದ ಅದು ಕೆಳಕ್ಕೆ ಮತ್ತು ಬಲಕ್ಕೆ ಚಲಿಸಬಹುದು. ನೀವು ಈಗಾಗಲೇ ನಿಮಗೆ ಸಹಾಯ ಮಾಡಬೇಕಾದ ಕೋಡ್ ಬಳಸಿ.

--- hints ---


--- hint ---

ಮೇಲಕ್ಕೆ ಸರಿಸಲು, ನೀವು ಸೂಚಿಸುತ್ತೀರಿ `player` ಸ್ಪ್ರೈಟ್ ದಿಕ್ಕಿನಲ್ಲಿ `0` ಡಿಗ್ರಿ. ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಕೆಳಕ್ಕೆ ಸರಿಸಲು ನೀವು ಏನು ಮಾಡಬೇಕು?

ಎಡಕ್ಕೆ ಸರಿಸಲು, ನೀವು ಸ್ಪ್ರೈಟ್ ಅನ್ನು ದಿಕ್ಕಿನಲ್ಲಿ ತೋರಿಸುತ್ತೀರಿ `-90` ಡಿಗ್ರಿ. ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಸರಿಯಾಗಿ ಸರಿಸಲು ನೀವು ಏನು ಮಾಡಬೇಕು?

--- /hint ---

--- hint ---

ನೀವು ಈ ಎರಡು ಬ್ಲಾಕ್ಗಳನ್ನು ಬದಲಾಯಿಸಬೇಕಾಗಿದೆ:

![ಆಟಗಾರ](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

ಮಾಡುವ ಕೋಡ್ ಅನ್ನು ನಕಲು ಮಾಡಿ `player` ಸ್ಪ್ರೈಟ್ ಮೇಲಕ್ಕೆ ಚಲಿಸುತ್ತದೆ, ಮತ್ತು ಸ್ಪ್ರೈಟ್ ಕೆಳಗೆ ಚಲಿಸುವಂತೆ ಮಾಡಲು ಈ ಎರಡು ಬ್ಲಾಕ್ಗಳನ್ನು ಬದಲಾಯಿಸಿ. ಕೋಡ್ ಅನ್ನು ಮತ್ತೆ ನಕಲು ಮಾಡಿ, ಮತ್ತು ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಬಲಕ್ಕೆ ಚಲಿಸುವಂತೆ ಬದಲಾಯಿಸಿ.

--- /hint ---

--- hint ---

ನಿಮ್ಮ ಕೋಡ್ ಹೇಗೆ ಕಾಣಬೇಕು ಎಂಬುದು ಇಲ್ಲಿದೆ:

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

--- /hint ---

--- /hints ---

--- /task ---
