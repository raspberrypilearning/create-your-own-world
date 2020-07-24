## 도전 과제: 적 추가하기

원한다면 주변을 순찰하는 적을 추가할 수도 있습니다. `플레이어` 스프라이트가 적과 닿으면 게임은 종료됩니다.

+ 게임에는 `적` 스프라이트가 포함되어 있습니다. `적` 스프라이트에 코드를 추가해 그것이 방2에만 나타나게 합니다.

+ 코드를 추가해 `적` 스프라이트가 움직이고 `적` 스프라이트가 `플레이어` 스프라이트에 닿으면 게임이 종료되게 합니다. 분리된 코드 블럭으로 진행하는 게 보다 용이합니다. `적` 스프라이트 코드는 다음과 같습니다:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
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

+ 새 코드를 테스트해 다음을 확인합니다: 
    + `적` 스프라이트는 방2에서만 보인다
    + `적` 스프라이트는 해당 방을 돌아다닌다
    + `플레이어` 스프라이트가 `적` 스프라이트에 닿으면 게임이 종료된다

방 3에서 벽의 틈 사이를 통해 위 아래로 지나다니는 `적` 스프라이트를 추가적으로 만들 수 있나요?

![스크린샷](images/world-enemy2.png)