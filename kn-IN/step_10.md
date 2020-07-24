## ನಾಣ್ಯಗಳನ್ನು ಸಂಗ್ರಹಿಸಿ

ನಿಮ್ಮ`player` ಸ್ಪ್ರೈಟ್ ಪ್ರಪಂಚದಾದ್ಯಂತ ಚಲಿಸುವಾಗ ನಾಣ್ಯಗಳನ್ನು ಸಂಗ್ರಹಿಸಲು ಶಕ್ತವಾಗಿರಬೇಕು.

\--- task \---

ಹೊಸ ವೇರಿಯೇಬಲ್ ಅನ್ನು ಸೇರಿಸಿ `coins`{:class="block3variables"} ನಿಮ್ಮ ಯೋಜನೆಗೆ.

\--- /task \---

\--- task \---

ಆಯ್ಕೆಮಾಡಿ `coin` ಸ್ಪ್ರೈಟ್ ಮತ್ತು ಕ್ಲಿಕ್ ಮಾಡಿ **show**.

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/coin.png)

\--- /task \---

\--- task \---

ನಿಮ್ಮ ಕೋಡ್ ಸೇರಿಸಿ `coin` ಸ್ಪ್ರೈಟ್ ಆದ್ದರಿಂದ ಅದು ಕೊಠಡಿ 1 ರಲ್ಲಿ ಮಾತ್ರ ಕಾಣಿಸಿಕೊಳ್ಳುತ್ತದೆ.

![ಸ್ಕ್ರೀನ್‍ಶಾಟ್ (ಪರದೆ ಚಿತ್ರ)](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

ನಿಮ್ಮ ಕೋಡ್ ಸೇರಿಸಿ `coin` ಸ್ಪ್ರೈಟ್ ಆದ್ದರಿಂದ ಸ್ಪ್ರೈಟ್ `hides`{:class="block3looks"} ಮತ್ತು `1`{:class="block3variables"} ಸೇರಿಸಲಾಗಿದೆ `coins`{:class="block3variables"} ಒಮ್ಮೆ ವೇರಿಯಬಲ್ `player` ಸ್ಪ್ರೈಟ್ ಸ್ಪರ್ಶಿಸುತ್ತದೆ `coin` ಸ್ಪ್ರೈಟ್ ಅನ್ನು 'ಅದನ್ನು ತೆಗೆದುಕೊಳ್ಳಲು'.

![ನಾಣ್ಯ](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

ಕೋಡ್ `stop other scripts in sprite`{:class="block3control"} ಅಗತ್ಯವಿದೆ ಆದ್ದರಿಂದ `coin` ಸ್ಪ್ರೈಟ್ ಅದನ್ನು ಸಂಗ್ರಹಿಸಿದ ನಂತರ ಕೊಠಡಿ 1 ರಲ್ಲಿ ಪ್ರದರ್ಶಿಸುವುದನ್ನು ನಿಲ್ಲಿಸುತ್ತದೆ.

\--- /task \---

\--- task \---

ನಿಮ್ಮ ಹೊಂದಿಸಲು ಈಗ ಹಂತಕ್ಕೆ ಕೋಡ್ ಸೇರಿಸಿ `coins`{:class="block3variables"} ವೇರಿಯಬಲ್ಗೆ `0`{:class="block3variables"} ಆಟದ ಪ್ರಾರಂಭದಲ್ಲಿ.

![ಹಂತ](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

ನಿಮ್ಮ ಆಟವನ್ನು ಪರೀಕ್ಷಿಸಿ. ನಾಣ್ಯವನ್ನು ಸಂಗ್ರಹಿಸುವುದ್ದರಿಂದ ನಿಮ್ಮ ಬದಲಾವಣೆ `ನಾಣ್ಯಗಳು` ಸ್ಕೋರ್ `1`{:class="block3variables"}.

\--- /task \---