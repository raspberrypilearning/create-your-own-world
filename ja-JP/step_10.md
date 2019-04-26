## コインを集める

あなたの `プレイヤー` スプライトは、世界中を移動するにつれてコインを集めることができるはずです。

\--- task \--- `コイン`コイン付きの新しい変数</code> {：class = "block3variables"}をあなたのプロジェクトに追加します。 \--- /task \---

\--- task \--- Select the `coin` sprite and click **show**.

![スクリーンショット](images/coin.png) \--- /task \---

\--- task \--- `コイン` スプライトにコードを追加し、それが部屋1にのみ現れるようにする。 ![スクリーンショット](images/coin.png)

```blocks3
flagが永遠に
クリックしたとき
 <（room :: variables）=[1]>
>
それ以外のとき
隠す
```

\--- /task \---

\--- task \---

`コイン` スプライトにコードを追加して、スプライト `が`{：class = "block3looks"}を隠し、 `1`{：class = "block3variables"}が `コインに追加されるようにします`{：class = "block3variables"} `プレイヤー` スプライトが `コイン` スプライトに触れて「それを拾う」場合に可変です。

![コイン](images/coin.png)

```blocks3
フラグがクリックされたときに
になるまで待ち <touching (player v)?>
変化[コインV]（1）によって
隠す
STOP [スプライトVの他のスクリプト]
```

スプライト</code>{：class = "block3control"}の他のスクリプトを停止するコード `は、 <code>コイン` スプライトが収集後に部屋1に表示されないようにするために必要です。

\--- /task \---

\--- task \--- ゲームの開始時に `コイン`{：class = "block3variables"}変数を `0`{：class = "block3variables"}に設定するコードをステージに追加します。

![ステージ](images/stage.png)

```blocks3
flagが
クリックしたとき[coins v]を [0]
```

\--- /task \---

\--- task \--- ゲームをテストしてください。 コインを集めると `コイン` 得点が `1`{：class = "block3variables"}に変わります \--- /task \---