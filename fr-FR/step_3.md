## Murs solides

\--- task \--- Teste à nouveau ton sprite `joueur`. Vois-tu qu'il peut traverser les murs gris clair.

![capture d'écran](images/world-walls.png) \--- /task \---

\--- task \--- Pour résoudre ce problème, vous devez faire reculer le sprite `joueur` s'il touche un mur gris clair. Voici le code que tu dois ajouter dans ton bloc `répéter indéfiniment`{: class = "block3control"} sous les blocs de direction:

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter pour toujours
    si la touche <(flèche haut v) est enfoncée? > alors
        s'orienter dans la direction (0)
        déplacer de (4) pas
    fin
    si <la touche (flèche de gauche v) est appuyée? > alors
        s'orienter dans la direction (-90)
        déplacer de (4) pas
    fin
        si <la touche (flèche du bas v) est appuyée? > alors
        s'orienter dans la direction (-180)
        déplacer de (4) pas
    fin
        si <la touche [flèche de droite v] est appuyée? > alors
        s'orienter dans la direction (90)
        déplacer de (4) pas
    fin
+   si < la couleur touchée [#BABABA]? > alors
    déplacer de (-4) pas
    fin
fin
```

\--- /task \---

\--- task \---

Essaye de faire en sorte que le sprite `joueur` passe à travers un mur. Si ton nouveau code fonctionne, cela ne devrait pas être possible.

![capture d'écran](images/world-walls-test.png) \--- /task \---