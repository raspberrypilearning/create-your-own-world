## Murs solides

--- task --- Teste à nouveau ton sprite `joueur`. Vois-tu qu'il peut traverser les murs gris clair.

![capture d'écran](images/world-walls.png) --- /task ---

--- task --- Pour résoudre ce problème, tu dois faire reculer le sprite `joueur` s'il touche un mur gris clair. Voici le code que tu dois ajouter dans ton bloc `répéter indéfiniment`{:class="block3control"} sous les blocs de direction:

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment 
    si <touche (flèche haut v) pressée ? > alors
        s'orienter en direction de (0)
        avancer de (4) pas
    end
si <touche (flèche de gauche v) pressée ? > alors
        s'orienter en direction de (-90)
        avancer de (4) pas
    end
        si < touche (flèche du bas v) pressée ? > alors
        s'orienter en direction de (-180)
        avancer de (4) pas
    end
        si <touche [flèche de droite v] pressée? > alors
        s'orienter en direction de (90)
        avancer de (4) pas
    end
+ si < couleur [#BABABA] touchée ? > alors
    avancer de (-4) pas
    end
end
```

--- /task ---

--- task ---

Essaye de faire en sorte que le sprite `joueur` passe à travers un mur. Si ton nouveau code fonctionne, cela ne devrait pas être possible.

![capture d'écran](images/world-walls-test.png) --- /task ---