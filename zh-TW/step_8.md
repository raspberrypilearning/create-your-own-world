## 人

將您的 `玩家` 精靈可以與之互動的其他人添加到您的世界。

\--- task \---

Switch to the `person` sprite.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

Add some code to the `person` sprite so that the person talks to the `player` sprite. This code is very similar to the code you added to your `sign` sprite:

![人](images/person.png)

```blocks3
當標誌點擊
轉到x：（0）y：（ -  150）
永遠
    如果 < 觸及（玩家v）？ > 然後
        說[你知道你可以通過橙色和黃色的門嗎？]
    其他
        說[]
    結束
結束
```

\--- /任務\---

\--- task \---

Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

```blocks3
當標誌點擊
轉到x：（0）y：（ -  150）
永遠
    如果 < 觸及（玩家v）？ > 然後
        說[你知道你可以通過橙色和黃色的門嗎？]
    其他
        說[]
+移動（1）步驟
+如果在邊緣，反彈
    結束
結束
```

\--- /task \---

Your `person` sprite will now move, but will stop to talk to the `player` sprite.

![screenshot](images/world-person-test.png)

\--- task \---

Add code to your new `person` sprite so that the sprite only appears in room 1. The code you need is exactly the same as the code that makes the `sign` sprite only visible in room 1.

Make sure you test out your new code.

\--- /task \---