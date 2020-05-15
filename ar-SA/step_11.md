## الأبواب والمفاتيح

الآن ستضيف تعليمة برمجية حتى تكون بعض الأبواب في عالم اللعبة الخاص بك مقفلة، ويجب على اللاعب أن يجد المفتاح لفتحها والوصول إلى الغرفة التالية.

\--- task \---

عُد إلى كائن `المفتاح`. انقر فوق ` إظهار`{:class="blocklooks"} في قائمة البرامج النصية بحيث يظهر الكائن على المنصة.

\--- /task \---

\--- task \---

حرر مظهر كائن `المفتاح` بحيث يكون لونه أزرق.

\--- /task \---

\--- task \---

حوِّل خلفية المنصة إلى الغرفة 3، وضَع كائن `المفتاح` في مكان ما بحيث يصعُب الوصول إليه!

![screenshot](images/world-key.png)

\--- /task \---

\--- task \---

أضف تعليمة برمجية إلى كائن `المفتاح` بحيث تضمن أنه لن يظهر إلّا في الغرفة 3.

\--- /task \---

\--- task \---

إنشاء قائمة جديدة تسمى `مخزن`{:class="block3variables"} لتخزين العناصر الخاصة بك `اللاعب ` مجموعات الكائن.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

التعليمة البرمجية لجمع المفتاح تُشبه التعليمةَ البرمجية لجمع العملات الذهبية إلى حدٍ كبير. الفرق هو أنك تضيف المفتاح إلى `المخزن`{:class="block3variables"}.

![key](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```

\--- /task \---

\--- task \---

Add code to your Stage to empty your inventory at the start of the game.

```blocks3
	احذف (الكل v) من [inventory v]
```

\--- /task \---

\--- task \---

Test out your game to check whether you can collect the `key` sprite and add it to your inventory.

\--- /task \---

\--- task \---

Now add the locked door. Select the `door-blue` sprite and click on `show`{:class="blocklooks} in the Scripts menu, and then position the sprite across the gap between the two walls.

![screenshot](images/world-door.png)

\--- /task \---

\--- task \---

Add code to the `door-blue` sprite so that it is only visible in room 3.

\--- /task \---

\--- task \---

Add code to the `door-blue` sprite so that, when the key is in the `inventory`{:class="block3variables"}, the sprite `hides`{:class="block3looks"} to allow your `player` sprite to pass.

![door](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \---

Test out your game and see if you can collect the blue key to open the door!

\--- /task \---