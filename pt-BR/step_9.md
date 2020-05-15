## Desafio: adicione um inimigo

Se você quiser, você também pode adicionar ao seu jogo inimigos de patrulha. Se o ator `jogador` toca em um inimigo, o jogo termina.

+ Seu jogo já contém um ator `inimigo`. Adicione código ao ator `inimigo` para que apareça apenas na sala 2.

+ Adicione código para mover o ator `inimigo` e para terminar o jogo se o ator `inimigo` tocar o ator `jogador`. É mais fácil fazer isso em blocos de código separados. Aqui está como seu código do ator `inimigo` deve ficar:

```blocks3
quando ⚑ for clicado
sempre 
se < (sala :: variables)=[2]> então 
mostre
senão 
esconda

quando ⚑ for clicado
sempre 
se < tocando em (jogador v)?> então 
pare [todos v]

quando ⚑ for clicado
vá para x: (170) y: (0)
sempre 
repita (130) vezes 
adicione (-1) a x
end
repita (130) vezes 
adicione (1) a x
```

+ Teste o seu novo código para ter certeza que: 
    + O ator `inimigo` é visível apenas na sala 2
    + O ator `inimigo` patrulha a sala
    + O jogo acaba se o ator `jogador` tocar o ator `inimigo`

Você pode criar outro ator `inimigo` na sala 3 que patrulha para cima e para baixo e pelo vão da parede?

![captura de tela](images/world-enemy2.png)