## 동전 모으기

`플레이어` 스프라이트는 맵을 지나다니며 동전을 수집 할 수 있어야 합니다.

\--- task \---

프로젝트에 `동전`{:class="block3variables"} 이라는 새로운 변수를 추가합니다.

\--- /task \---

\--- task \---

`동전` 스프라이트를 클릭 후 **보이기** 를 선택합니다.

![스크린샷](images/coin.png)

\--- /task \---

\--- task \---

`동전` 스프라이트에 코드를 추가해 방1에만 나타나도록 합니다.

![스크린샷](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

`동전` 스프라이트에 코드를 추가해 해당 스프라이트가 `숨기기`{:class="block3looks"} 되며 `플레이어` 스프라이트가 '동전을 줍기 위해' `동전` 스프라이트에 닿으면 `동전`{:class="block3variables"} 변수에 `1`{:class="block3variables"} 이 추가되게 합니다.

![동전](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

동전을 일단 줍게 되면 `동전` 스프라이트가 방1에 보이는 걸 중단하기 위해 `스프라이트 내 기타 스크립트 중지`{:class="block3control"} 코드가 필요합니다.

\--- /task \---

\--- task \---

이제 스테이지에 코드를 추가해 게임 시작 시 `동전`{:class="block3variables"} 변수가 `0`{:class="block3variables"} 이 되게 설정합니다.

![스테이지](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

게임을 테스트해보세요. 동전을 줍게 되면 `동전` 스코어가 `1`{:class="block3variables"} 로 바뀌어야 합니다.

\--- /task \---