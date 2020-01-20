## 标志

现在为您的世界添加标志，以指导玩家的旅程。

您的项目包含 `欢迎标志` 精灵：

![screenshot](images/world-sign.png)

\--- task \---

The `welcome sign` sprite should only be visible in room 1, so add some code to the sprite to make sure that this happens:

\--- hints \---

\--- hint \---

`When the flag is clicked`{:class="block3events"}, in a `forever`{:class="block3control"} loop, check `if`{:class="block3control"} the `room is 1`{:class="block3variables"} and in that case `show`{:class="block3looks"} `welcome sign` sprite, `else`{:class="block3control"} `hide`{:class="block3looks"} the sprite.

\--- /hint \---

\--- hint \---

Here are the blocks you need:

![sign](images/sign.png)

```blocks3
<br />if < > then
else
end

< （room :: variables）= [1] >

hide

show

forever
end

when flag clicked

```

\--- /hint \---

\--- hint \---

Here is the complete code:

![sign](images/sign.png)

```blocks3
当标志点击
永远
    如果 < （房间::变量）= [1] > 然后
        显示
    其他
        隐藏
    结束
结束
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Test the code for your `welcome sign` sprite by moving between rooms. The sign should only be visible in room 1.

![screenshot](images/world-sign-test.png)

\--- /task \---

\--- task \---

A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

```blocks3
当标志点击
永远
如果 < （房间::变量）= [1] > 然后
显示
否则
隐藏
结束
+如果 < 触摸（玩家v）？ > 然后
说[欢迎！ 你能得到宝藏吗？]
其他
说[]
结束
结束
```

\--- /task \---

\--- task \---

Test your `welcome sign` sprite again. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![screenshot](images/world-sign-test2.png)

\--- /task \---