## 단단한 벽

--- task ---

`플레이어` 스프라이트를 다시 테스트해보세요. 밝은 회색 벽을 통과 할 수 있다는 것을 볼 수 있나요?

![스크린샷](images/world-walls.png)

--- /task ---

--- task ---

이것을 고치기 위해서는, `플레이어` 스프라이트가 밝은 회색 벽에 닿으면 뒤로 물러나게끔 해야 합니다. 방향 블록 아래에 있는 `무한 반복하기` 블록 안에 추가해야 할 코드는 다음과 같습니다:

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
        if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

--- /task ---

--- task ---

`플레이어` 스프라이트가 벽을 통과하게끔 시도해보세요. 만약에 새로 작성한 코드가 잘 작동한다면, 이것이 불가능할 것입니다.

![스크린샷](images/world-walls-test.png)

--- /task ---