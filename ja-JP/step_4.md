## あなたの世界を動き回る

`プレイヤー` スプライトはドアを通って他の部屋に入ることができるはずです。

プロジェクトに追加の部屋の背景が含まれています。

![スクリーンショット](images/world-backdrops.png)

\--- task \---

`room`{：class = "block3variables"}という新しい 'for all sprites'変数を作成して、 `プレーヤー` スプライトがどのルームにあるかを追跡します。

[[[generic-scratch3-add-variable]]]

![screenshot](images/world-room.png)

\--- /task \---

\--- task \---

When the `player` sprite touches the orange door in the first room, the game should display the next backdrop, and the `player` sprite should move back to the left side of the Stage. Add this code inside the `player` sprite's `forever`{:class="block3control"} loop:

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
        方向（90）に点
        の動きは（4）ステップ
    の端部
    であれば < [#BABABA】タッチ色？ > 次に
    移動（-4）ステップ
    終了
+ < タッチ色[＃F2A24A] > 次に
    背景に（次の背景v）
    に切り替える
 xに移動：（-200）y：（0）
    change [room] v]×（1）
    端
端
```

\--- /task \---

\--- task \---

Every time the game starts, the room, character position, and backdrop need to be reset.

Add code to the **start** of your `player` sprite code above the `forever`{:class="block3control"} loop, to reset everything when the flag is clicked:

\--- hints \---

\--- hint \---

When the game starts:

+ `room`{：class = "block3variables"}の値は、 `1`{：class = "block3variables"}に設定する必要があります。
+ `背景`{：class = "block3looks"}を `room1`{：class = "block3looks"}に設定します。
+ The position of the `player` sprite should be set to `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Here are the extra blocks you need:

![player](images/player.png)

```blocks3
x：（-200）y：（0）

[room v]を（1）

背景を（room1 v）に切り替える
```

\--- /hint \---

\--- hint \---

Here's what your finished script should look like:

![player](images/player.png)

```blocks3
フラグがクリックされたときに
設定+ [ルームV]（1）〜
+は、Xに移動します（-200）、Y（0）
+（ROOM1 V）に背景を切り替え
永久
    であれば <（矢印Vアップ）キーが押され？ > 次に方向
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
        方向（90）に点
        の動きは（4）ステップ
    の端部
    であれば < [#BABABA】タッチ色？ > 次に
    の動きは（-4）ステップ
    端
    であれば < タッチ色[＃1 F2A24A] > 次いで
    （次背景V）にスイッチ背景を
    （-200）Y：（0）Xに移動
    変化[部屋vを]（1）
終了
終了
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Click the flag, and then move your `player` sprite until it touches the orange door. Does the sprite move to the next screen? Does the `room`{:class="block3variables"} variable change to `2`?

![screenshot](images/world-room-test.png)

\--- /task \---