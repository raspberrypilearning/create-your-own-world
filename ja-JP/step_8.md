## 人

あなたの `プレイヤー` スプライトが相互作用できる他の人々をあなたの世界に追加しましょう。

\--- task \---

Switch to the `person` sprite.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

Add some code to the `person` sprite so that the person talks to the `player` sprite. This code is very similar to the code you added to your `sign` sprite:

![人](images/person.png)

```blocks3
旗がクリックされたとき
はxに行きます：（0）y：（-150）
永遠に
 < 触れたら
 （プレイヤーv） > その後、
        [あなたはオレンジと黄色のドアを通って行くことができることを知っていますか？]と言う
    他
        []と言う
    終了
終了
```

\--- /task \---

\--- task \---

Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

```blocks3
旗がクリックされたとき
はxに行きます：（0）y：（-150）
永遠に
 < 触れたら
 （プレイヤーv） > その後、
        [あなたはオレンジと黄色のドアを通って行くことができることを知っていますか？]と言う
    他
        []と言う
+移動が（1）の手順
端に、バウンス場合は+
    終了
終了を
```

\--- /task \---

Your `person` sprite will now move, but will stop to talk to the `player` sprite.

![screenshot](images/world-person-test.png)

\--- task \---

Add code to your new `person` sprite so that the sprite only appears in room 1. The code you need is exactly the same as the code that makes the `sign` sprite only visible in room 1.

Make sure you test out your new code.

\--- /task \---