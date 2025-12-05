## 堅い壁

--- task ---

`プレーヤー` スプライトをもう一度テストしてください。 プレイヤーが薄灰色の壁を歩いて通り抜けることができるのがわかりますか？

![スクリーンショット](images/world-walls.png)

--- /task ---

--- task ---

これを修正するには、 `プレーヤー` スプライトが薄い灰色の壁に接触した場合に、スプライトを後方に移動させる必要があります。 方向ブロックの下にある`無限ループ`{:class="block3control"}ブロック内に追加する必要があるコードは次の通りです。

![プレーヤー](images/player.png)

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
		if <key (下矢印 v) pressed? > then
		point in direction (180)
		move (4) steps
	end
		if <key (右矢印 v) pressed? > then
		point in direction (90)
		move (4) steps
	end
+	if < touching color [#BABABA]? > then
	move (-4) steps
	end
end
```

--- /task ---

--- task ---

`プレイヤー` スプライトを壁を通り抜けることができるか試してみましょう。 あなたの新しいコードがうまく動作する場合は、通り抜けることができないはずです。

![スクリーンショット](images/world-walls-test.png)

--- /task ---