## 맵 안에서 이동하기

`플레이어` 스프라이트는 문을 통과하여 다른 방으로 걸어 들어갈 수 있어야 합니다.

이 프로젝트에는 추가적인 방들에 대한 배경이 제공됩니다.

![스크린샷](images/world-backdrops.png)

\--- task \---

'모든 스프라이트에서 사용'할 수 있는 변수 `방 번호`를 만들어 `플레이어` 스프라이트가 어느 방에 있는 지를 추적해봅시다.

[[[generic-scratch3-add-variable]]]

![스크린샷](images/world-room.png)

\--- /task \---

\--- task \---

`플레이어` 스프라이트가 첫번째 방의 주황색 문에 닿으면, 게임은 다음 배경을 보여주어야 하고, `플레이어` 스프라이트는 다시 무대의 왼쪽으로 돌아가야 합니다. `플레이어` 스프라이트의 `무한 반복하기`{:class="block3control"} 블록 안에 다음 코드를 추가합니다:

![플레이어](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
+   if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
    end
end
```

\--- /task \---

\--- task \---

게임이 시작될 때마다 방, 캐릭터 위치, 배경이 초기화되어야 합니다.

플래그를 클릭했을 때 모든 것이 초기화되게끔 `플레이어` 스프라이트의 **시작** 부분에서 `무한 반복하기`{:class="block3control"} 블록을 찾아, 그 윗부분에 다음 코드를 추가하세요:

\--- hints \---

\--- hint \---

게임이 시작되면:

+ `방 번호` 변수의 값이 `1`로 설정되어야 합니다.
+ `배경`{:class="block3looks"}은 `방1`로 설정되어야 합니다.
+ `플레이어` 스프라이트의 위치가 `x: -200 y: 0`{:class="block3motion"}로 설정되어야 합니다.

\--- /hint \---

\--- hint \---

추가로 필요한 블록은 다음과 같습니다:

![플레이어](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

\--- /hint \---

\--- hint \---

완성된 코드는 다음과 같아야 합니다:

![플레이어](images/player.png)

```blocks3
when flag clicked
+set [room v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to (room1 v)
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
    if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

깃발을 클릭한 후, `플레이어` 스프라이트가 주황색 문에 닿을 때까지 움직입니다. 스프라이트가 다음 화면으로 넘어가나요? `방 번호`{:class="block3variables"} 변수가 `2`로 변하나요?

![스크린샷](images/world-room-test.png)

\--- /task \---