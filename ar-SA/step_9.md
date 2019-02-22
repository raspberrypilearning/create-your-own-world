## تحدي: إضافة عدو

If you want, you can also add patrolling enemies to your game. If the `player` sprite touches an enemy, the game ends.

+ Your game already contains an `enemy` sprite. أضف تعليمة برمجية إلى الكائن`عدو (enemy)` بحيث لا يظهر إلّا في الغرفة 2.

+ Add code to move the `enemy` sprite and to end the game if the `enemy` sprite touches the `player` sprite. من الأسهل أن تكون التعليمات البرمجية على هيئة قوالب منفصلة. يجب أن يكون الرمز للكائن `عدو` كما يلي:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ Test out your new code to make sure that: 
    + The `enemy` sprite only visible in room 2
    + The `enemy` sprite patrols the room
    + The game ends if the `player` sprite touches the `enemy` sprite

هل يمكنك إنشاء كائن `عدو (enemy)` آخر في الغرفة 3 يتحرك إلى أعلى وإلى أسفل لحراسة الفتحة الموجودة في الحائط؟

![لقطة شاشة](images/world-enemy2.png)