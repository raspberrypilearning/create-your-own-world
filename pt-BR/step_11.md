## Portas e chaves

Agora você vai adicionar o código para que algumas das portas do seu mundo de jogo estejam bloqueadas, e o jogador deve encontrar a chave para abri-las e chegar para a próxima sala.

\--- tarefa \--- Alterne para a `key` sprite. Clique em `show`{:class="blocklooks"} no menu Scripts para que o sprite apareça na fase. \--- /task \---

\--- tarefa \--- Edite a `key` do sprite para que fique azul. \--- /task \---

\--- tarefa \--- Mude seu plano de fundo para a sala 3, e coloque o `key` sprite em algum lugar difícil de alcançar!

![screenshot](images/world-key.png)

\--- /task \---

\--- tarefa\--- Adicione código à sua `key` sprite para que ele só apareça na sala 3. \--- /task \---

\--- tarefa \--- Crie uma nova lista chamada `inventory` {:class="block3variables"} para armazenar os itens do seu `player` sprite coleta.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- tarefa \--- O código que você precisa adicionar para coletar a chave é muito semelhante ao código para coletar moedas. A diferença é que você adiciona a chave ao inventário ` ` {:class="block3variables"}.

![key](images/key.png)

```blocks3
quando o sinalizador clicou
espere até <touching (player v)?>
adicione [chave azul] ao [inventário v]
oculte
pare [outros scripts no sprite v]
```

\--- /task \---

\--- tarefa \--- Adicione um código ao seu estágio para esvaziar seu inventário no início do jogo.

```blocks3
deletar (todos v) de [inventário v]
```

\--- /task \---

\--- tarefa \--- Teste seu jogo para verificar se você pode coletar a `key` sprite e adicioná-lo ao seu inventário. \--- /task \---

\--- tarefa \--- Agora adicione a porta trancada. Selecione o `door-blue` sprite e clique no `show`{:class="blocklooks} no menu Scripts e então posicione o sprite entre as duas paredes.

![screenshot](images/world-door.png) \--- /task \---

\--- tarefa\--- Adicione o código à sua `door-blue` sprite para que ele só apareça na sala 3. \--- /task \---

\--- tarefa \--- Adicione código ao sprite `door-blue` para que, quando a chave estiver no `inventário`{:class="block3variables"}, o sprite `hides`{:class="block3looks"} para permitir que seu `player` sprite passe.

![door](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- tarefa \--- Teste seu jogo e veja se você consegue coletar a chave azul para abrir a porta! \--- /task \---