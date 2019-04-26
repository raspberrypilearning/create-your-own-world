## 收集硬幣

你的 `玩家` 精靈應該能夠收集硬幣在世界各地移動。

\--- task \--- 為你的項目添加一個新的變量valled `coins`{：class =“block3variables”}。 \--- /任務\---

\--- task \--- Select the `coin` sprite and click **show**.

![截圖](images/coin.png) \--- /任務\---

\---任務\--- 將代碼添加到 `硬幣` 精靈中，使其僅出現在房間1中。 ![截圖](images/coin.png)

```blocks3
當標誌點擊
永遠
如果 <（房間::變量）=[1]> 然後
顯示
其他
隱藏
```

\--- /任務\---

\---任務\---

將代碼添加到 `硬幣` 精靈中，以便精靈 `隱藏`{：class =“block3looks”}並將 `1`{：class =“block3variables”}添加到 `硬幣`{：class =“block3variables”}變量一旦 `玩家` 精靈觸及 `硬幣` 精靈來“撿起來”。

![硬幣](images/coin.png)

```blocks3
當標誌點擊
等待直到 <touching (player v)?>
更改[硬幣v]由（1）
隱藏
停止[其他腳本在精靈v]
```

代碼 `停止精靈`{：class =“block3control”}中的其他腳本是必要的，以便 `硬幣` 精靈在收集後停止在房間1中顯示。

\--- /任務\---

\--- task \--- 現在在舞台上添加代碼，在遊戲開始時將 `硬幣`{：class =“block3variables”}變量設置為 `0`{：class =“block3variables”}。

![階段](images/stage.png)

```blocks3
當標記點擊
將[硬幣v]設置為 [0]
```

\--- /任務\---

\---任務\--- 測試你的遊戲。 收集硬幣應該將你的 `硬幣` 分改為 `1`{：class =“block3variables”}。 \--- /任務\---