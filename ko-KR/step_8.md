## 새로운 사람

`플레이어` 스프라이트와 상호작용할 수 있는 다른 사람들을 추가해봅시다.

\--- task \---

`사람` 스프라이트를 클릭합니다.

![사람 스프라이트](images/person.png)

\--- /task \---

\--- task \---

`사람` 스프라이트에 코드를 추가하여 `플레이어` 스프라이트에게 말을 걸게 해봅시다. 이것은 `표지판` 스프라이트에 추가했던 코드와 매우 비슷합니다:

![사람](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
    end
end
```

\--- /task \---

\--- task \---

다음 두 블록을 `아니라면` 부분에 추가하여 `사람` 스프라이트가 움직일 수 있게끔 합니다:

![사람](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
+       move (1) steps
+       if on edge, bounce
    end
end
```

\--- /task \---

`사람` 스프라이트는 이제 움직이면서도, `플레이어`와 이야기하기 위해서는 멈춰설 것입니다.

![스크린샷](images/world-person-test.png)

\--- task \---

`사람` 스프라이트에 코드를 추가하여 스프라이트가 방1에서만 나타나게 해보세요. 이것에 필요한 코드는 `표지판` 스프라이트가 방1에서만 보이게 하는 코드와 정확히 동일합니다.

새 코드를 반드시 테스트해보세요.

\--- /task \---