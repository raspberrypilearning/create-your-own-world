## Portas e chaves

Agora você vai adicionar o código para que algumas das portas do seu mundo de jogo estejam bloqueadas, e o jogador deve encontrar a chave para abri-las e chegar à próxima sala.

--- task ---

Mude para o ator `chave`. Clique em `Mostrar`{:class="blocklooks"} para que o ator apareça no palco.

--- /task ---

--- task ---

Edite a fantasia do ator `chave` para que fique azul.

--- /task ---

--- task ---

Mude seu cenário do palco para a sala 3 e coloque o ator `chave` em algum lugar difícil de alcançar!

![captura de tela](images/world-key.png)

--- /task ---

--- task ---

Adicione código ao ator `chave` para torná-lo visível apenas na sala 3.

--- /task ---

--- task ---

Crie uma nova lista chamada `inventário`{:class="block3variables"} para armazenar os itens que o ator `jogador` coleta.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

O código que você precisa adicionar para coletar a chave é muito semelhante ao código para coletar moedas. A diferença é que você adiciona a chave ao `inventário`{:class="block3variables"}.

![chave](images/key.png)

```blocks3
when flag clicked
wait until <touching (jogador v)?>
add [chave azul] to [inventário v]
hide
stop [outros scripts no ator v]
```

--- /task ---

--- task ---

Adicione código ao seu palco para esvaziar seu inventário no início do jogo.

```blocks3
delete all of [inventário v]
```

--- /task ---

--- task ---

Teste seu jogo para verificar se você pode coletar o ator `chave` e adicioná-lo ao seu inventário.

--- /task ---

--- task ---

Agora adicione a porta trancada. Selecione o ator `porta azul` e clique em `Mostrar`{:class="blocklooks} e então posicione o ator no espaço entre as duas paredes.

![captura de tela](images/world-door.png)

--- /task ---

--- task ---

Adicione código ao ator `porta azul` para que apareça apenas na sala 3.

--- /task ---

--- task ---

Adicione código ao ator `porta azul` para que, quando a chave estiver no `inventário`{:class="block3variables"}, o ator se `esconda`{:class="block3looks"} para permitir que seu `jogador` passe.

![porta](images/door.png)

```blocks3
when flag clicked
wait until <[inventário v] contains [chave azul]?>
stop [other scripts in sprite v]
hide
```

--- /task ---

--- task ---

Teste seu jogo e veja se você pode pegar a chave azul para abrir a porta!

--- /task ---