## 坚固的墙壁

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
当标志点击
永久
    如果按下 <键（向上箭头v）？ > 然后
        点方向（0）
        移动（4）步骤
    结束
    如果按下 <键（左箭头v）？ > 然后
        点方向（-90）
        移动（4）步骤
    结束
        如果按下 <键（向下箭头v）？ > 然后
        点方向（-180）
        移动（4）步骤
    结束
        如果按下 <键[右箭头v]？ > 然后
        点方向（90）
        移动（4）步骤
    结束
+如果 < 接触颜色[#BABABA]？ > 然后
    移动（-4）步骤
    结束
结束
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---