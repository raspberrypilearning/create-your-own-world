## Sinalizações

Agora adicione sinalizações ao seu mundo para guiar os jogadores em suas jornadas.

Seu projeto inclui um ator `sinalização bem-vindo`:

![captura de tela](images/world-sign.png)

\--- task \---

O ator `sinalização bem-vindo` deve estar visível apenas na sala 1, então adicione algum código ao ator para garantir que isso aconteça:

\--- hints \---

\--- hint \---

`quando ⚑ for clicado`{:class="block3events"}, em um loop `sempre`{:class="block3control"}, verifique `se`{:class="block3control"} a `sala é 1`{:class="block3variables"} e, nesse caso, `mostre`{:class="block3looks"} o ator `sinalização bem-vindo`, `senão`{:class="block3control"} `esconda`{:class="block3looks"} o ator.

\--- /hint \---

\--- hint \---

Aqui estão os blocos que você precisa:

![sinalização](images/sign.png)

```blocks3
<br />se < > então
senão
end

< (sala :: variáveis) = [1] >

esconda

mostre

sempre
end

quando ⚑ for clicado

```

\--- /hint \---

\--- hint \---

Aqui está o código completo:

![sinalização](images/sign.png)

```blocks3
when flag clicked
forever
    if < (room :: variables) = [1] > then
        show
    else
        hide
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Teste o código para o seu ator `sinalização bem-vindo` movendo-se entre as salas. A sinalização só deve estar visível na sala 1.

![captura de tela](images/world-sign-test.png)

\--- /task \---

\--- task \---

Uma sinalização não é muito boa se não diz nada! Adicione um pouco mais de código para exibir uma mensagem se o ator `sinalização bem-vindo` está tocando no ator `jogador`:

![sinalização](images/sign.png)

```blocks3
when flag clicked
forever
if < (room :: variables) = [1] > then
show
else
hide
end
+if < touching (player v)? > então 
   diga [Bem-vindo! Can you get to the treasure?]
else
say []
end
end
```

\--- /task \---

\--- task \---

Teste seu ator `sinalização bem-vindo` novamente. Agora você deve ver uma mensagem quando o ator `jogador` toca no ator `sinalização bem-vindo`.

![captura de tela](images/world-sign-test2.png)

\--- /task \---