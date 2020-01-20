## 移動玩家精靈

首先創建一個可以在你的世界中移動的 `玩家` 精靈。

\---任務\---

打開“創建您自己的世界” Scratch 啟動項目。

**Online**: open the online starter project at [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"}.

If you have a Scratch account you can make a copy by clicking **Remix**.

**Offline**: download the starter project [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_blank"}, and then open it using the offline editor. If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![screenshot](images/world-starter.png)

\--- /task \---

Pressing the arrow keys should move the `player` sprite around. When the up arrow is pressed, the `player` sprite should move upwards on the Stage in response.

\--- task \---

Add this code to the `player` sprite:

![player](images/player.png)

```blocks3
當標誌點擊
永久
    如果按下 <鍵（向上箭頭v）？ > 然後
        點方向（0）
        移動（4）步驟
    結束
結束
```

\--- /task \---

\--- task \---

Click the flag and then hold down the up arrow. Does the `player` sprite move up?

![screenshot](images/world-up.png)

\--- /task \---

\--- task \---

To move the `player` sprite to the left, you need to add another `if`{:class="block3control"} block with similar code:

![player](images/player.png)

```blocks3
當標誌點擊
永久
    如果按下 <鍵（向上箭頭v）？ > 然後
        點方向（0）
        移動（4）步驟
    結束
+如果按下 <鍵（左箭頭v）？ > 然後
        點方向（-90）
        移動（4）步驟
    結束
結束
```

\--- /task \---

\--- task \---

Add more code to your `player` sprite so it can move down and to the right as well. Use the code you already have to help you.

\--- hints \---

\--- hint \---

To move up, you point the `player` sprite in the direction `0` degrees. What do you have to do to move the sprite down?

To move left, you point the sprite in the direction `-90` degrees. What do you have to do to move the sprite right?

\--- /hint \---

\--- hint \---

You need to change these two blocks:

![player](images/player.png)

```blocks3
<key ( v) pressed>

點方向（）
```

Duplicate the code that makes the `player` sprite move upwards, and change these two blocks to make the sprite move down. Duplicate the code again, and change it to make the sprite move to the right.

\--- /hint \--- \--- hint \--- Here is how your code should look:

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

+如果按下 <鍵（向下箭頭v）？ > 然後
        點方向（180）
        移動（4）步驟
    結束
+如果按下 <鍵[右箭頭v]？ > 然後
        點方向（90）
        移動（4）步驟
    結束
結束
```

\--- /hint \--- \--- /hints \---

\--- /task \---