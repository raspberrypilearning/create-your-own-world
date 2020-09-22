## नाणी गोळा करा

आपला `player` sprite गेममधे फिरत असताना नाणी गोळा करण्यास सक्षम असायला हवा.

--- task ---

आपल्या प्रकल्पामधे `coins`{:class="block3variables"} हे नवीन चल जोडा.

--- /task ---

--- task ---

`coin` sprite निवडा आणि **show** वर क्लिक करा.

![screenshot](images/coin.png)

--- /task ---

--- task ---

`coin` sprite मध्ये कोड जोडा जेणेकरून ते फक्त रूम 1 मध्ये दिसून येईल.

![screenshot](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

--- /task ---

--- task ---

आपल्या `coin` sprite मध्ये कोड जोडा जेणेकरून sprite `hides`{:class="block3looks"} आणि `1`{:class="block3variables"} `coins`{:class="block3variables"} मध्ये समाविष्ट केला जाईल जेव्हा `player` sprite `coin` sprite ला 'pick it up'(उचलण्यासाठी) साठी स्पर्श करेल.

![coin](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

`stop other scripts in sprite`{:class="block3control"} sprite मध्ये इतर स्क्रिप्ट्स थांबवणे आवश्यक आहे जेणेकरून `coin` sprite संग्रहित झाल्यानंतर रूम 1 मध्ये प्रदर्शित करणे थांबेल.

--- /task ---

--- task ---

आता आपल्या गेमच्या सुरूवातीस `coins`{:class="block3variables"} मध्ये `0`{:class="block3variables"} सेट करण्यासाठी स्टेजमधे कोड जोडा.

![stage](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

--- /task ---

--- task ---

आपल्या गेमची चाचणी घ्या. नाणी गोळा केल्यानंतर आपला `coins` स्कोअर `1`{:class="block3variables"} वर बदलला पाहिजे.

--- /task ---