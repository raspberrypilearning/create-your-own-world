## 課題：あなたの世界を広げる

You can now continue creating your own world! Here are some ideas:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Add sound and music to your game
+ Add more people, enemies, and signs
+ Add red and yellow doors, and special keys to open them
+ Add more rooms to your world
+ Add other useful items to your game
    
    + Use coins to get information from other people:

![screenshot](images/world-bribe.png)

+ 部屋1の北と南の壁にドアを追加することもでき、プレイヤーは4方向すべての部屋を移動できます。 For example, your game can have nine rooms in a 3×3 grid. 部屋番号に `3` を追加して1つ下の階層に移動できます。

![スクリーンショット](images/north-south-rooms.png) ![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```