## Mova-se pelo seu mundo

O ator `jogador` deve ser capaz de atravessar portas para outras salas.

Seu projeto contém cenários para salas adicionais:

![captura de tela](images/world-backdrops.png)

\--- task \---

Crie uma nova variável 'para todos os atores' chamada `sala` {:class="block3variables"} para acompanhar em qual sala está o ator `jogador`.

[[[generic-scratch3-add-variable]]]

![captura de tela](images/world-room.png)

\--- /task \---

\--- task \---

Quando o ator `jogador` toca a porta laranja na primeira sala, o jogo deve exibir o próximo cenário, e o ator `jogador` deve voltar para o lado esquerdo do Palco. Adicione este código no ator `jogador` dentro do loop `sempre`{:class="block3control"}:

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
        point in direction (180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > então 
    aponte para a direção (90)
    mova (4) passos
  end
  se <tocando na cor [#BABABA]? > então 
    mova (-4) passos
  end
+ se < tocando na cor [#F2A24A]> então 
    mude para o cenário (próximo cenário v)
    vá para x: (-200) y: (0)
    adicione (1) a [sala v]
  end
end
```

\--- /task \---

\--- task \---

Sempre que o jogo começa, a sala, a posição do personagem e o cenário precisam ser redefinidos.

Adicione código ao **início** do código do seu ator `jogador` acima do loop `sempre`{:class="block3control"}, para redefinir tudo quando bandeira é clicada:

\--- hints \---

\--- hint \---

Quando o jogo começa:

+ O valor de `sala`{:class="block3variables"} deve ser definido como `1`{:class="block3variables"}
+ O `cenário`{:class="block3looks"} deve ser definido para `sala1`{:class="block3looks"}
+ A posição do ator `jogador` deve ser definida como `x: -200 y: 0`{:class="block3motion"}

\--- /hint \---

\--- hint \---

Aqui estão os blocos que você precisa:

![jogador](images/player.png)

```blocks3
vá para x: (-200) y: (0)

mude [sala v] para (1)

mude para o cenário (sala1 v)
```

\--- /hint \---

\--- hint \---

Veja como seu código finalizado deve parecer:

![jogador](images/player.png)

```blocks3
quando ⚑ for clicado
+mude [sala v] para (1)
+vá para x: (-200) y: (0)
+mude para o cenário (sala1 v)
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
        point in direction (180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > então 
    aponte para a direção (90)
    mova (4) passos
  end
    se <tocando na cor [#BABABA]? > então 
    mova (-4) passos
  end
  se <tocando na cor [#F2A24A]?> então 
    mude para o cenário (próximo cenário v)
    vá para x: (-200) y: (0)
    adicione (1) a [sala v]
  end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Clique na bandeira e, em seguida, mova seu ator `jogador` até que ele toque a porta laranja. O ator se move para a próxima tela? A variável `sala`{:class="block3variables"} muda para `2`?

![captura de tela](images/world-room-test.png)

\--- /task \---