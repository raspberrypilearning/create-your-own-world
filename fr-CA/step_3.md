## Murs solides

\--- task \---

Task \---Teste à nouveau ton sprite `joueur`. Do you see that it can walk through the light grey walls?

![capture d'écran](images/world-walls.png)

\--- /task \---

\--- task \---

Pour corriger cela, tu dois faire reculer le lutin `joueur` s'il touche un mur gris clair. Voici le code que tu dois ajouter dans ton bloc `répéter indéfiniment`{:class="block3control"} sous les blocs de direction:

![joueur](images/player.png)

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
        point in direction (180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > then
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

Essaye de faire en sorte que le sprite `joueur` passe à travers un mur. Si ton nouveau code fonctionne, cela ne devrait pas être possible.

![capture d'écran](images/world-walls-test.png)

\--- /task \---