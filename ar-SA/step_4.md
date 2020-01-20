## حوائط صلبة

`اللاعب ` يجب أن يكون قادرا على التحرك عبر الأبواب للغرف الأخرى.

يحتوي مشروعك على خلفيات لغرف إضافية:

![لقطة شاشة](images/world-backdrops.png)

\--- task \---

أنشىء متغير جديد لكل الكائنات يسمى الغرفة `room`{:class="blockdata"} لتتبع الغرفة التي يكون اللاعب `player` موجودا فيها.

[[[generic-scratch3-add-variable]]]

![لقطة الشاشة](images/world-room.png) \--- /task \---

\--- task \--- عندما يلمس `اللاعب` الباب البرتقالي في الغرفة الأولى، يجب أن تظهر الخلفية الثانية، ويجب أن يتحرك `اللاعب` إلى الخلف ناحية اليسار من المنصة. أضف هذه التعليمة البرمجية إلى كائن `اللاعب` داخل حلقة التكرار `forever`{:class="blockcontrol"}:

![اللاعب](images/player.png)

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

\---/task\---

\--- task \--- كل مرة تبدأ اللعبة ، يجب إعادة تعيين الغرفة وموضع الشخصية والخلفية.

أضف هذه التعليمية البرمجية إلى **start** للتعليمة البرمجية لكائن ` player` (أعلى حلقة `forever`{:class="blockcontrol"}) لتتأكد من عودة كل شيء إلى الحالة الأولي عند النقر على العلم:

\--- hints \--- \--- hint \--- عند بداية اللعبة:

+ قيمة الغرفة `room` {: class = "block3variables"} يجب تعيينه على ` 1 ` {: class = "block3variables"}
+ قيمة `backdrop`{:class="block3looks"} يجب تعيينة علي `room1`{:class="block3looks"}
+ موقع اللاعب `player` يجب تحديده بـ `x: -200 y: 0`{:class="block3motion"} \--- /hint \--- \--- hint \--- وهاهنا الفقرة التي تحتاج اليها:

![اللاعب](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

\--- /hint \--- \--- hint \--- هذا ما يجب أن تبدو عليه تعليماتك البرمجية النهائية:

![اللاعب](images/player.png)

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

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- انقر على العلم ، ثم انقل ` للاعب` حتى يلمس الباب البرتقالي. هل ينتقل العفريت إلى الشاشة التالية؟ هل يتغير المتغير الخاص بالغرف `room`{:class="block3variables"} الي القيمة `2`؟

![لقطة الشاشة](images/world-room-test.png) \--- /task \---