## サイン

今すぐあなたの世界にサインを追加して、プレイヤーを彼らの旅に導いてください。

あなたのプロジェクトには、 `ウェルカムサイン` スプライトが含まれてい` 。</p>

<p><img src="images/world-sign.png" alt="スクリーンショット" /></p>

<p>--- task ---</p>

<p>The <code>welcome sign` sprite should only be visible in room 1, so add some code to the sprite to make sure that this happens:

\--- hints \---

\--- hint \---

`When the flag is clicked`{:class="block3events"}, in a `forever`{:class="block3control"} loop, check `if`{:class="block3control"} the `room is 1`{:class="block3variables"} and in that case `show`{:class="block3looks"} `welcome sign` sprite, `else`{:class="block3control"} `hide`{:class="block3looks"} the sprite.

\--- /hint \---

\--- hint \---

Here are the blocks you need:

![sign](images/sign.png)

```blocks3
<br />場合 < > 、次いで
他の
末端

< （部屋::変数）= [1] >

隠す

ショー

永久
の端部

フラグがクリックしたとき

```

\--- /hint \---

\--- hint \---

Here is the complete code:

![sign](images/sign.png)

```blocks3
flagが永遠に
クリックしたとき
 < （room :: variables）= [1] >
        >
    それ以外のとき
        隠す
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Test the code for your `welcome sign` sprite by moving between rooms. The sign should only be visible in room 1.

![screenshot](images/world-sign-test.png)

\--- /task \---

\--- task \---

A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

```blocks3
flagが永遠に
クリックしたとき
 < （room :: variables）= [1] >
show
else
hide
end
+ < タッチしている場合（プレーヤーv） > それから
と言う[ようこそ！ あなたは宝物に得ることができますか？]
他
[]と言う
エンド
終了
```

\--- /task \---

\--- task \---

Test your `welcome sign` sprite again. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![screenshot](images/world-sign-test2.png)

\--- /task \---