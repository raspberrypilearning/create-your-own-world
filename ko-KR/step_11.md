## 문과 열쇠

이제 게임에서 일부 문이 잠기도록 코드를 추가할 것입니다. 지금부터 플레이어는 열쇠를 찾아 문을 열은 후 다음 방으로 가야 합니다.

--- task ---

`열쇠` 스프라이트를 클릭합니다. 그리고 스크립트 메뉴의 `보이기`{:class="blocklooks"}를 클릭하여 무대에 나타나게 합니다.

--- /task ---

--- task ---

`열쇠` 스프라이트의 색상이 파란색이 되도록 합니다.

--- /task ---

--- task ---

무대 배경을 방3으로 바꾼 다음, `열쇠` 스프라이트를 다가가기 어려운 위치에 놓아보세요!

![스크린샷](images/world-key.png)

--- /task ---

--- task ---

`열쇠` 스프라이트에 코드를 추가하여 방3에서만 나타나게 해보세요.

--- /task ---

--- task ---

`플레이어` 스프라이트가 수집하는 아이템들을 저장할 수 있는 `아이템 목록`{:class="block3variables"}이라는 새 리스트를 만듭니다.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

열쇠를 수집하기 위해 추가해야 하는 코드는 동전을 수집하는 코드와 매우 비슷합니다. 차이점은 열쇠를 `아이템 목록`{:class="block3variables"}에 추가해야 한다는 것입니다.

![열쇠](images/key.png)

```blocks3
when flag clicked
wait until <touching (동전 개수 v)?>
add [파란색 열쇠] to [아이템 목록 v]
hide
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

무대에 코드를 추가하여 게임 시작 시 아이템 목록을 초기화하게 해봅시다.

```blocks3
delete (all v) of [아이템 목록 v]
```

--- /task ---

--- task ---

게임을 테스트하여 `열쇠` 스프라이트를 수집하여 아이템 목록에 추가할 수 있는지 확인하세요.

--- /task ---

--- task ---

이제 잠긴 문을 추가하세요. `문-파란색` 스프라이트를 선택하고 스크립트 메뉴의 `보이기`{:class="blocklooks}를 클릭하고, 두 벽 사이의 공간에 스프라이트를 위치시키세요.

![스크린샷](images/world-door.png)

--- /task ---

--- task ---

`문-파란색` 스프라이트에 코드를 추가하여 방3에서만 나타나게 해보세요.

--- /task ---

--- task ---

`문-파란색` 스프라이트에 코드를 추가하여, 열쇠가 `아이템 목록`{:class="block3variables"}에 있을 때 스프라이트가 `숨기기`{:class="block3looks"} 되어 `플레이어` 스프라이트가 지나갈 수 있게 합니다.

![문](images/door.png)

```blocks3
when flag clicked
wait until <[아이템 목록 v] contains [파란색 열쇠]?>
stop [other scripts in sprite v]
hide
```

--- /task ---

--- task ---

게임을 테스트하고 파란색 열쇠를 수집하여 문을 열 수 있는지 확인해보세요!

--- /task ---