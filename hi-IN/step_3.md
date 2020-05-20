## पक्की दीवारें

--- task ---

अपने `player` (खिलाड़ी) स्प्राइट का फिर से परीक्षण करें। क्या आप देख पा रहे हैं कि यह हल्के भूरे रंग की दीवारों (grey walls) के बीच से भी चल सकता है?

![screenshot](images/world-walls.png)

--- /task ---

--- task ---

इसे ठीक करने के लिए आपको `player` (खिलाड़ी) स्प्राइट को थोड़ा पीछे हिलना होगा अगर यह एक हल्के भूरे रंग (grey walls) की दीवार को छूता है। यहाँ दिया गया कोड आपको अपने `forever`{:class="block3control"} ब्लॉक के अंदर डालना होगा जोकि direction ब्लॉक के नीचे है:

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
        if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

--- /task ---

--- task ---

कोशिश करें कि `player` स्प्राइट दिवार के बीचो बीच से निकल जाये । यदि आपका नया कोड काम करता है, तो यह संभव नहीं होना चाहिए।

![screenshot](images/world-walls-test.png)

--- /task ---