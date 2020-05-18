## 在你的世界逛逛

`玩家`角色應該要能通過門進入其它的空間。

你的專案包含了其它空間的背景：

![截圖](images/world-backdrops.png)

--- task ---

創建一個「適用於所有角色」的變數，名稱叫做`空間`{:class="block3variables"}，用這個變數來紀錄`玩家`走到了哪個空間。

[[[generic-scratch3-add-variable]]]

![截圖](images/world-room.png)

--- /task ---

--- task ---

當`玩家`角色碰到了第一個空間裡的橙色門，遊戲應該要顯示下一個背景，`玩家`應該被定位到舞台的最左邊。 為`玩家`角色添加程式到`重複無限次`{:class="block3control"}迴圈裡：

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
	if < touching color [#BABABA]? > then
	move (-4) steps
	end
+	if < touching color [#F2A24A] > then
	switch backdrop to (下一個背景 v)
	go to x: (-200) y: (0)
	change [空間 v] by (1)
	end
end
```

--- /task ---

--- task ---

每次遊戲的一開始，角色所處空間、角色的位置、背景都要重新設置。

把**初始**的程式添加到`玩家`角色的`重複無限次`{:class="block3control"}積木上面，這樣一來，當點擊綠旗時，所有東西都會被重置。

--- hints ---


--- hint ---

當遊戲開始運行時：

+ `空間`{:class="block3variables"}的值應該設定為 `1`{:class="block3variables"}
+ `背景`{:class="block3looks"}應該被設定成 `空間1`{:class="block3looks"}
+ `玩家`角色的位置應該設定為 `x: -200 y: 0`{:class="block3motion"}

--- /hint ---

--- hint ---

這裡是你需要的程式積木：

![玩家](images/player.png)

```blocks3
定位到 x:(-200) y:(0)

變數 [空間 v] 設為 (1)

背景換成 (空間1 v)
```

--- /hint ---

--- hint ---

你的程式看起來應該像這樣：

![玩家](images/player.png)

```blocks3
when flag clicked
+set [空間 v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to (空間1 v)
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
	if < touching color [#BABABA]? > then
	move (-4) steps
	end
	if < touching color [#F2A24A] > then
	switch backdrop to (下一個背景 v)
	go to x: (-200) y: (0)
	change [空間 v] by (1)
end
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

點擊綠旗，移動`玩家`到橙色門那邊，碰一下門。 如何，角色進入下一個畫面了嗎？ 變數`空間`{:class="block3variables"}的值變成 `2` 了嗎？

![截圖](images/world-room-test.png)

--- /task ---