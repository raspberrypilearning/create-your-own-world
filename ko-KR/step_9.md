## 도전 과제: 적 추가하기

원한다면 주변을 순찰하는 적을 추가할 수도 있습니다. `플레이어` 스프라이트가 적에게 닿는다면, 게임이 끝납니다.

+ 이 게임에는 `적` 스프라이트가 포함되어 있습니다. `적` 스프라이트에 코드를 추가하여 방2에서만 나타나게 해보세요.

+ 코드를 추가하여 `적` 스프라이트가 움직이게 하고 `적` 스프라이트가 `플레이어` 스프라이트와 닿으면 게임이 끝나게 해보세요. 이것은 분리된 코드 블럭에서 진행하면 더 쉽습니다. `적` 스프라이트의 코드는 다음과 같아야 할 것입니다:

```blocks3
when flag clicked
forever
if <(방 번호 :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (플레이어 v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ 다음을 테스트해보세요: 
    + `적` 스프라이트는 오직 방2에서만 보인다
    + `적` 스프라이트는 방을 순찰한다
    + `플레이어` 스프라이트가 `적` 스프라이트에 닿으면 게임이 종료된다

방3에서 벽면 사이의 공간에서 위 아래로 순찰하는 또 다른 `적` 스프라이트를 만들어볼 수 있나요?

![스크린샷](images/world-enemy2.png)