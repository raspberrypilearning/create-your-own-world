## 堅い壁

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
<キー（上向き矢印v）が押されたらフラグが永久に
クリックしたとき
 > 次に方向
        指す（0）
        移動する（4）ステップ
    終了
 <キー（左矢印v）を押すと？ > から
        方向に
ポイント（-90）
        移動（4）ステップ
    終了
 <キー（下矢印v）が押されたら > そして
        方向を向く（-180）
        移動する（4）ステップ
    終了
 <キー[右矢印v]を押すと？ > その後
        方向を指す（90）
        移動する（4）ステップ
    終了
+ < [ < ]色に触れた場合、 > から
    移動（-4）ステップ
    終了
終了
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---