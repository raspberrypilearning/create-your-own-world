## 收集硬币

你的 `玩家` 精灵应该能够收集硬币在世界各地移动。

\--- task \--- 为你的项目添加一个新的变量valled `coins`{：class =“block3variables”}。 \--- /task \---

\---任务\--- 选择 `硬币` 精灵，然后单击 **显示**。

![截屏](images/coin.png) \--- /task \---

\---任务\--- 将代码添加到 `硬币` 精灵中，使其仅出现在房间1中。 ![截屏](images/coin.png)

```blocks3
当标志点击
永远
如果 <（房间::变量）=[1]> 然后
显示
其他
隐藏
```

\--- /task \---

\--- task \---

将代码添加到 `硬币` 精灵中，以便精灵 `隐藏`{：class =“block3looks”}并将 `1`{：class =“block3variables”}添加到 `硬币`{：class =“block3variables”}变量一旦 `玩家` 精灵触及 `硬币` 精灵来“捡起来”。

![硬币](images/coin.png)

```blocks3
当标志点击
等待直到 <touching (player v)?>
更改[硬币v]由（1）
隐藏
停止[其他脚本在精灵v]
```

代码 `停止精灵`{：class =“block3control”}中的其他脚本是必要的，以便 `硬币` 精灵在收集后停止在房间1中显示。

\--- /task \---

\--- task \--- 现在在舞台上添加代码，在游戏开始时将 `硬币`{：class =“block3variables”}变量设置为 `0`{：class =“block3variables”}。

![阶段](images/stage.png)

```blocks3
当标记点击
将[硬币v]设置为 [0]
```

\--- /task \---

\---任务\--- 测试你的游戏。 收集硬币应该将你的 `硬币` 分改为 `1`{：class =“block3variables”}。 \--- /task \---