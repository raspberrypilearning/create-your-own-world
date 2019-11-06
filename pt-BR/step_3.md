## Paredes sólidas

\--- tarefa \--- Teste seu `player` sprite novamente. Você vê que ele pode atravessar as paredes cinza-claras.

![screenshot](images/world-walls.png) \--- /task \---

\--- tarefa \--- Para corrigir isso, você precisa criar o `player` sprite retroceda se tocar uma parede cinza clara. Aqui está o código que você precisa adicionar dentro de seu `para sempre`{:class="block3control"} bloco abaixo dos blocos de direção:

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
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

\--- /task \---

\--- task \---

Tente fazer o `player` se mover através de uma parede. Se seu novo código funcionar, isso não deve ser possível.

![screenshot](images/world-walls-test.png) \--- /task \---