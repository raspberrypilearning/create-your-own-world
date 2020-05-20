## लोग

अन्य लोगों को अपनी दुनिया में जोड़ें जो आपके `player` स्प्राइट के साथ बातचीत कर सकते हैं।

--- task ---

`person` वाले स्प्राइट पर बदलें ।

![Person sprite](images/person.png)

--- /task ---

--- task ---

`person` स्प्राइट में कुछ कोड जोड़ें ताकि वह `player` स्प्राइट से बात करे। यह कोड आपके द्वारा अपने `sign` (संकेत) स्प्राइट के कोड समान है:

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

--- /task ---

--- task ---

`person` स्प्राइट को हिलने कि आज़ादी इन दो ब्लॉक्स को जोड़कर दीजिये, यह अपने `else`{:class="block3control"} खंड में डालें:

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

--- /task ---

आपका `person` स्प्राइट अब चलेगा लेकिन `player`स्प्राइट से बात करना करने के लिए रुकेगा।

![screenshot](images/world-person-test.png)

--- task ---

अपने `person` स्प्राइट में कोड जोड़ें ताकि यह केवल कमरा 1 में दिखाई दे। आपको जिस कोड की आवश्यकता है वह कोड के समान ही है जो आपने `sign` स्प्राइट में उपयोग किया था ताकी वह केवल कमरे 1 में दिखाई दे।

सुनिश्चित करें कि आप अपने नए कोड कि परीक्षण करें।

--- /task ---