## ಸವಾಲು: ಶತ್ರುವನ್ನು ಸೇರಿಸಿ

ನೀವು ಬಯಸಿದರೆ, ನಿಮ್ಮ ಆಟಕ್ಕೆ ಗಸ್ತು ತಿರುಗುವ ಶತ್ರುಗಳನ್ನು ಸಹ ನೀವು ಸೇರಿಸಬಹುದು. `player` ಸ್ಪ್ರೈಟ್ ಶತ್ರುವನ್ನು ಮುಟ್ಟುತ್ತಾನೆ, ಆಟವು ಕೊನೆಗೊಳ್ಳುತ್ತದೆ.

+ ನಿಮ್ಮ ಆಟವು ಈಗಾಗಲೇ ಒಂದು ಹೊಂದಿದೆ `enemy` ಸ್ಪ್ರೈಟ್. ನಿಮ್ಮ ಕೋಡ್ ಸೇರಿಸಿ `enemy` ಸ್ಪ್ರೈಟ್ ಆದ್ದರಿಂದ ಅದು ಕೊಠಡಿ 2 ರಲ್ಲಿ ಮಾತ್ರ ಕಾಣಿಸಿಕೊಳ್ಳುತ್ತದೆ.

+ ಸರಿಸಲು ಕೋಡ್ ಸೇರಿಸಿ `enemy` ಸ್ಪ್ರೈಟ್ ಮತ್ತು ಆಟವನ್ನು ಕೊನೆಗೊಳಿಸಲು `enemy` ಸ್ಪ್ರೈಟ್ ಸ್ಪರ್ಶಿಸುತ್ತದೆ `player` ಸ್ಪ್ರೈಟ್. ಪ್ರತ್ಯೇಕ ಕೋಡ್ ಬ್ಲಾಕ್‌ಗಳಲ್ಲಿ ಇದನ್ನು ಮಾಡುವುದು ಸುಲಭ. ನಿಮ್ಮ `enemy` ಸ್ಪ್ರೈಟ್ ಕೋಡ್ ಕಾಣಿಸಬಹುದು:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ ಇದನ್ನು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ನಿಮ್ಮ ಹೊಸ ಕೋಡ್ ಅನ್ನು ಪರೀಕ್ಷಿಸಿ: 
    + `enemy` ಸ್ಪ್ರೈಟ್ room 2 ರಲ್ಲಿ ಮಾತ್ರ ಗೋಚರಿಸುತ್ತದೆ
    + `enemy` ಸ್ಪ್ರೈಟ್ ಕೋಣೆಯಲ್ಲಿ ಗಸ್ತು ತಿರುಗುತ್ತದೆ
    + ಒಂದು ವೇಳೆ ಆಟವು ಕೊನೆಗೊಳ್ಳುತ್ತದೆ `player` ಸ್ಪ್ರೈಟ್ ಸ್ಪರ್ಶಿಸುತ್ತದೆ `enemy` ಸ್ಪ್ರೈಟ್

ನೀವು ಇನ್ನೊಂದು `enemy` ಕೋಣೆಯ 3 ರಲ್ಲಿ ಸ್ಪ್ರೈಟ್ ಗೋಡೆಯ ಅಂತರದ ಮೂಲಕ ಮೇಲಕ್ಕೆ ಮತ್ತು ಕೆಳಕ್ಕೆ ಗಸ್ತು ತಿರುಗುತ್ತದೆಯ?

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/world-enemy2.png)