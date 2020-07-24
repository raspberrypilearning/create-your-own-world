## लोक

आपल्या गेममध्ये इतर लोकांना जोडा जे आपल्या `player` sprite सोबत संवाद साधू शकतील.

\--- task \---

`person` sprite कडे स्विच करा.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

`person` sprite मध्ये काही कोड जोडा जेणेकरुन ती व्यक्ती `player` sprite सोबत बोलू शकेल. हा कोड आपण आपल्या `sign` sprite मध्ये जोडलेल्या कोडसारखेच आहे:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
    end
end
```

\--- /task \---

\--- task \---

`person` sprite ला हलविण्यासाठी आपल्या कोडच्या `else`{:class="block3control"} विभागात हे दोन ब्लॉक्स जोडून आपल्या sprite ला परवानगी द्या:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
+       move (1) steps
+       if on edge, bounce
    end
end
```

\--- /task \---

आपला `person` sprite आता हलेल, परंतु `player` sprite शी बोलायला थांबेल.

![screenshot](images/world-person-test.png)

\--- task \---

`enemy` sprite मध्ये कोड जोडा जेणेकरून ते फक्त रूम 1 मध्ये दिसून येईल. आपल्याला आवश्यक असलेला कोड `sign` sprite केवळ रूम 1 मध्ये दिसेल त्या कोडच्या समानच आहे.

आपण आपला नवीन कोड तपासला असल्याचे सुनिश्चित करा.

\--- /task \---