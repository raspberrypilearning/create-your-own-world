## Challange: розширюйте свій світ

Тепер ви можете продовжувати створювати свій власний світ! Ось деякі ідеї:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Додайте звуки і музику до своєї гри
+ Add more people, enemies, and signs
+ Додайте червоні та жовті двері, а також спеціальні ключі, щоб відкрити їх
+ Додайте більше кімнат до вашого світу
+ Додайте інші корисні елементи у свою гру
    
    + Використовуйте монети, щоб отримати інформацію від інших людей:

![screenshot](images/world-bribe.png)

+ Ви навіть можете додати двері на північ та південь стін кімнати 1, щоб гравець міг рухатися між приміщеннями у всіх чотирьох напрямках. For example, your game can have nine rooms in a 3×3 grid. Потім можна додати ` 3 ` до номера кімнати, щоб рухатися вниз на один рівень.

![скріншот](images/north-south-rooms.png) ![скріншот](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```