## Déplace le sprite du joueur

Commence par créer un sprite `joueur` qui peut se déplacer dans ton monde.

\--- task \---

Ouvre le projet de démarrage Scratch «Créez ton propre monde».

**En ligne**: ouvre le projet de démarrage en ligne à [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){: target = "_ blank"}.

Si tu as un compte Scratch, tu peux en créer une copie en cliquant sur **Remix**.

**Hors ligne**: télécharge le projet de démarrage [rpf.io/p/fr/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){: target = "_ blank"}, puis ouvre-le à l'aide de l'éditeur hors connexion. Si tu dois télécharger et installer l'éditeur hors ligne Scratch, tu peux le trouver à [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![capture d'écran](images/world-starter.png)

\--- /task \---

En appuyant sur les touches fléchées, le sprite</code> doit être déplacé à `joueur. Lorsque vous appuyez sur la flèche vers le haut, le sprite <code>joueur` doit remonter sur la scène en réponse.

\--- task \---

Ajoute ce code au sprite `joueur` :

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
    si la touche <(flèche haut v) est enfoncée? > alors
        s'orienter en direction de (0)
        déplacer de (4) pas
    fin
fin
```

\--- /task \---

\--- task \---

Clique sur le drapeau, puis maintenez la flèche vers le haut. Est-ce que le sprite `joueur` monte vers le haut?

![capture d'écran](images/world-up.png)

\--- /task \---

\--- task \---

Pour déplacer le sprite `joueur` vers la gauche, tu dois ajouter un autre bloc `si`{: class = "block3control"} avec le code similaire:

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué 
répéter indéfiniment
    si la touche <(flèche haut v) est enfoncée? > alors
        s'orienter en direction de (0)
        déplacer de (4) pas
    fin
+ si <touche (flèche gauche v) est appuyée? > alors
        s'orienter en direction de (-90)
        déplacer de (4) pas
    fin
fin
```

\--- /task \---

\--- task \---

Ajoute plus de code à ton sprite `joueur` pour qu'il puisse se déplacer vers le bas et à droite également. Utilise le code que tu as déjà pour t'aider.

\--- hints \---

\--- hint \---

Pour te déplacer vers le haut, tu pointes le sprite `joueur` dans la direction `0` degrés. Que dois-tu faire pour déplacer le sprite vers le bas?

Pour te déplacer à gauche, pointe le sprite dans la direction `90` degrés. Que dois-tu faire pour déplacer le sprite correctement?

\--- /hint \---

\--- hint \---

Tu dois changer ces deux blocs:

![joueur](images/player.png)

```blocks3
<key ( v) pressed>

s'orienter dans la direction ()
```

Dupliquez le code qui fait que le sprite `joueur` progresse vers le haut et modifie ces deux blocs pour faire descendre le sprite. Duplique à nouveau le code et modifie-le pour que le sprite se déplace vers la droite.

\---/hint\--- \---hint\--- Voici a quoi devrait ressembler ton code :

![joueur](images/player.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
    si la touche <(flèche haut v) est enfoncée? > alors
        s'orienter dans la direction (0)
        déplacer de (4) pas

    si <touche (flèche gauche v) est enfoncée? > alors
        s'orienter en direction de (-90)
        déplacer de (4) pas


+ si <touche (flèche vers le bas v) est appuyée? > alors
        s'orienter en direction de (180)
        déplacer de (4) pas
    fin
+ si <touche [flèche droite v] enfoncée? > alors
        s'orienter en direction de (90)
        déplacer de (4) pas
    fin
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---