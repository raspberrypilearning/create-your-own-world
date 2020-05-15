## Pessoas

Adicione outras pessoas ao seu mundo com quem seu ator `jogador` pode interagir.

\--- task \---

Mude para o ator `pessoa`.

![Ator pessoa](images/person.png)

\--- /task \---

\--- task \---

Adicione algum código ao ator `pessoa` para que a pessoa converse com o ator `jogador`. Este código é muito parecido com o código que você adicionou ao seu ator `sinalização`:

![pessoa](images/person.png)

```blocks3
quando ⚑ for clicado
vá para x: (0) y: (-150)
sempre 
  se <tocando em (jogador v)? > então 
diga [Você sabia que pode passar pelas portas laranjas e amarelas?]
senão 
diga []
end
end
```

\--- /task \---

\--- task \---

Permita que seu ator `pessoa` se mova adicionando esses dois blocos na seção `senão`{:class="block3control"} do seu código:

![pessoa](images/person.png)

```blocks3
quando ⚑ for clicado
vá para x: (0) y: (-150)
sempre 
  se <tocando em (jogador v)? > então 
diga [Você sabia que passar pelas portas laranjas e amarelas?]
senão 
diga []
+   mova (1) passos
+   se tocar na borda, volte
end
end
```

\--- /task \---

Seu ator `pessoa` se moverá agora, mas vai parar para falar com o ator `jogador`.

![captura de tela](images/world-person-test.png)

\--- task \---

Adicione código ao seu novo ator `pessoa` para que o ator apareça apenas na sala 1. O código que você precisa é exatamente o mesmo que o código que torna o ator `sinalização` visível apenas na sala 1.

Certifique-se de testar seu novo código.

\--- /task \---