## दारे आणि चाबी

आता आपण कोड जोडाल जेणेकरून आपल्या गेममधील काही दारे लॉक होतील आणि ते उघडण्यासाठी आणि पुढील खोलीत जाण्यासाठी खेळाडूला एक चाबी सापडली पाहिजे.

\--- task \---

`key` sprite कडे स्विच करा. स्क्रिप्ट्स मेनूमध्ये `show`{:class="blocklooks"} वर क्लिक करा जेणेकरून sprite स्टेजवर दिसून येईल.

\--- /task \---

\--- task \---

`key` sprite's costume(पोशाख) एडिट करा जेणेकरुन ते निळे दिसेल.

\--- /task \---

\--- task \---

रूम 3 वर आपल्या स्टेज पार्श्वभूमीवर स्विच करा आणि `key` sprite असे कोठेतरी ठेवा की तिथून जाणे अवघड असेल!

![screenshot](images/world-key.png)

\--- /task \---

\--- task \---

`key` sprite मध्ये कोड जोडा जेणेकरून ते फक्त रूम 3 मध्ये दिसून येईल.

\--- /task \---

\--- task \---

`inventory`{:class="block3variables"} नावाची एक नवीन सूची तयार करा त्यात `player` sprite ने गोळा केलेल्या वस्तू जमा होतील.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

आपल्याला चाबी गोळा करण्यासाठी जो कोड जोडण्याची आवश्यकता आहे ते नाणी गोळा करण्यासाठीच्या कोडसारखेच आहे. फरक म्हणजे आपण `inventory`{:class="block3variables"} मध्ये key(चाबी) जोडणार आहो.

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

गेमच्या सुरूवातीस आपली यादी(inventory) रिक्त करण्यासाठी आपल्या स्टेजमध्ये कोड जोडा.

```blocks3
delete all of [inventory v]
```

\--- /task \---

\--- task \---

आपण `key` sprite संकलित करून आपल्या यादीमध्ये जोडू शकता की नाही हे तपासण्यासाठी आपल्या गेमची चाचणी घ्या.

\--- /task \---

\--- task \---

आता लॉक केलेला दरवाजा जोडा. `door-blue` sprite निवडा आणि स्क्रिप्ट्स मेनूमध्ये `show`{:class="blocklooks} वर क्लिक करा आणि नंतर दोन भिंतींमधील अंतर ओलांडून sprite स्थित करा.

![screenshot](images/world-door.png)

\--- /task \---

\--- task \---

`door-blue` sprite मध्ये कोड जोडा जेणेकरून ते फक्त रूम 3 मध्ये दिसून येईल.

\--- /task \---

\--- task \---

`door-blue` sprite मध्ये कोड जोडा जेणेकरून जेव्हा तुमची चाबी `inventory`{:class="block3variables"} मध्ये असेल तेव्हा, sprite `hides`{:class="block3looks"} आपल्या `player` sprite ला परवानगी देईल.

![door](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \---

आपला गेम तपासून पहा आणि आपण दार उघडण्यासाठी निळी चाबी एकत्रित करू शकता की नाही ते पहा!

\--- /task \---