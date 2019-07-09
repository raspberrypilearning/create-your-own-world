## Murs solides

\--- tâche \--- Testez à nouveau votre sprite `joueur`. Voyez-vous qu'il peut traverser les murs gris clair?

![capture d'écran](images/world-walls.png) \--- /task \---

\--- tâche \--- Pour résoudre ce problème, vous devez faire reculer le sprite `joueur` s'il touche un mur gris clair. Voici le code que vous devez ajouter dans votre bloc `forever`{: class = "block3control"} sous les blocs de direction:

![joueur](images/player.png)

```blocks3
lorsque le drapeau a cliqué sur
pour toujours
    si la touche <(flèche haut v) est enfoncée > puis
        point dans la direction (0)
        déplacer (4) les étapes

    si <touche (flèche gauche v) est enfoncée? > puis
        point dans le sens (-90)
        déplacer (4) les étapes

        si <touche (flèche vers le bas v) est enfoncée? > puis
        point dans la direction (-180)
        déplacer (4) les étapes

        si <touches [flèche droite v] sont enfoncées? > puis
        point dans la direction (90)
        déplacer (4) les étapes

+ si < couleurs touchantes > puis
    mouvement (-4) pas
    fin
fin
```

\--- /task \---

\--- task \---

Essayez de faire en sorte que le `joueur` sprite passe à travers un mur. Si votre nouveau code fonctionne, cela ne devrait pas être possible.

![capture d'écran](images/world-walls-test.png) \--- /task \---