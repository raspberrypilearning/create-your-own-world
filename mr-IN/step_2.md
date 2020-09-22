## तुमचा खेळाडू (player) sprite ला हलवा

आपल्या जगात फिरू शकणारे `player` sprite तयार करुन सुरवात करा.

\--- task \---

'आपला स्वतःचा गेम तयार करा' Scratch स्टार्टर प्रकल्प उघडा.

**ऑनलाइन**: [ rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target ="_ blank"} वर एक नवीन ऑनलाइन स्क्रॅच प्रकल्प उघडा.

आपल्याकडे Scratch खाते असल्यास आपण **Remix** वर क्लिक करुन एक काॅपी बनवू शकता.

**ऑफलाइन**: [ rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_ blank"} वरून ऑफलाइन स्टार्टर प्रकल्प डाउनलोड करा आणि नंतर ते ऑफलाइन एडिटरचा वापर करून उघडा. आपल्याला स्क्रॅच ऑफलाइन एडिटर डाउनलोड आणि स्थापित करणे आवश्यक असल्यास, आपण ते [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"} येथे शोधू शकता.

![screenshot](images/world-starter.png)

\--- /task \---

एरो की दाबल्याने `player` sprite हलला पाहिजे. जेव्हा वरचा बाण दाबला जाईल तेव्हा `player` sprite प्रतिसाद म्हणून स्टेजच्या वरच्या दिशेने जावा.

\--- task \---

हा कोड `player` sprite मध्ये जोडा:

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

ध्वज क्लिक करा आणि नंतर वरचा बाण दाबून ठेवा. `player` sprite वर हलतो का?

![screenshot](images/world-up.png)

\--- /task \---

\--- task \---

`player` sprite ला डावीकडे हलविण्यासाठी, `if`{:class="block3control"} ब्लॉकमधे आपल्याला समान कोडसह आणखी एक जोडण्याची आवश्यकता आहे:

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

आपल्या `player` sprite मध्ये अधिक कोड जोडा जेणेकरून ते खाली आणि उजवीकडे देखील जाऊ शकेल. आपल्याला आधीपासून मदत करण्यासाठी आपल्याकडे असलेला कोड वापरा.

\--- hints \---

\--- hint \---

वर जाण्यासाठी आपण `player` sprite ला `0` अंश दिशेने निर्देशित करा. खाली sprite ला हलविण्यासाठी आपल्याला काय करावे लागेल?

डावीकडे हलविण्यासाठी, आपण sprite ला `-90` अंश दिशेने निर्देशित करा. उजवीकडे sprite ला हलविण्यासाठी आपल्याला काय करावे लागेल?

\--- /hint \---

\--- hint \---

आपल्याला हे दोन ब्लॉक बदलण्याची आवश्यकता आहे:

![player](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

कोड डुप्लिकेट करा `player` sprite ला वरच्या दिशेने सरकावण्यासाठी आणि sprite ला खाली हलविण्यासाठी हे दोन ब्लॉक्स बदला. कोड पुन्हा डुप्लिकेट करा आणि sprite ला उजवीकडे हलविण्यासाठी कोड बदलून घ्या.

\--- /hint \---

\--- hint \---

तुमचा कोड कसा दिसला पाहिजे हे येथे आहे:

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