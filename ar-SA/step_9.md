\--- challenge \---

## التحدي: إضافة عدو

يمكنك أيضًا إضافة أعداء يقومون بدوريات حراسة. وإذا لمس اللاعب عدوًا، فستنتهي اللعبة.

+ أضف تعليمة برمجية إلى الكائن`عدو` بحيث لا يظهر إلّا في الغرفة 2.

+ أضف تعليمة برمجية لتحريك الكائن `عدو`، ولتنتهي اللعبة إذا لمس الكائن `عدو` الكائنَ `اللاعب`. It's easier to do this in separate code blocks. Here's how your `enemy` sprite code might look:

![screenshot](images/world-enemy-code.png)

+ + It's only visible in room 2
    + It patrols the room
    + The game ends if the `player` sprite touches it

\--- /challenge \---

\--- challenge \---

## Challenge: more enemies

Can you create another `enemy` sprite in room 3 that patrols up and down through the gap in the wall?

![screenshot](images/world-enemy2.png)

\--- /challenge \---