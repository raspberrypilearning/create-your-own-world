## Mova o sprite do jogador

Comece criando um sprite `player` que pode se mover ao redor do seu mundo.

\--- task \---

Abra o projeto inicial do Scratch 'Crie seu próprio mundo'.

** Online: ** abra o projeto inicial em [ rpf.io/create-your-own-world-on ](http://rpf.io/create-your-own-world-on) {: target = "_ blank"}.

Se você tiver uma conta Scratch, você pode fazer uma cópia clicando em **Remix**.

**Offline**: download the starter project [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_blank"}, and then open it using the offline editor. Se você precisar baixar e instalar o editor offline do Scratch, poderá encontrá-lo em [ rpf.io/scratchoff ](https://rpf.io/scratchoff) {: target = "_ blank"}.

![screenshot](images/world-starter.png)

\--- /task \---

Ao pressionar as setas mover o sprite `player`. Quando a seta para cima é pressionada, o `player` sprite move para cima em resposta.

\--- task \---

Adicione este código para imprimir sua variável `jogadores`:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

Clique no sinalizador e depois segure a seta para cima. O `player` sprite se move para cima?

![screenshot](images/world-up.png)

\--- /task \---

\--- task \---

Para mover o `player` sprite à esquerda, você precisa adicionar outro `se`{:class="block3control"} com um código similar:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

Adicione mais código ao seu ` player ` sprite para que ele também possa se mover para baixo e para a direita. Use o código que você já tem para ajudá-lo.

\--- hints \---

\--- hint \---

Para mover para cima, aponte o `player` para a direção `0` graus. O que você precisa fazer para mover o sprite para baixo?

Para mover para a esquerda, você aponta o sprite na direção `-90` graus. O que você tem que fazer para mover o sprite para a direita?

\--- /hint \---

\--- hint \---

Você precisa alterar estes dois blocos:

![player](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Duplique o código que faz o `player` sprite mover para cima e alterar esses dois blocos para fazer o sprite descer. Duplique o código novamente e altere-o para fazer o sprite se mover para a direita.

\--- /hint \--- \--- hint \--- Aqui está como o teu código deve parecer:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end

+    if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
+    if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---