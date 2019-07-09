## Collecter des pièces

Votre `joueur` sprite devrait pouvoir collecter des pièces lorsqu'il se déplace dans le monde.

\--- tâche \--- Ajouter une nouvelle variable alimentée `pièces de monnaie`{: class = "block3variables"} à votre projet. \--- /task \---

\--- tâche \--- Sélectionnez le sprite `coin` et cliquez sur **afficher**.

![capture d'écran](images/coin.png) \--- /task \---

\--- tâche \--- Ajoutez le code à votre `pièce` sprite afin qu'il n'apparaisse que dans la salle 1. ![capture d'écran](images/coin.png)

```blocks3
lorsque le drapeau est cliqué sur
pour toujours
si <(room :: variables) =[1]> puis
affichent
sinon
masquer
```

\--- /task \---

\--- task \---

Ajoutez du code à votre image-objet `pièce` façon à ce que l'image-objet `masque`{: class = "block3looks"} et `1`{: class = "block3variables"} est ajouté aux `pièces`{: class = "block3variables"} variable une fois que le sprite `joueurs` touche le sprite `pièces` pour le «ramasser».

![pièce de monnaie](images/coin.png)

```blocks3
quand flag a cliqué sur
attendez <touching (player v)?>
changez [pièces v] par (1)
masquer
arrêtez [autres scripts dans le sprite v]
```

Le code `stop autres scripts de l’image-objet`{: class = "block3control"} est nécessaire pour que l’image-objet `coin` ne soit plus affichée dans la salle 1 une fois qu’elle a été collectée.

\--- /task \---

\--- tâche \--- Ajoutez maintenant du code sur la scène pour définir votre variable `pièces`{: class = "block3variables"} à `0`{: class = "block3variables"} au début du jeu.

![étape](images/stage.png)

```blocks3
quand le drapeau a cliqué
set [pièces v] à [0]
```

\--- /task \---

\--- tâche \--- Testez votre jeu. La collecte d'une pièce de monnaie devrait changer vos `pièces` score en `1`{: class = "block3variables"}. \--- /task \---