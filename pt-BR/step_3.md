## Paredes sólidas

\--- task \---

Teste seu ator `jogador` novamente. Do you see that it can walk through the light grey walls?

![captura de tela](images/world-walls.png)

\--- /task \---

\--- task \---

Para consertar isso, você precisa fazer o ator `jogador` mover de volta se tocar uma parede cinza. Aqui está o código que você precisa adicionar dentro do seu bloco `sempre`{:class="block3control"} abaixo dos blocos de direção:

![jogador](images/player.png)

```blocks3
quando ⚑ for clicado
sempre 
  se <tecla (seta para cima v) pressionada? > então 
    aponte para a direção (0)
    mova (4) passos
  end
  se <tecla (seta para esquerda v) pressionada? > então 
    aponte para a direção (-90)
    mova (4) passos
  end
  se <tecla (seta para baixo v) pressionada? > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > então 
    aponte para a direção (90)
    mova (4) passos
  end
+ se <tocando na cor [#BABABA]? > então 
    mova (-4) passos
  end
end
```

\--- /task \---

\--- task \---

Tente fazer o ator `jogador` se mover através de uma parede. Se o seu novo código funcionar, isso não deve ser possível.

![captura de tela](images/world-walls-test.png)

\--- /task \---