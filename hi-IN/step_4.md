## अपनी दुनिया में घूमें

`player` स्प्राइट अब अब अन्य कमरों के दरवाज़ों से चलने में सक्षम होना चाहिए

आपकी प्रोजेक्ट में अन्य कमरों के लिए बैकड्रॉप (backdrop) हैं:

![screenshot](images/world-backdrops.png)

--- task ---

`room`{:class="block3variables"} नामक एक वेरिएबल (variable) बनाये जो सारे स्प्राइटस का पता रखेगा कि `player` किस कमरे में है |

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

--- /task ---

--- task ---

जब `player` स्प्राइट पहले कमरे में नारंगी (orange) दरवाजे को छूता है, खेल को अगला बैकड्रॉप दिखाना चाहिए और `player` स्प्राइट को स्टेज के बाईं ओर वापस जाना चाहिए। इस कोड को `player` खिलाड़ी स्प्राइट के `forever`{:class="block3control"} लूप अंदर के जोड़ें:

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
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
+   if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
    end
end
```

--- /task ---

--- task ---

हर बार खेल शुरू होने पर कमरा, पात्रों की जगह और बैकड्रॉप (backdrop) को रीसेट (reset) होना चाहिए।

अपने `player` स्प्राइट के **start** ये कोड जोड़ें जो `forever`{:class="block3control"} लूप के ऊपर है, ताकी हरा झंडा क्लिक करते ही सब कुछ रिसेट (reset) होजाये:

--- hint ---

--- hint ---

जब गेम शुरू होता है:

+ `room`{:class="block3variables"} का मूल्य `1`{:class="block3variables"} करें
+ `backdrop`{:class="block3looks"} को `room1`{:class="block3looks"} में करें
+ `player` का जगह हमें सेट करना चाहिए, `x: -200 y: 0`{:class="block3motion"}

--- /hint ---

--- hint ---

आपको इन कोड ब्लॉक्स की ज़रुरत पड़ेगी:

![player](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

--- /hint ---

--- hint ---

यहां बताया गया है कि आपका तैयार कोड कैसा दिखना चाहिए:

![player](images/player.png)

```blocks3
when flag clicked
+set [room v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to (room1 v)
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
    if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
end
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

हरे झंडे पर क्लिक करें और फिर अपने `player` स्प्राइट को घुमाएं जब तक वह नारंगी दरवाजे (orange door) को छू ना ले | क्या स्प्राइट अगली स्क्रीन (screen) पर जाता है? क्या `room`{:class="block3variables"} वेरिएबल बदल के `2` होता है?

![screenshot](images/world-room-test.png)

--- /task ---