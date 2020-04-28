## 코인 모으기

`플레이어` 스프라이트는 맵을 통과하면서 동전을 수집 할 수 있어야 합니다.

--- task ---

프로젝트에 `동전 개수`{:class="block3variables"}라는 새로운 변수를 추가합니다.

--- /task ---

--- task ---

`동전` 스프라이트를 클릭한 후 **보이기**를 클릭합니다.

![스크린샷](images/coin.png)

--- /task ---

--- task ---

`동전` 스프라이트에 코드를 추가하여 방1에서만 나타나게 해보세요.

![스크린샷](images/coin.png)

```blocks3
when flag clicked
forever
if <(방 번호 :: variables)=[1]> then
show
else
hide
```

--- /task ---

--- task ---

`플레이어` 스프라이트가 `동전`에 닿으면 동전을 `숨기기`{:class="block3looks"}하고 `동전 개수`{:class="block3variables"} 변수에 `1`{:class="block3variables"}이 추가되게끔 하여 `플레이어`가 <0>동전</0>을 '주울 수 있도록' 코드를 추가해봅시다.

![동전](images/coin.png)

```blocks3
when flag clicked
wait until <touching (플레이어 v)?>
change [동전 개수 v] by (1)
hide
stop [other scripts in sprite v]
```

`이 스프라이트에 있는 다른 스크립트`{:class="block3control"}라는 코드는 `동전` 스프라이트가 주워진 이후 방1에서 표시되지 않게 하기 위해 필요합니다.

--- /task ---

--- task ---

이제 무대에 코드를 추가하여 게임이 시작되면 `동전 개수`{:class="block3variables"} 변수가 `0`이 되게 코드를 추가해보세요.

![무대](images/stage.png)

```blocks3
when flag clicked
set [동전 개수 v] to [0]
```

--- /task ---

--- task ---

게임을 테스트해보세요. 동전을 모으면 `동전 개수`가 `1`{:class="block3variables"}로 바뀔 것 입니다.

--- /task ---