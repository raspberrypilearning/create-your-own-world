## جدران صلبة

\--- task \--- أختبر `لاعبك`. هل ترى أنه يمكنه المشي من خلال الجدران الرمادية الفاتحة.

![لقطة الشاشة](images/world-walls.png) \--- /task \---

\--- task \--- لإصلاح ذلك ، تحتاج إلى جعل ` اللاعب ` يتحرك للخلف إذا لمس جدار رمادي فاتح. هنا التعليمات البرمجية التي ستحتاج إضافتها داخل قالب التكرار المستمر `forever` {:class="blockcontrol"} أسفل القوالب البرمجية الخاصة بالإتجاهات:

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
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

\---/task--

\--- task \---

حاول أن تجعل ` اللاعب` يتحرك من خلال الجدار. إذا كانت التعليمات البرمجية الجديدة تعمل، فلن يكون ذلك ممكنا.

![لقطة الشاشة](images/world-walls-test.png) \--- /task \---