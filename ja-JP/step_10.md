## コインを集める

あなたの `プレイヤー` スプライトは、世界中を移動するにつれてコインを集めることができるはずです。

--- task ---

`時間`{:class="block3variables"}という新しい変数をステージに追加します。

--- /task ---

--- task ---

`コイン` のスプライトを選択し、 **表示**をクリックします。

![スクリーンショット](images/coin.png)

--- /task ---

--- task ---

`コイン` スプライトにコードを追加して、部屋1にのみ表示されるようにします。

![スクリーンショット](images/coin.png)

```blocks3
when flag clicked
forever
if <(ルーム :: variables)=[1]> then
show
else
hide
```

--- /task ---

--- task ---

`コイン` スプライトにコードを追加して、`プレーヤー` スプライトが `コイン` スプライトにさわることによってこいんを「拾い上げる」と、スプライト が`非表示`{:class="block3looks"}になり、 `1`{:class="block3variables"}ポイントが `コイン`{:class="block3variables"}変数に追加されるようにします。

![コイン](images/coin.png)

```blocks3
when flag clicked
wait until <touching (プレーヤー v)?>
change [コイン v] by (1)
hide
stop [スプライトの他のスクリプト v]
```

コード `スプライトの他のスクリプトを停止する`{:class="block3control"}は、 `コイン` スプライトが一たび拾い上げられると、とルーム1の中では非表示とするために必要となります。

--- /task ---

--- task ---

次に、ゲーム開始時に `コイン`{:class="block3variables"}変数を `0`{:class="block3variables"}に設定するために、ステージにコードを追加します。

![ステージ](images/stage.png)

```blocks3
when flag clicked
set [コイン v] to [0]
```

--- /task ---

--- task ---

あなたのゲーム（コード）をテストしましょう。 コインを集めると、 `コイン` スコアが `1`{:class="block3variables"}に変わるはずです。

--- /task ---