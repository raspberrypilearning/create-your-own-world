## برمج عالمك

لنسمح لكائن `اللاعب` العبور من خلال الأبواب إلى الغرف الأخرى.

يحتوي مشروعك على خلفيات لغرف إضافية:

![screenshot](images/world-backdrops.png)

+ أنشىء متغير جديد لكل الكائنات يسمى `غرفة`{:class="blockdata"} لتتبع الغرفة التي يكون كائن `اللاعب`موجود فيها.

[generic-scratch-add-variable]

![screenshot](images/world-room.png)

+ عندما يلمس كائن `اللاعب` الباب البرتقالي في الغرفة الأول، يجب أن تظهر الخلفية الثانية، ويجب أن يتحرك كائن `اللاعب` إلى الخلف ناحية اليسار من المنصة. أضف هذه التعليمة البرمجية إلى كائن `اللاعب` داخل حلقة `كرر باستمرار`{:class="blockcontrol"}:

```blocks
    if < touching color [#F2A24A] > then
        switch backdrop to [next backdrop v]
        go to x: (-200) y: (0)
        change [room v] by (1)
    end
```

+ Add this code to the **start** of your `player` sprite code (above the `forever`{:class="blockcontrol"} loop) to make sure that everything is reset when the flag is clicked:
    
    ```blocks
        set [room v] to (1)
        go to x: (-200) y: (0)
        switch backdrop to [room1 v]
    ```

+ Click the flag and move your `player` sprite over the orange door. Does your sprite move to the next screen? Does the `room`{:class="blockdata"} variable change to `2`?

![screenshot](images/world-room-test.png)

\--- challenge \---

### Challenge: moving to the previous room

+ Can you make your `player` sprite move to the previous room when they touch a yellow door? The code you need for this is very similar to the code you've already added for moving to the next room.

\--- /challenge \---