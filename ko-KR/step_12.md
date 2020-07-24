## 도전 과제: 나만의 세계 넓히기

이제 나만의 세상을 계속 만들어 나갈 수 있습니다! 다음은 몇 가지 아이디어입니다.

+ 여러 방마다 게임에 동전을 더 추가합니다. 적을 순찰하는 방법으로 동전을 지킬 수 있나요?
+ 게임 배경을 변경합니다
+ 게임에 사운드와 음악을 추가합니다
+ 사람, 적, 표지판을 더 많이 추가합니다.
+ 빨간색과 노란색 문을 비롯해 이를 열기 위한 특별 열쇠를 추가합니다.
+ 맵에 방을 더 많이 추가합니다.
+ 개임에 기타 유용한 아이템을 추가합니다.
    
    + 동전을 사용해 다른 사람으로부터 정보를 얻습니다:

![스크린샷](images/world-bribe.png)

+ 심지어 방1의 북쪽과 남쪽 벽에 문을 추가해 플레이어가 전체 4가지 방향으로 방 사이를 이동하도록 할 수 있습니다. 예를 들어 3x3 그리드 내 9개 방이 형성될 수 있습니다. You can then add `3` to the room number to move down one level.

![스크린샷](images/north-south-rooms.png)

![스크린샷](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```