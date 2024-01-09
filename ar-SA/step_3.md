## جدران صلبة

\--- task \---

اختبر كائن `اللاعب ` الخاص بك مرة أخرى. هل ترى أنه يمكنه المشي من خلال الجدران الرمادية الفاتحة؟

![لقطة الشاشة](images/world-walls.png)

\--- /task \---

\--- task \---

لإصلاح ذلك، يجب تحريك كائن `اللاعب` للخلف إذا كان يلامس الجدار الرمادي. هنا التعليمات البرمجية التي ستحتاج إضافتها داخل كتلة حلقة `كرر باستمرار`{:class="block3control"} أسفل القوالب البرمجية الخاصة بالإتجاهات:

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
        point in direction (180)
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

\--- /task \---

\--- task \---

حاول أن تجعل ` اللاعب` يتحرك من خلال الجدار. إذا كانت التعليمات البرمجية الجديدة تعمل، فلن يكون ذلك ممكنا.

![لقطة الشاشة](images/world-walls-test.png)

\--- /task \---