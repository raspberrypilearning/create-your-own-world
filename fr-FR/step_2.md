## Déplace le sprite du joueur

Commencez par créer un `joueur` sprite qui peut se déplacer dans votre monde.

\--- task \---

Ouvrez le projet de démarrage Scratch «Créez votre propre monde».

**En ligne**: ouvrez le projet de démarrage en ligne à [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){: target = "_ blank"}.

Si tu as un compte Scratch, tu peux en créer une copie en cliquant sur **Remix**.

**Offline**: téléchargez le projet de démarrage [rpf.io/p/fr/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){: target = "_ blank"}, puis ouvrez-le à l'aide de l'éditeur hors connexion. Si tu dois télécharger et installer l'éditeur hors ligne Scratch, tu peux le trouver à [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![capture d'écran](images/world-starter.png)

\--- /task \---

En appuyant sur les touches fléchées, le sprite</code> doit être déplacé à `joueur. Lorsque vous appuyez sur la flèche vers le haut, le sprite <code>joueur` doit remonter sur la scène en réponse.

\--- task \---

Ajoute ce code au lutin `jouer` :

![joueur](images/player.png)

```blocks3
lorsque le drapeau a cliqué sur
pour toujours
    si la touche <(flèche haut v) est enfoncée > puis
        point en direction (0)
        mouvement (4) pas
    fin
fin
```

\--- /task \---

\--- task \---

Cliquez sur le drapeau, puis maintenez la flèche vers le haut. Est-ce que le `joueur` sprite monte?

![capture d'écran](images/world-up.png)

\--- /task \---

\--- task \---

Pour déplacer le sprite `joueur` vers la gauche, vous devez ajouter un autre bloc `si`{: class = "block3control"} avec le code similaire:

![joueur](images/player.png)

```blocks3
lorsque le drapeau a cliqué sur
pour toujours
    si la touche <(flèche haut v) est enfoncée > puis
        point en direction (0)
        déplacer (4) pas
    fin
+ si <touche (flèche gauche v) appuyée? > puis
        point en direction (-90)
        mouvement (4) pas
    fin
fin
```

\--- /task \---

\--- task \---

Ajouter plus de code à votre `joueur` sprite il peut se déplacer vers le bas et à droite aussi. Utilise le code que tu as déjà pour t'aider.

\--- hints \---

\--- hint \---

Pour vous déplacer vers le haut, vous pointez le sprite `joueur` dans la direction `0` degrés. Que devez-vous faire pour déplacer le sprite vers le bas?

Pour vous déplacer à gauche, pointez l’image-objet dans la direction `90` degrés. Que devez-vous faire pour déplacer le sprite correctement?

\--- /hint \---

\--- hint \---

Vous devez changer ces deux blocs:

![joueur](images/player.png)

```blocks3
<key ( v) pressed>

point dans la direction ()
```

Dupliquez le code qui fait que le sprite `joueur` progresse vers le haut et modifiez ces deux blocs pour faire descendre le sprite Dupliquez à nouveau le code et modifiez-le pour que le sprite se déplace vers la droite.

\---/hint\--- \---hint\--- Voici a quoi devrait ressembler ton code :

![joueur](images/player.png)

```blocks3
lorsque le drapeau a cliqué sur
pour toujours
    si la touche <(flèche haut v) est enfoncée > puis
        point dans la direction (0)
        déplacer (4) les étapes

    si <touche (flèche gauche v) est enfoncée? > puis
        point en direction (-90)
        déplacer (4) étapes


+ si <touche (flèche vers le bas v) appuyée? > puis
        point en direction (180)
        déplacer (4) pas
    fin
+ si <touche [flèche droite v] enfoncée? > puis
        point en direction (90)
        déplacer (4) pas
    fin
fin
```

\--- / indice \--- \--- / conseils \---

\--- /task \---