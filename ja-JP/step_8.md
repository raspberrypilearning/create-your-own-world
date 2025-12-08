## 人

あなたの `プレイヤー` スプライトが相互作用できる他の人々をあなたの世界に追加しましょう。

--- task ---

`人`のスプライトを選んでください。

![人のスプライト](images/person.png)

--- /task ---

--- task ---

`人` スプライトにコードを追加して、その人が `プレーヤー` スプライトと会話できるようにします。 このコードは `標識（ようこそ！）` スプライトに追加したコードにとてもよく似ています。

![人](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
	if < touching (プレーヤー v)? > then
		say [オレンジいろやきいろのどあをとおりぬけることができることをしっていたかな？]
	else
		say []
	end
end
```

--- /task ---

--- task ---

コードの `そのほか`{:class="block3control"}セクションに2つのブロックを追加することで、 `人`スプライトを移動させることができます。

![人](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
	if < touching (プレーヤー v)? > then
		say [オレンジいろやきいろのどあをとおりぬけることができることをしっていたかな？]
	else
		say []
+		move (1) steps
+		if on edge, bounce
	end
end
```

--- /task ---

`人` のスプライトは動きますが、 `プレイヤー` のスプライトと話すために立ち止まります。

![スクリーンショット](images/world-person-test.png)

--- task ---

新しい `人` のスプライトがルーム1にのみ現れるようにコードを追加しましょう。 必要なコードは、 `標識（ようこそ！）` のスプライトをルーム1でのみ見えるようにするコードとまったく同じです。

新しいコードを必ずテストしてください。

--- /task ---