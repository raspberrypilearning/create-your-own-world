## Coletar moedas

Seu `jogador` sprite deve coletar moedas à medida que se move pelo mundo.

--- task ---

Adicione uma nova variável chamada `moedas`{:class="block3variables"} em seu projeto.

--- /task ---

--- task ---

Selecione o ator `moeda` e clique em **mostrar**.

![captura de tela](images/coin.png)

--- /task ---

--- task ---

Adicione código ao ator `moeda` para que apareça apenas na sala 1.

![captura de tela](images/coin.png)

```blocks3
quando ⚑ for clicado
sempre 
se <(sala :: variáveis)=[1]> então 
mostre
senão 
esconda
```

--- /task ---

--- task ---

Adicione código a seu ator `moeda` para que o ator moeda `se esconda`{:class="block3looks"} e `1`{:class="block3variables"} seja adicionado à variável `moedas`{:class="block3variables"} uma vez que o ator `jogador` tocar no ator `moeda` para 'pegá-lo'.

![moeda](images/coin.png)

```blocks3
quando ⚑ for clicado
espere até que <touching (player v)?>
adicione (1) a [moedas v]
esconda
pare [outros scripts no sprite v]
```

O código `interrompe outros scripts no sprite`{:class="block3control"} é necessário para que a `moeda` sprite deixe de ser exibida na sala 1 depois de coletado.

--- /task ---

--- task ---

Agora adicione código ao palco para definir sua variável `moedas`{:class="block3variables"} para `0`{:class="block3variables"} no início do jogo.

![palco](images/stage.png)

```blocks3
quando ⚑ for clicado
mude [moedas v] para [0]
```

--- /task ---

--- task ---

Teste seu jogo. Coletar uma moeda deve alterar a sua pontuação `moedas` para `1`{:class="block3variables"}.

--- /task ---