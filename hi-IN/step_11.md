## दरवाज़े और चाभियाँ

अब आप कोड जोड़ने जा रहे हैं ताकि आपके खेल की दुनिया के कुछ दरवाजे बंद (lock) हो और खिलाड़ी को उन्हें खोलने और अगले कमरे में जाने के लिए चाबी ढूंढनी होगी।

\--- task \---

`key` चाभी वाली स्प्राइट पर जाएं | स्क्रिप्ट्स मेनू (Scripts menu) से `show`{:class="blocklooks"} ब्लॉक पर क्लिक करें ताकि स्प्राइट स्टेज (जहा आपके पात्र हिलते है) पर नज़र आये | 

\--- /task \---

\--- task \---

`key` (चाभी) स्प्राइट के पोशाक (Costume) को नीले में बदलने के लिए एडिट (edit) करें |

\--- /task \---

\--- task \---

अपनी स्टेज बैकड्रॉप (stage backdrop) को कमरे 3 में बदलें और `key` (चाभी) स्प्राइट को ऐसी जगह रखें जहाँ पहुँचने के लिए मुश्किल हो!

![screenshot](images/world-key.png)

\--- /task \---

\--- task \---

अपने `key` (चाभी) स्प्राइट में कोड जोड़ें ताकि यह केवल कमरा 3 में दिखाई दे।

\--- /task \---

\--- task \---

Create a new list called `inventory`{:class="block3variables"} to store the items your `player` sprite collects.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

The code you need to add for collecting the key is very similar to the code for collecting coins. The difference is that you add the key to the `inventory`{:class="block3variables"}.

![key](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```

\--- /task \---

\--- task \---

Add code to your Stage to empty your inventory at the start of the game.

```blocks3
delete (all v) of [inventory v]
```

\--- /task \---

\--- task \---

Test out your game to check whether you can collect the `key` sprite and add it to your inventory.

\--- /task \---

\--- task \---

Now add the locked door. Select the `door-blue` sprite and click on `show`{:class="blocklooks} in the Scripts menu, and then position the sprite across the gap between the two walls.

![screenshot](images/world-door.png)

\--- /task \---

\--- task \---

Add code to the `door-blue` sprite so that it is only visible in room 3.

\--- /task \---

\--- task \---

Add code to the `door-blue` sprite so that, when the key is in the `inventory`{:class="block3variables"}, the sprite `hides`{:class="block3looks"} to allow your `player` sprite to pass.

![door](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \---

Test out your game and see if you can collect the blue key to open the door!

\--- /task \---