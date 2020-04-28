## 플레이어 스프라이트 움직이기

맵에서 움직일 수 있는 `플레이어` 스프라이트를 만들어 시작해봅시다.

--- task ---

'나만의 세계 만들기' 스크래치 스타터 프로젝트를 엽니다.

**온라인:** [scratch.mit.edu/projects/389820598](https://scratch.mit.edu/projects/389820598){:target="_blank"}에서 새로운 스타터 프로젝트를 열어주세요.

스크래치 계정이 있는 경우 **Remix를 클릭** 하여 사본을 만들 수 있습니다.

**오프라인:** 오프라인 시작 프로그램을 [rpf.io/p/ko-KR/create-your-own-world-go](http://rpf.io/p/ko-KR/create-your-own-world-go){:target="_blank"} 에서 다운로드하고, 오프라인 에디터로 파일을 엽니다. 스크래치 오프라인 에디터를 다운로드 받아야 하는 경우, [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}에서 파일을 다운로드할 수 있습니다.

![스크린샷](images/world-starter.png)

--- /task ---

화살표 키를 누르면 `플레이어` 스프라이트가 움직여야 합니다. 위 화살표를 누르면, `플레이어` 스프라이트가 반응하여 위로 움직일 것입니다.

--- task ---

`플레이어` 스프라이트에 다음 코드를 추가하세요:

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

--- /task ---

--- task ---

플래그를 클릭한 후 위 화살표를 길게 눌러보세요. `플레이어` 스프라이트가 위로 움직이나요?

![스크린샷](images/world-up.png)

--- /task ---

--- task ---

`플레이어` 스프라이트를 왼쪽으로 움직이고 싶다면, 비슷한 코드를 가진 또 다른 `만약 ( ) (이)라면`{:class="block3control"} 블록을 추가해야 합니다.

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

--- /task ---

--- task ---

`플레이어` 스프라이트에 더 많은 코드를 추가하여 위 아래로도 움직일 수 있게 해봅시다. 지금 가지고 있는 코드를 활용해보세요.

--- hints ---


--- hint ---

위로 움직이고 싶다면, `플레이어` 스프라이트를 `0`도 방향으로 향하게 합니다. 스프라이트를 아래로 움직이기 위해서는 무엇을 해야 하나요?

왼쪽으로 움직이고 싶다면, 스프라이트를 `-90`도 방향으로 향하게 합니다. 오른쪽으로 움직이기 위해서는 무엇을 해야 하나요?

--- /hint ---

--- hint ---

다음 두 블록을 수정해야 합니다:

![플레이어](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

`플레이어` 스프라이트를 위로 움직이게 하는 코드를 복제하고, 이 두 블록을 스프라이트가 아래로 움직이게 수정합니다. 다시 코드를 복제한 후, 스프라이트가 오른쪽으로 움직이게 수정합니다.

--- /hint ---

--- hint ---

코드는 다음과 같이 설계되어야 합니다:

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

--- /hint ---

--- /hints ---

--- /task ---