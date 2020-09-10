## আপনার জগতের চারপাশে ঘুরুন

`player ` স্প্রিটের দরজা দিয়ে অন্যান্য ঘরে ঢুকতে পারা উচিত।.

আপনার প্রকল্পে অতিরিক্ত কক্ষগুলির জন্য ব্যাকড্রপ রয়েছে:

![screenshot](images/world-backdrops.png)

--- task ---

`player` Sprite কোন রুমে আছে সেদিকে নজর রাখার জন্য `room`{:class="block3variables"} নামে পরিচিত সকল sprite র ভেরিয়েবলের জন্য একটি নতুন 'for all sprite' variable তৈরি করুন।.

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

--- /task ---

--- task ---

`player` sprite যখন প্রথম ঘরে কমলা দরজা স্পর্শ করে, গেমটি পরবর্তী পটভূমি প্রদর্শিত হবে এবং `player` sprite টিকে স্টেজের বাম দিকে ফিরে যেতে হবে।. `player` sprite র `forever`{:class="block3control"} loop এ এই কোড যুক্ত করুন:

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

প্রতিবার খেলা শুরু হওয়ার সাথে সাথে ঘর, character র অবস্থান এবং ব্যাকড্রপগুলি পুনরায় সেট করা দরকার।.

Add code to the **start** of your `player` sprite code above the `forever`{:class="block3control"} loop, to reset everything when the flag is clicked:

--- hints ---


--- hint ---

খেলাটি যখন শুরু হয়:

+ `room`{:class="block3variables"} এর মান `1`{:class="block3variables"} হওয়া উচিত
+ `backdrop`{:class="block3looks"} টি `room1`{:class="block3looks"} হওয়া উচিত
+ `player` sprite এর অবস্থান `x: -200 y: 0`{:class="block3motion"} হওয়া উচিত

--- /hint ---

--- hint ---

Here are the extra blocks you need:

![player](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

--- /hint ---

--- hint ---

আপনার সমাপ্ত script টি দেখতে কেমন হওয়া উচিত তা এখানে আছে:

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

পতাকাটিতে ক্লিক করুন এবং তারপরে কমলার দরজাটি স্পর্শ না করা পর্যন্ত আপনার `player` sprite কে সরান।. Sprite টি কি পরের পর্দায় চলে আসে? `room`{:class="block3variables"} variable কি পরিবর্তিত হয়ে `2` হয়?

![screenshot](images/world-room-test.png)

--- /task ---