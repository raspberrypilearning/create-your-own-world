## ಚಿಹ್ನೆಗಳು

ಆಟಗಾರರ ಪ್ರಯಾಣದಲ್ಲಿ ಮಾರ್ಗದರ್ಶನ ನೀಡಲು ಈಗ ನಿಮ್ಮ ಜಗತ್ತಿಗೆ ಚಿಹ್ನೆಗಳನ್ನು ಸೇರಿಸಿ.

ನಿಮ್ಮ ಯೋಜನೆಯು ಒಂದು `welcome sign` ಸ್ಪ್ರೈಟ್:

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-sign.png)

--- task ---

`welcome sign` ಸ್ಪ್ರೈಟ್ ಕೊಠಡಿ 1 ರಲ್ಲಿ ಮಾತ್ರ ಗೋಚರಿಸಬೇಕು, ಆದ್ದರಿಂದ ಇದು ಸಂಭವಿಸುತ್ತದೆ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ಸ್ಪ್ರೈಟ್‌ಗೆ ಕೆಲವು ಕೋಡ್ ಸೇರಿಸಿ:

--- hints ---


--- hint ---

`When the flag is clicked`{:class="block3events"}, ಒಂದು `forever`{:class="block3control"} ಲೂಪ್, ಪರಿಶೀಲಿಸಿ `if`{:class="block3control"} `room is 1`{:class="block3variables"} ಮತ್ತು ಆ ಸಂದರ್ಭದಲ್ಲಿ `show`{:class="block3looks"} `welcome sign` ಸ್ಪ್ರೈಟ್, `else`{:class="block3control"} `hide`{:class="block3looks"} ಸ್ಪ್ರೈಟ್.

--- /hint ---

--- hint ---

ನಿಮಗೆ ಅಗತ್ಯವಿರುವ ಬ್ಲಾಕ್ಗಳು ಇಲ್ಲಿವೆ:

![ಚಿಹ್ನೆ](images/sign.png)

```blocks3
- if < > then
else
end

< (room :: variables) = [1] >

hide

show

forever
end

when flag clicked

```

--- /hint ---

--- hint ---

ಸಂಪೂರ್ಣ ಕೋಡ್ ಇಲ್ಲಿದೆ:

![ಚಿಹ್ನೆ](images/sign.png)

```blocks3
when flag clicked
forever
    if < (room :: variables) = [1] > then
        show
    else
        hide
    end
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು ಪರೀಕ್ಷಿಸಿ `welcome sign` ಕೊಠಡಿಗಳ ನಡುವೆ ಚಲಿಸುವ ಮೂಲಕ ಸ್ಪ್ರೈಟ್. ಚಿಹ್ನೆ ಕೊಠಡಿ 1 ರಲ್ಲಿ ಮಾತ್ರ ಗೋಚರಿಸಬೇಕು.

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-sign-test.png)

--- /task ---

--- task ---

ಏನನ್ನೂ ಹೇಳದಿದ್ದರೆ ಚಿಹ್ನೆ ಹೆಚ್ಚು ಒಳ್ಳೆಯದಲ್ಲ! ಒಂದು ವೇಳೆ ಸಂದೇಶವನ್ನು ಪ್ರದರ್ಶಿಸಲು ಇನ್ನೂ ಕೆಲವು ಕೋಡ್‌ಗಳನ್ನು ಸೇರಿಸಿ `welcome sign` ಸ್ಪ್ರೈಟ್ ಸ್ಪರ್ಶಿಸುತ್ತಿದೆ `player` ಸ್ಪ್ರೈಟ್:

![ಚಿಹ್ನೆ](images/sign.png)

```blocks3
when flag clicked
forever
if < (room :: variables) = [1] > then
show
else
hide
end
+if < touching (player v)? > then
say [Welcome! Can you get to the treasure?]
else
say []
end
end
```

--- /task ---

--- task ---

ನಿಮ್ಮ ಪರೀಕ್ಷಿಸಿ `welcome sign` ಸ್ಪ್ರೈಟ್ ಮತ್ತೆ. ಯಾವಾಗ ನೀವು ಈಗ ಸಂದೇಶವನ್ನು ನೋಡಬೇಕು `player` ಸ್ಪ್ರೈಟ್ ಸ್ಪರ್ಶಿಸುತ್ತದೆ `welcome sign` ಸ್ಪ್ರೈಟ್.

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-sign-test2.png)

--- /task ---