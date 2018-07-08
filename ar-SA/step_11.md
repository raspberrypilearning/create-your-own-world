## الأبواب والمفاتيح

ماذا لو كانت بعض الأبواب مغلقة في لعبتك، ويجب على اللاعب أن يعثر على المفاتيح لمتابعة اللعبة؟

+ عُد إلى كائن `المفتاح`. انقر فوقه بزر الفأرة الأيمن واختر **إظهار** ليظهر على المنصة.

+ حرر مظهر كائن `المفتاح` بحيث يكون لونه أزرق.

+ Switch your Stage backdrop to room 3, and place the `key` sprite somewhere difficult to reach!
    
    ![screenshot](images/world-key.png)

+ Add code to the `key` sprite to make sure that it is only visible in room 3.

+ Create a new list variable called `inventory`{:class="blockdata"}. This will be where you store all of the items your `player` sprite collects.

[[[generic-scratch-make-list]]]

+ The code for collecting the key is very similar to the code for collecting coins. The difference is that you add the key to your inventory.

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