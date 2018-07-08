## الأبواب والمفاتيح

ماذا لو كانت بعض الأبواب مغلقة في لعبتك، ويجب على اللاعب أن يعثر على المفاتيح لمتابعة اللعبة؟

+ عُد إلى كائن `المفتاح`. انقر فوقه بزر الفأرة الأيمن واختر **إظهار** ليظهر على المنصة.

+ حرر مظهر كائن `المفتاح` بحيث يكون لونه أزرق.

+ حوِّل خلفية المنصة إلى الغرفة 3، وضَع كائن `المفتاح` في مكان ما بحيث يصعُب الوصول إليه!
    
    ![screenshot](images/world-key.png)

+ أضف تعليمة برمجية إلى كائن `المفتاح` بحيث تضمن أنه لن يظهر إلّا في الغرفة 3.

+ أنشئ متغير قائمة جديدًا يُسمى `المخزون`{:class="blockdata"}. وسيكون هذا المخزون هو المكان الذي يخزِّن فيه كائن `اللاعب` كل الأشياء التي يجمعها.

[[[generic-scratch-make-list]]]

+ التعليمة البرمجية لالتقاط المفتاح تُشبه التعليمةَ البرمجية لجمع العملات الذهبية إلى حدٍ كبير. الفرق هو أنك تضيف المفتاح إلى المخزون.

```blocks
    when flag clicked
    wait until <touching [player v]?>
    add [blue key] to [inventory v]
    stop [other scripts in sprite v]
    hide
```

+ Test out your `key` sprite to see if you can collect it and add it to your inventory. Remember to add code to your Stage to empty your inventory at the start of the game.

```blocks
    delete (all v) of [inventory v]
```

+ Now let's add the locked door. Right-click on the `door-blue` sprite and select **show**, then position the sprite across the gap in the two walls.

![screenshot](images/world-door.png)

+ Add code to the `door-blue` sprite so that it is only visible in room 3.

+ The `door-blue` sprite should hide to allow your `player` sprite to pass once you have the blue key in your inventory.

```blocks
    when flag clicked
    wait until <[inventory v] contains [blue key]>
    stop [other scripts in sprite v]
    hide
```

+ Test out your project, and see if you can collect the blue key to open the door!