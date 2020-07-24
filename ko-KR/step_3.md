## 단단한 벽

\--- task \---

`플레이어` 스프라이트를 다시 테스트해보세요. Do you see that it can walk through the light grey walls?

![스크린샷](images/world-walls.png)

\--- /task \---

\--- task \---

이것을 고치려면 `플레이어` 스프라이트가 밝은 회색 벽에 닿을 때 뒤로 물러나게 해야 합니다. 방향 블록 아래의 `무한반복` 블록 내 추가할 코드는 다음과 같습니다:

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

\--- /task \---

\--- task \---

`플레이어` 스프라이트가 벽을 통과하게 해보세요. If your new code works, this shouldn't be possible.

![스크린샷](images/world-walls-test.png)

\--- /task \---