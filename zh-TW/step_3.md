## 堅固的牆壁

--- task ---

再測試你的`玩家`角色。 你觀察到了嗎？它可以穿過淺灰色的牆壁…這一點也不科學！

![截圖](images/world-walls.png)

--- /task ---

--- task ---

要解決這個問題，你必須讓`玩家`角色在碰到淺灰色牆壁時，讓它彈回來。 請把這個程式添加到`重複無限次`{:class="block3control"}區段中面朝方向積木的下面：

![玩家](images/player.png)

```blocks3
when flag clicked
forever
	if <key (向上 v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (向左 v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
		if <key (向下 v) pressed? > then
		point in direction (-180)
		move (4) steps
	end
		if <key (向右 v) pressed? > then
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

試著讓`玩家`角色經過牆壁。 如果新的程式有用的話，它應該不能再穿牆而過了。

![截圖](images/world-walls-test.png)

--- /task ---