## ドアとキー

Now you are going to add code so that some of the doors in your game world are locked, and the player must find the key to open them and get to the next room.

\--- task \--- `キー` スプライトに切り替えます。 スクリプトメニューの `show`{：class = "blocklooks"}をクリックすると、スプライトがステージに表示されます。 \--- /task \---

\--- task \--- `key` スプライトのコスチュームを青になるように編集します。 \--- /task \---

\--- task \--- ステージの背景を部屋3に切り替え、 `キー` スプライトを届きにくい場所に配置します。

![screenshot](images/world-key.png)

\--- /task \---

\--- task \--- `key` スプライトにコードを追加して、部屋3でのみ見えるようにします。 \--- /task \---

\--- task \--- `inventory`{：class = "block3variables"}という名前の新しいリストを作り、あなたの `プレイヤー` スプライトが集めるアイテムを保存します。

[[[generic-scratch3-make-list]]] \--- / task \---

\--- task \--- キーを集めるために追加する必要があるコードはコインを集めるためのコードと非常によく似ています。 違いは、 `在庫`キーを追加することです</code> {：class = "block3variables"}。

![キー](images/key.png)

```blocks3
フラグがクリックされたとき
 <touching (player v)?>まで待つ
[インベントリv]に[青い鍵]を追加
非表示
停止[スプライトvの他のスクリプト]
```

\--- /task \---

\--- task \--- ゲームの開始時にあなたの持ち物を空にするためにあなたのステージにコードを追加します。

```blocks3
[inventory v]の削除（すべてv）
```

\--- /task \---

\--- task \--- `キー` スプライトを集めてあなたのインベントリに追加できるかどうかチェックするためにあなたのゲームをテストしてください。 \--- /task \---

\--- task \--- 今度は鍵付きドアを追加します。 `ドアブルー` スプライトを選択し、スクリプトメニューの `show`{：class = "blocklooks}をクリックしてから、2つの壁の間の隙間にスプライトを配置します。

![スクリーンショット](images/world-door.png) \--- /task \---

\--- task \--- `ドア青` スプライトにコードを追加して、部屋3にのみ見えるようにします。 \--- /task \---

\--- task \--- `ドアブルー` スプライトにコードを追加して、キーが `インベントリ`にあるときにスプライト `が`{：class = "block3looksを隠すようにあなたの `プレイヤー` スプライトが通過することを可能にするために "}。

![ドア](images/door.png)

```blocks3
フラグがクリックされたとき
 <[在庫v]に[ブルーキー]が含まれるまで待つ？>
停止[スプライトvの他のスクリプト]
隠す
```

\--- /task \---

\--- task \--- あなたのゲームを試して、ドアを開けるための青い鍵を集めることができるかどうか確認してください！ \--- /task \---