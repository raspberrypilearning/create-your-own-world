## आव्हान: एक शत्रू जोडा

आपण इच्छित असल्यास, आपण आपल्या गेममध्ये गस्त घालणारे शत्रू देखील जोडू शकता. जर `player` sprite शत्रूला स्पर्श करेल तेव्हा गेम संपेल.

+ आपल्या गेममध्ये आधीपासून `enemy` sprite आहे. `enemy` sprite मध्ये कोड जोडा जेणेकरून ते फक्त room 2 मध्ये दिसून येईल.

+ `enemy` sprite ला हलविण्यासाठी आणि `player` sprite ने `enemy` sprite ला स्पर्श केल्यावर गेम समाप्त करण्यासाठी कोड जोडा. हे स्वतंत्र कोड ब्लॉकमध्ये करणे सोपे आहे. आपला `enemy` sprite कोड कसा आहे ते येथे दिसू शकेल:

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

+ आपल्या नवीन कोडची चाचणी घ्या हे सुनिश्चित करण्यासाठी: 
    + `enemy` sprite केवळ रूम 2 मध्ये दिसू शकेल
    + `enemy` sprite रूम मधे गस्त घालत आहे
    + `player` sprite ने `enemy` sprite ला स्पर्श केल्यावर गेम समाप्त होईल

आपण रूम 3 मध्ये आणखी एक `enemy` sprite तयार करू शकता का जो भिंतीत असलेल्या अंतरातून वर खाली पेट्रोलिंग करेल?

![screenshot](images/world-enemy2.png)