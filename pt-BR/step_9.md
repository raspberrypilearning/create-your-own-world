## Desafio: adicione um inimigo

Se você quiser, você também pode adicionar ao seu jogo inimigos de patrulha. Se o `player` sprite toca um inimigo, o jogo termina.

+ Seu jogo já contém `enemy` sprite. Adicione código ao `enemy` sprite para que ele só apareça na sala 2.

+ Adicione código para mover o `enemy` sprite e para terminar o jogo se o `enemy` sprite tocar o `player` sprite. É mais fácil fazer isso em blocos de código separados. Aqui está como seu `enemy` sprite pode parecer:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ Testa o teu jogo para ter a certeza que: 
    + O `enemy` sprite visível somente na sala 2
    + O `enemy` sprite visível somente na sala
    + O jogo acaba se o `player` sprite `enemy`

Você pode criar outro `enemy` sprite na sala 3 que patrulha para cima e para baixo o fosso na parede?

![screenshot](images/world-enemy2.png)