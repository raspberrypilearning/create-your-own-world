## खिलाडी स्प्राइट (player sprite) को हिलाएं

एक खिलाडी `player` स्प्राइट (sprite) बनाने से शुरुआत करिये जो आपकी बनायी गयी दुनिया में घूमेगा |

\--- task \---

'Create your own world' Scratch स्टार्टर प्रोजेक्ट खोलें।

**ऑनलाइन**: आप इस प्रोजेक्ट को [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"} में खोल सकते हैं।

यदि आपके पास एक Scratch खाता (account) है, तो आप **Remix** पर क्लिक करके कॉपी बना सकते हैं।

**ऑफ़लाइन**: स्टार्टर प्रजेक्ट को [ rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_blank"} से डाउनलोड करें और फिर इसे ऑफ़लाइन एडिटर (offline editor) का उपयोग करके खोलें। यदि आपको Scratch ऑफ़लाइन एडिटर को डाउनलोड और इंस्टॉल (download and install) करने की आवश्यकता है तो आप इसे [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"} पर पा सकते हैं।

![स्क्रीनशॉट](images/world-starter.png)

\--- /task \---

Arrow keys (ऊपर निचे करना वाला बटन) को दबाने से हमारा `player` (खिलाड़ी) स्प्राइट हिलेगा | जब ऊपर का बटन दबाया जाता है, तो `player` (खिलाड़ी) स्प्राइट को प्रतिक्रिया में स्टेज (stage - जहा ये पात्र हिलते हैं) पर ऊपर की ओर जाना चाहिए।

\--- task \---

इस कोड को अपने `player` (खिलाड़ी) स्प्राइट में जोड़ें:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

हरे झंडे पर क्लिक करें और फिर ऊपर तीर वाले बटन को दबाए रखें। क्या `player` (खिलाडी) स्प्राइट ऊपर की ओर जाता है?

![स्क्रीनशॉट](images/world-up.png)

\--- /task \---

\--- task \---

`player` (खिलाड़ी) स्प्राइट को बाईं ओर हिलाने के लिए आपको एक और `if`{:class="block3control"} ब्लॉक जोड़ना होगा वो भी सामान्य कोड के साथ |

![player](images/player.png)

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

\--- /task \---

\--- task \---

अपने `player` (खिलाड़ी) स्प्राइट में और कोड जोड़ें ताकि वह नीचे और दाईं ओर भी जा सके। उस कोड का उपयोग और मदद लें जो आपके पास पहले से है।

\--- hint \---

\--- hint \---

ऊपर जाने के लिए आप `player` स्प्राइट `0` डिग्री (degrees) कि दिशा की ओर इशारा करेंगे | स्प्राइट को नीचे ले जाने के लिए आपको क्या करना होगा?

बाएं जाने के लिए आप `player` स्प्राइट <0>-90</0> डिग्री (degrees) कि दिशा की ओर इशारा करेंगे | What do you have to do to move the sprite right?

\--- /hint \---

\--- hint \---

You need to change these two blocks:

![player](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Duplicate the code that makes the `player` sprite move upwards, and change these two blocks to make the sprite move down. Duplicate the code again, and change it to make the sprite move to the right.

\--- /hint \---

\--- hint \---

Here is how your code should look:

![player](images/player.png)

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

\--- /hint \---

\--- /hints \---

\--- /task \---