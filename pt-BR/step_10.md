## Coletar moedas

Seu `jogador` sprite deve coletar moedas à medida que se move pelo mundo.

\--- task \--- Adicione uma nova variável chamada ` coins ` {:class="block3variables"} para o seu projeto. \--- /task \---

\--- tarefa \--- Selecione `coin` sprite e clique em **show**.

![screenshot](images/coin.png) \--- /task \---

\--- tarefa\--- Adicione código à sua `moeda` sprite para que ele só apareça na sala 1. ![screenshot](images/coin.png)

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

Adicione código à sua `coin` sprite para que o sprite `hides` {:class="block3looks"} e `1` {:class="block3variables"} é adicionado às moedas ` ` variável {:class="block3variables"} uma vez que o `player` sprite toca a `coin` sprite para 'buscá-lo'.

![moeda](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

O código `interrompe outros scripts no sprite`{:class="block3control"} é necessário para que a `moeda` sprite deixe de ser exibida na sala 1 depois de coletado.

\--- /task \---

\--- tarefa \--- Agora adicione o código ao estágio para definir suas `moedas`{:class="block3variables"} variável `0`{:class="block3variables"} ao início do jogo.

![estágio](images/stage.png)

```blocks3
quando a bandeira for clicada
definir [coins v] para [0]
```

\--- /task \---

\--- task \--- Teste seu projeto. Para coletar uma moeda deve-se alterar a sua pontuação `moedas ` para `1`{:class="block3variables"}. \--- /task \---