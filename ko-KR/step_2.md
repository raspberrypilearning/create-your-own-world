## 플레이어 스프라이트 움직이기

맵에서 움직일 수 있는 `플레이어` 스프라이트를 만들어 시작해봅시다.

\--- task \---

'나만의 세계 만들기' 스크래치 스타터 프로젝트를 엽니다.

**Online**: open the online starter project at [rpf.io/create-your-own-world-on](https://rpf.io/create-your-own-world-on){:target="_blank"}.

스크래치 계정이 있는 경우 **Remix** 를 클릭하여 사본을 만들 수 있습니다.

**Offline**: download the starter project [rpf.io/p/en/create-your-own-world-go](https://rpf.io/p/en/create-your-own-world-go){:target="_blank"}, and then open it using the offline editor. 스크래치 오프라인 에디터 다운로드 및 설치는 [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"} 에서 합니다.

![스크린샷](images/world-starter.png)

\--- /task \---

화살표 키를 누르면 `플레이어` 스프라이트가 움직여야 합니다. 위 방향 화살표를 누르면 `플레이어` 스프라이트가 위로 움직여야 합니다.

\--- task \---

`플레이어` 스프라이트에 다음의 코드를 추가하세요:

![플레이어](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

플래그 클릭 후 위 방향 화살표를 길게 눌러보세요. `플레이어` 스프라이트가 위로 움직이나요?

![스크린샷](images/world-up.png)

\--- /task \---

\--- task \---

`플레이어` 스프라이트를 왼쪽으로 움직이려면 비슷한 코드를 담은 `만약`{:class="block3control"} 블록을 추가해야 합니다.

![플레이어](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

`플레이어` 스프라이트에 코드를 좀 더 추가해 아래 방향과 우측으로 움직이도록 해봅시다. 가지고 있는 코드를 활용해보세요.

\--- hints \---

\--- hint \---

위로 움직이기 위해 `플레이어` 스프라이트를 `0`도 방향으로 향하게 합니다. 스프라이트를 아래로 움직이기 위해서는 무엇을 해야 하나요?

왼쪽으로 움직이고 싶다면 스프라이트를 `-90`도 방향으로 향하게 합니다. 스프라이트를 오른쪽으로 움직이기 위해 무엇을 해야 하나요?

\--- /hint \---

\--- hint \---

다음 두 블록을 수정해야 합니다:

![플레이어](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

`플레이어` 스프라이트를 위 방향으로 움직이게 하는 코드를 복사하고 이 두 블록을 변경하여 스프라이트가 아래로 움직이도록 합니다. 다시 코드를 복사 후 변경하여 스프라이트가 오른쪽으로 움직이도록 합니다.

\--- /hint \---

\--- hint \---

코드는 다음과 같아야 합니다:

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

+    if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
+    if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---