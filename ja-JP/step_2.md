## プレーヤーのスプライトを移動する

あなたの世界を動き回ることができる `プレイヤー` スプライトを作成することから始めます。

--- task ---

'Create your own world'スクラッチスタータープロジェクトを開きます。

**オンライン：** [rpf.io/create-your-own-world-on](https://rpf.io/create-your-own-world-on){:target="_blank"}にあるスタータープロジェクトを開きます。

Scratchアカウントをお持ちの場合は、 「リミックス」ボタンをクリックしてコピーできます。

**オフライン:** [rpf.io/p/ja-JP/create-your-own-world-go](https://rpf.io/p/ja-JP/create-your-own-world-go){:target="_blank"}から基本のプロジェクトをダウンロードして、オフラインエディターで開きます。 Scratchオフラインエディタをダウンロードしてインストールする必要がある場合は、 [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}で見つけることができます。

![スクリーンショット](images/world-starter.png)

--- /task ---

矢印キーを押すと、 `プレーヤー` のスプライトが移動します。 上向きの矢印が押されると、 `プレーヤー` のスプライトがステージの上方に移動します。

--- task ---

以下のコードを `プレイヤー` スプライトに追加してください。

![プレイヤー](images/player.png)

```blocks3
when flag clicked
forever
	if <key (上向き矢印 v) pressed? > then
		point in direction (0)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

旗をクリックし、上矢印キーを押し下げ続けます。 `プレイヤー` スプライトは上に移動しますか？

![スクリーンショット](images/world-up.png)

--- /task ---

--- task ---

`プレイヤー` スプライトを左に動かすには、似たようなコードを使って `イフ（もし）`{:class="block3control"}ブロックを追加する必要があります。

![プレイヤー](images/player.png)

```blocks3
when flag clicked
forever
	if <key (上向き矢印 v) pressed? > then
		point in direction (0)
		move (4) steps
	end
+	if <key (左矢印 v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

`プレイヤー` スプライトに、下や右に動かすコードを追加しましょう。 あなたがすでに書いたコードを活用してください。

--- hints ---

--- hint ---

上に移動するには、 `プレーヤー` スプライトを `0` 度の方向に向けます。 スプライトを下に動かすには、どうすればよいでしょうか？

左に動かすには、スプライトを `-90` 度の方向に向けます。 スプライトを右に動かすには、どうすればよいでしょうか？

--- /hint ---

--- hint ---

これらの2つのブロックを変更する必要があります。

![プレイヤー](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

`プレイヤー`スプライト を上に動かすコードを複製して、2つのブロックのコードを変更して、スプライトを下に動かすように書き換えます。 コードを再度複製し、スプライトが右に移動するようにコードを変更します。

--- /hint ---

--- hint ---

コードは次のようになります。

![プレイヤー](images/player.png)

```blocks3
when flag clicked
forever
	if <key (上向き矢印 v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (左矢印 v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
+    if <key (下矢印 v) pressed? > then
		point in direction (180)
		move (4) steps
	end
+    if <key (右矢印 v) pressed? > then
		point in direction (90)
		move (4) steps
	end
end
```

--- /hint ---

--- /hints ---

--- /task ---