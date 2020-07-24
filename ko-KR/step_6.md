## 표지판

이제 표지판을 추가해 플레이어에게 여행을 안내해봅시다.

이 프로젝트는 `환영 표지판` 스프라이트를 포함합니다.

![스크린샷](images/world-sign.png)

\--- task \---

`환영 표지판` 스프라이트가 방1에서만 나타나도록 해당 스트라이트에 코드를 약간 추가합니다:

\--- hints \---

\--- hint \---

`깃발이 클릭되었을 때`{:class="block3events"}, `무한반복`{:class="block3control"} 루프 내에서, `만약`{:class="block3control"} `방 번호가 1`{:class="block3variables"} 이면 `환영 표지판` 스프라이트가 `보이기`{:class="block3looks"} 되고 `만약 아니라면`{:class="block3control"} 스프라이트가 `숨기기`{:class="block3looks"} 되는지 확인하세요.

\--- /hint \---

\--- hint \---

필요한 블록은 다음과 같습니다.

![표지판](images/sign.png)

```blocks3
<br />if < > then
else
end

< (room :: variables) = [1] >

hide

show

forever
end

when flag clicked

```

\--- /hint \---

\--- hint \---

완성된 코드는 다음과 같습니다:

![표지판](images/sign.png)

```blocks3
when flag clicked
forever
    if < (room :: variables) = [1] > then
        show
    else
        hide
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

방 사이를 이동해 다니면서 `환영 표지판` 스프라이트 코드를 테스트해 보세요. 해당 표지판은 방1에서만 보여야 합니다.

![스크린샷](images/world-sign-test.png)

\--- /task \---

\--- task \---

표지판이 아무 말도 하지 않는다면 썩 양호하다고 할 수는 없겠죠! 코드를 좀 더 추가해 `환영 표지판` 스프라이트가 `플레이어` 스프라이트에 닿을 때 메세지가 표시되도게 합니다:

![표지판](images/sign.png)

```blocks3
when flag clicked
forever
if < (room :: variables) = [1] > then
show
else
hide
end
+if < touching (player v)? > then
say [Welcome! Can you get to the treasure?]
else
say []
end
end
```

\--- /task \---

\--- task \---

`환영 표지판` 스트라이트를 다시 한번 테스트해보세요. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![스크린샷](images/world-sign-test2.png)

\--- /task \---