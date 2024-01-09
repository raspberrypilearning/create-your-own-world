## Mova o ator do jogador

Comece criando um ator `jogador` que pode se mover ao redor do seu mundo.

\--- task \---

Abra o projeto inicial do Scratch 'Crie seu próprio mundo'.

**Online**: open the online starter project at [rpf.io/create-your-own-world-on](https://rpf.io/create-your-own-world-on){:target="_blank"}.

Se você tiver uma conta Scratch, você pode fazer uma cópia clicando em **Remix**.

**Offline**: download the starter project [rpf.io/p/en/create-your-own-world-go](https://rpf.io/p/en/create-your-own-world-go){:target="_blank"}, and then open it using the offline editor. Se você precisar baixar e instalar o editor offline do Scratch, você pode encontrá-lo em [rpf.io/scratchoff](https://rpf.io/scratchoff) {: target = "_ blank"}.

![captura de tela](images/world-starter.png)

\--- /task \---

Pressionando as setas direcionais moverá o ator `jogador`. Quando a seta para cima é pressionada, o ator `jogador` moverá para cima em resposta.

\--- task \---

Adicione este código ao ator `jogador`:

![jogador](images/player.png)

```blocks3
quando ⚑ for clicado
sempre 
  se <tecla (seta para cima v) pressionada? > então 
    aponte para a direção (0)
    mova (4) passos
  end
end
```

\--- /task \---

\--- task \---

Clique na bandeira e mantenha pressionada a seta para cima. O ator `jogador` se move para cima?

![captura de tela](images/world-up.png)

\--- /task \---

\--- task \---

Para mover o ator `jogador` para a esquerda, você precisa adicionar outro bloco `se`{:class="block3control"} com código similar:

![jogador](images/player.png)

```blocks3
quando ⚑ for clicado
sempre 
  se <tecla (seta para cima v) pressionada? > então 
    aponte para a direção (0)
    mova (4) passos
  end
  + se <tecla (seta para esquerda v) pressionada? > então 
    aponte para a direção (-90)
    mova (4) passos
  end
end
```

\--- /task \---

\--- task \---

Adicione mais código ao seu ator `jogador` para que ele possa se mover para baixo e para a direita. Use o código que você já tem para ajudá-lo.

\--- hints \---

\--- hint \---

Para mover para cima, aponte o ator `jogador` para a direção `0` graus. O que você precisa fazer para mover o ator para baixo?

Para mover para a esquerda, você aponta o ator na direção `-90` graus. O que você precisa fazer para mover o ator para direita?

\--- /hint \---

\--- hint \---

Você precisa alterar estes dois blocos:

![jogador](images/player.png)

```blocks3
<tecla ( v) pressionada>

aponte para a direção ()
```

Duplique o código que faz o ator `jogador` mover para cima e altere esses dois blocos para fazer o ator mover para baixo. Duplique o código novamente e altere-o para fazer o ator mover para a direita.

\--- /hint \---

\--- hint \---

Aqui está como seu código deve ficar:

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

+ se <tecla (seta para baixo v) pressionada? > então 
    aponte para a direção (180)
    mova (4) passos
  end
+ se <tecla (seta para direita v) pressionada? > então 
    aponte para a direção (90)
    mova (4) passos
  end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---