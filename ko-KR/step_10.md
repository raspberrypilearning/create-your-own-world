## 코인 모으기

`플레이어` 스프라이트는 세계를 통과하면서 동전을 수집 할 수 있어야합니다.

\--- task \--- 새로운 변수 `코인`{: class = "block3variables"} 을 프로젝트에 추가하세요. \--- /task \---

\--- task \--- `코인` 스프라이트를 클릭하고 **보여주기**를 클릭하세요.

![스크린샷](images/coin.png) \--- /task \---

\--- task \--- 당신의 코드를 `코인` 스프라이트에 방1 에서만 나타나도록 추가하세요. ![스크린샷](images/coin.png)

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

당신의 코드를 `coin`스프라이트에 추가해서 스프라이트 `hides`{:class="block3looks"} 와 `1`{:class="block3variables"} 가 `coins`{:class="block3variables"} 변수에 `player`스프라이트가 `coin`스프라이트를 '줍기'위해 닿았을 때 추가되도록 하십시오.

![코인](images/coin.png)

```blocks3
flag클릭 시
기다리기 <touching (player v)?>
[coins v] 를 (1) 로 바꾸기
숨기기
[스프라이트v의 다른 스크립트들] 멈추기
```

`스프라이트에서 다른 스크립트를 중지시키기`{:class="block3control"}라는 코드는 `coin`스프라이트가 수집된 후 방1에서 표시되는 것을 멈추게 하기 위해 필요합니다. 

\--- /task \---

\--- task \--- 이제 스테이지에 코드를 추가하여 `coins`{:class="block3variables"} 변수를 게임 시작시 `0`{:class="block3variables"}으로 설정하세요.

![스테이지](images/stage.png)

```blocks3
flag 클릭했을 때
[coins v] 를 [0] 으로 설정하기
```

\--- /task \---

\--- task \--- 게임을 테스트 해 보세요. 동전을 모으면 `coins`점수가 `1`{:class="block3variables"}로 바뀔 것 입니다. \--- /task \---