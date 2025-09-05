## 收集硬币

你的 `玩家` 子图在探索世界的同时，还可以收集硬币。

\--- task \---

向你的项目添加一个名为 `硬币`{:class="blockdata"}的新变量。

\--- /task \---

\--- task \---

右键点击 `硬币` 子图并选择 **显示**。

![截屏](images/coin.png)

\--- /task \---

\--- task \---

向你的 `硬币` 子图添加代码使其仅出现在房间 1 内。

![截屏](images/coin.png)

```blocks3
当绿旗被点击
重复执行
如果 <(room :: variables)=[1]> 那么
显示
否则
隐藏
```

\--- /task \---

\--- task \---

向你的 `硬币` 子图添加代码，从而在 `玩家` 子图触碰到 `硬币` 子图将其“拾取”时，`硬币`{:class="blockdata"}变量便会增加 `1`。

![images/world-coins.png](images/coin.png)

```blocks3
当旗帜被点击
等待直到 <touching (player v)?>
将[coins v]增加 (1)
隐藏
停止[该角色的其他脚本]
```

需要 `停止子图中的其他脚本`{:class="blockcontrol"} 代码，这样在收集硬币后，`硬币` 子图将停止在房间 1 中显示。

\--- /task \---

\--- task \---

你还将需要添加代码。以在游戏开始时将你的 `硬币`{:class="blockdata"}变量设为 `0`。

![舞台](images/stage.png)

```blocks3
当绿旗被点击
将 [硬币] 设为 [0]
```

\--- /task \---

\--- task \---

测试你的游戏。 向你的项目添加一个名为 `硬币`{:class="blockdata"}的新变量。

\--- /task \---