## Mova o ator do jogador

Comece criando um ator `jogador` que pode se mover ao redor do seu mundo.

--- task ---

Abra o projeto inicial do Scratch 'Crie seu próprio mundo'.

**Online:** abra o projeto inicial em [scratch.mit.edu/projects/395786610](https://scratch.mit.edu/projects/395786610){:target="_blank"}.

Se você tiver uma conta Scratch, você pode fazer uma cópia clicando em **Remix**.

**Offline**: faça o download do projeto inicial [rpf.io/p/pt-BR/create-your-own-world-go](https://rpf.io/p/pt-BR/create-your-own-world-go){:target="_blank"}, e então abra-o usando o editor off-line. Se você precisar baixar e instalar o editor offline do Scratch, você pode encontrá-lo em [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![captura de tela](images/world-starter.png)

--- /task ---

Pressionando as setas direcionais moverá o ator `jogador`. Quando a seta para cima é pressionada, o ator `jogador` moverá para cima em resposta.

--- task ---

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

--- /task ---

--- task ---

Clique na bandeira e mantenha pressionada a seta para cima. O ator `jogador` se move para cima?

![captura de tela](images/world-up.png)

--- /task ---

--- task ---

Para mover o ator `jogador` para a esquerda, você precisa adicionar outro bloco `se`{:class="block3control"} com código similar:

![jogador](images/player.png)

```blocks3
when flag clicked
forever
	if <key (seta para cima v) pressed? > then
		point in direction (0)
		move (4) steps
	end
+	if <key (seta para esquerda v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Adicione mais código ao seu ator `jogador` para que ele possa se mover para baixo e para a direita. Use o código que você já tem para ajudá-lo.

--- hints ---


--- hint ---

Para mover para cima, aponte o ator `jogador` para a direção `0` graus. O que você precisa fazer para mover o ator para baixo?

Para mover para a esquerda, você aponta o ator na direção `-90` graus. O que você precisa fazer para mover o ator para direita?

--- /hint ---

--- hint ---

Você precisa alterar estes dois blocos:

![jogador](images/player.png)

```blocks3
<tecla ( v) pressionada>

aponte para a direção ()
```

Duplique o código que faz o ator `jogador` mover para cima e altere esses dois blocos para fazer o ator mover para baixo. Duplique o código novamente e altere-o para fazer o ator mover para a direita.

--- /hint ---

--- hint ---

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

--- /hint ---

--- /hints ---

--- /task ---
