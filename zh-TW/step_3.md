## 堅固的牆壁

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
當標誌點擊
永久
    如果按下 <鍵（向上箭頭v）？ > 然後
        點方向（0）
        移動（4）步驟
    結束
    如果按下 <鍵（左箭頭v）？ > 然後
        點方向（-90）
        移動（4）步驟
    結束
        如果按下 <鍵（向下箭頭v）？ > 然後
        點方向（-180）
        移動（4）步驟
    結束
        如果按下 <鍵[右箭頭v]？ > 然後
        點方向（90）
        移動（4）步驟
    結束
+如果 < 接觸顏色[#BABABA]？ > 然後
    移動（-4）步驟
    結束
結束
```

\--- /任務\---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---