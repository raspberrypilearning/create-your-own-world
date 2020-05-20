## संकेत (Signs)

अब खिलाड़ियों को उनकी यात्रा पर मार्गदर्शन करने के लिए अपनी दुनिया में संकेत (signs) जोड़ें।

आपकी प्रोजेक्ट में `welcome sign` (स्वागत चिन्ह) भी शामिल है:

![screenshot](images/world-sign.png)

--- task ---

`welcome sign` (स्वागत चिन्ह) स्प्राइट केवल कमरे 1 में दिखाई देनी चाहिए इसलिए स्प्राइट में कुछ कोड जोड़कर सुनिश्चित करें कि ऐसा ही होता है:

--- hints ---


--- hint ---

जब `When the flag is clicked`{:class="block3events"} एक `forever`{:class="block3control"} लूप के अंदर तो यह देखें कि `if`{:class="block3control"} वो `room is 1`{:class="block3variables"} तो इस मामले में `show`{:class="block3looks"} `welcome sign` स्प्राइट वरना स्प्राइट को `else`{:class="block3control"} `hide`{:class="block3looks"}

--- /hint ---

--- hint ---

इन ब्लॉक्स की आपको आवश्यकता होगी:

![sign](images/sign.png)

```blocks3
if < > then
else
end

< (room :: variables) = [1] >

hide

show

forever
end

when flag clicked

```

--- /hint ---

--- hint ---

यहाँ पूरा कोड है:

![sign](images/sign.png)

```blocks3
when flag clicked
forever
    if < (room :: variables) = [1] > then
        show
    else
        hide
    end
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

अपने `welcome sign` (स्वागत चिह्न) स्प्राइट का कोड परीक्षण करें यह देखकर कि वह कमरों के बीच हिल पा रहा हैकि नही । चिह्न (sign) केवल कमरे 1 में दिखाई देनी चाहिए।

![screenshot](images/world-sign-test.png)

--- /task ---

--- task ---

यदि चिह्न कुछ कहता नहीं है तो वह बहुत खूब नहीं है! संदेश प्रदर्शित करने के लिए कुछ और कोड जोड़ें अगर `welcome sign` स्प्राइट को `player` छूता है:

![sign](images/sign.png)

```blocks3
when flag clicked
forever
if < (room :: variables) = [1] > then
show
else
hide
end
+if < touching (player v)? > then
say [Welcome! Can you get to the treasure?]
else
say []
end
end
```

--- /task ---

--- task ---

अपने `welcome sign` (स्वागत चिन्ह) स्प्राइट का फिर से परीक्षण करें । अब आपको एक संदेश देखना चाहिए जब `player` स्प्राइट `welcome sign` को छूता है ।

![screenshot](images/world-sign-test2.png)

--- /task ---