## 移动 `玩家` 子图

\--- task \---

再次测试您的 `玩家` 角色。 Do you see that it can walk through the light grey walls?

![截图](images/world-walls.png)

\--- /task \---

\--- task \---

要解决这个问题，你需要让 `玩家` 角色判断，如果碰到浅灰色的墙，则将它移回。 为使 `玩家` 子图向左移动，你需要添加另一个 `如果`{:class="blockcontrol"}代码块，代码类似于：

![玩家](images/player.png)

```blocks3
当绿旗被点击
重复执行
    如果 < 按下 (向上箭头) 键? > 那么
        面向 (0) 方向
        移动 (4) 步
    结束
    如果 <按下 (向左箭头) 键？ > 那么
        面向 (-90) 方向
        移动 (4) 步
    结束
        如果 <按下 (向下箭头) 键？ > then
        point in direction (180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > 那么
        面向 (90) 方向
        移动 (4) 步
    结束
+ 如果 < 碰到颜色 [#BABABA]？ > 那么
    移动 (-4) 步
    结束
结束
```

\--- /task \---

\--- task \---

向你的 `玩家` 子图添加更多代码，使其能向下和向右移动。运用你已有的代码来帮你。 如果您的新代码有效，那应该玩家应该不会穿过墙壁。

![截图](images/world-walls-test.png)

\--- /task \---