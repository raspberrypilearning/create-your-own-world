## भरीव भिंती

--- task ---

आपल्या `player` sprite ची चाचणी करून घ्या. ते हलका राखाडी भिंतींमधून जाऊ शकतात का असे आपल्यला दिसत का?

![screenshot](images/world-walls.png)

--- /task ---

--- task ---

याचे निराकरण करण्यासाठी, आपल्याला `player` sprite ला हलकी राखाडी भिंतीस स्पर्श केल्यावर मागे सरकावणे आवश्यक आहे. आपल्याला आपल्या `forever`{:class="block3control"} ब्लॉक मध्ये direction ब्लॉक्सच्या खाली आवश्यक असलेला हा कोड जोडायचा आहे:

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

`player` sprite ला भिंती मधून हलवण्यासाठी प्रयत्न करा. आपला नवीन कोड कार्य करत असल्यास, हे शक्य नाही.

![screenshot](images/world-walls-test.png)

--- /task ---