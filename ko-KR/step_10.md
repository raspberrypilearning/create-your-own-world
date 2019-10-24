## 코인 모으기

`플레이어` 스프라이트는 세계를 통과하면서 동전을 수집 할 수 있어야합니다.

\--- task \--- 새로운 변수 `코인`{: class = "block3variables"} 을 프로젝트에 추가하세요. \--- /task \---

\--- task \--- `코인` 스프라이트를 클릭하고 **보여주기**를 클릭하세요.

![스크린샷](images/coin.png) \--- /task \---

\--- task \--- 당신의 코드를 `코인` 스프라이트에 방1 에서만 나타나도록 추가하세요. ![스크린샷](images/coin.png)

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

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

\--- /task \---

\--- task \--- Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \--- Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}. \--- /task \---