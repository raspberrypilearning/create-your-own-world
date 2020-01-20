## 收集硬幣

你的 `玩家` 精靈應該能夠收集硬幣在世界各地移動。

\--- task \---

Add a new variable valled `coins`{:class="block3variables"} to your project.

\--- /任務\---

\--- task \---

Select the `coin` sprite and click **show**.

![screenshot](images/coin.png)

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that it only appears in room 1.

![screenshot](images/coin.png)

```blocks3
當標誌點擊
永遠
如果 <（房間::變量）=[1]> 然後
顯示
其他
隱藏
```

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
當標誌點擊
等待直到 <touching (player v)?>
更改[硬幣v]由（1）
隱藏
停止[其他腳本在精靈v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \---

Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
當標記點擊
將[硬幣v]設置為 [0]
```

\--- /task \---

\--- task \---

Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.

\--- /task \---