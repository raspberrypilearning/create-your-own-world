## 코인 모으기

`플레이어` 스프라이트는 세계를 통과하면서 동전을 수집 할 수 있어야합니다.

\--- task \---

Add a new variable valled `coins`{:class="block3variables"} to your project.

\--- /task \---

\--- task \---

Select the `coin` sprite and click **show**.

![screenshot](images/coin.png)

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that it only appears in room 1.

![screenshot](images/coin.png)

```blocks3
flag를 클릭했을때
영원히
만약 <(방 :: 변수)=[1]> 그러면
보여주기
else
숨기기
```

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
flag클릭 시
기다리기 <touching (player v)?>
[coins v] 를 (1) 로 바꾸기
숨기기
[스프라이트v의 다른 스크립트들] 멈추기
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \---

Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
flag 클릭했을 때
[coins v] 를 [0] 으로 설정하기
```

\--- /task \---

\--- task \---

Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.

\--- /task \---