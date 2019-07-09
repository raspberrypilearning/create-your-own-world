## Les portes et les clés

Vous allez maintenant ajouter du code pour que certaines des portes de votre monde de jeu soient verrouillées, et le joueur doit trouver la clé pour les ouvrir et accéder à la pièce suivante.

\--- task \--- Basculez sur le sprite `touche`. Cliquez sur `show`{: class = "blocklooks"} dans le menu Scripts pour que le sprite apparaisse sur la scène. \--- /task \---

\--- tâche \--- Modifier le `clé` costume de lutin de sorte qu'il est bleu. \--- /task \---

\--- tâche \--- Basculez votre décor de scène sur la salle 3 et placez le sprite `clé` endroit difficile à atteindre!

![capture d'écran](images/world-key.png)

\--- /task \---

\--- tâche \--- Ajoutez du code à l'image-clé `clé` pour le rendre visible uniquement dans la salle 3. \--- /task \---

\--- tâche \--- Créez une nouvelle liste appelée `inventaire`{: class = "block3variables"} pour stocker les objets que votre sprite `joueurs` collectionne.

[[[generic-scratch3-make-list]]] \--- / tâche \---

\--- task \--- Le code que vous devez ajouter pour collecter la clé est très similaire au code pour collecter des pièces. La différence est que vous ajoutez la clé à l'inventaire ``{: class = "block3variables"}.

![clé](images/key.png)

```blocks3
lorsque l'indicateur a cliqué sur
attendez jusqu'à ce que <touching (player v)?>
ajoute la [touche bleue] à [inventaire v]
masque
arrêtez [autres scripts dans l'image-objet v]
```

\--- /task \---

\--- tâche \--- Ajoutez du code sur votre scène pour vider votre inventaire au début de la partie.

```blocks3
supprimer l'élément (tout v) de la liste [inventaire v]
```

\--- /task \---

\--- task \--- Testez votre jeu pour vérifier si vous pouvez collecter le sprite `clé` et l'ajouter à votre inventaire. \--- /task \---

\--- tâche \--- Ajoutez maintenant la porte verrouillée. Sélectionnez le sprite `door-blue` et cliquez sur `show`{: class = "blocklooks} dans le menu Scripts, puis positionnez le sprite sur l'interstice entre les deux murs.

![capture d'écran](images/world-door.png) \--- /task \---

\--- task \--- Ajoutez du code dans le sprite `door-blue` afin qu'il ne soit visible que dans la salle 3. \--- /task \---

\--- tâche \--- Ajoute du code au sprite `door-blue` sorte que, lorsque la clé est dans l'inventaire ``: (class = "block3variables"}), le lutin `cache`{: class = "block3looks "} pour permettre à votre sprite de `joueurs` de passer.

![porte](images/door.png)

```blocks3
lorsque le drapeau est cliqué sur
attendez que <[inventaire v] contienne [clé bleue]>
stop [autres scripts dans sprite v]
masquer
```

\--- /task \---

\--- tâche \--- Testez votre jeu et voyez si vous pouvez récupérer la clé bleue pour ouvrir la porte! \--- /task \---