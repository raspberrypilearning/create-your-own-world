## दरवाज़े और चाभियाँ

अब आप कोड जोड़ने जा रहे हैं ताकि आपके खेल की दुनिया के कुछ दरवाजे बंद (lock) हो और खिलाड़ी को उन्हें खोलने और अगले कमरे में जाने के लिए चाबी ढूंढनी होगी।

--- task ---

`key` चाभी वाली स्प्राइट पर जाएं | स्क्रिप्ट्स मेनू (Scripts menu) से `show`{:class="blocklooks"} ब्लॉक पर क्लिक करें ताकि स्प्राइट स्टेज (जहा आपके पात्र हिलते है) पर नज़र आये ।

--- /task ---

--- task ---

`key` (चाभी) स्प्राइट के पोशाक (Costume) को नीले में बदलने के लिए एडिट (edit) करें ।

--- /task ---

--- task ---

अपनी स्टेज बैकड्रॉप (stage backdrop) को कमरे 3 में बदलें और `key` (चाभी) स्प्राइट को ऐसी जगह रखें जहाँ पहुँचने के लिए मुश्किल हो!

![screenshot](images/world-key.png)

--- /task ---

--- task ---

अपने `key` (चाभी) स्प्राइट में कोड जोड़ें ताकि यह केवल कमरा 3 में दिखाई दे।

--- /task ---

--- task ---

एक नई सूची बनाएं जिसे हम कहेंगे `inventory`{:class="block3variables"} जो आपके `player` स्प्राइट द्वारा इकठ्ठा किये गए सामान (items) को एकत्रित (store) करेगा।

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

चाभी (key) को इकट्ठा करने के लिए आपको जिस कोड को जोड़ना होगा वह सिक्के एकत्र करने के कोड के समान है। अंतर यह है कि आप चाभी (key) को `inventory`{:class="block3variables"} में डालेंगे।

![key](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

खेल की शुरुआत में अपने inventory सूची को खाली करने के लिए अपने स्टेज (Stage) में कोड जोड़ें।

```blocks3
delete all of [inventory v]
```

--- /task ---

--- task ---

यह देखने के लिए कि क्या आप `key` (चाभी) एकत्र कर अपने inventory में जोड़ पाते है कि नहीं, अपने गेम का परीक्षण करें।

--- /task ---

--- task ---

अब बंद दरवाजे (locked door) को जोड़ें। `door-blue` स्प्राइट को चुनें और `show`{:class="blocklooks} पर क्लिक करें स्क्रिप्ट्स मेनू (scripts menu) में और फिर दो दीवारों के बीच में स्प्राइट को रखें।

![screenshot](images/world-door.png)

--- /task ---

--- task ---

अपने `door-blue` स्प्राइट में कोड जोड़ें ताकि यह केवल कमरा 3 में दिखाई दे।

--- /task ---

--- task ---

`door-blue` स्प्राइट में कोड जोड़ें ताकि जब key (चाभी) `inventory`{:class="block3variables"} में है तब स्प्राइट `hides`{:class="block3looks"} ताकि `player` स्प्राइट आराम से जा पाए ।

![door](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

--- /task ---

--- task ---

अपने खेल का परीक्षण करें और देखें कि क्या आप दरवाजा खोलने के लिए नीली चाभी बटोर सकते हैं!

--- /task ---