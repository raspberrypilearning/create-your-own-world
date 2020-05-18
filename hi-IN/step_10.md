## सिक्के (Coins) बटोरना

आपका `खिलाड़ी (player)` स्प्राइट सिक्कों को बटोरने में सक्षम होना चाहिए जब वो आपकी दुनिया में चल रहा है।

\--- task \---

`coins`{:class="block3variables"} नामक एक नया वेरिएबल (variable) अपने प्रोजेक्ट में जोड़ें |

\--- /task \---

\--- task \---

`coin` (सिक्के) स्प्राइट का चुनें और **show** पर क्लिक करें |

![screenshot](images/coin.png)

\--- /task \---

\--- task \---

अपने `coin` (सिक्के) स्प्राइट में कोड जोड़ें ताकि यह केवल कमरा 1 में दिखाई दे।

![screenshot](images/coin.png)

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

अपने `coin` (सिक्के) स्प्राइट में कोड जोड़ें ताकि स्प्राइट `hides`{:class="block3looks"} और `1`{:class="block3variables"} को जोड़ा जाये `coins`{:class="block3variables"} वेरिएबल में ताकि एक बार `player` (खिलाडी) स्प्राइट `coin` स्प्राइट जैसे ही छूता है वो उसे 'उठा ले' | 

![coin](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \---

Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.

\--- /task \---