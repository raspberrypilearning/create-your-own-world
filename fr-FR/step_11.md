## Les portes et les clés

Tu vas maintenant ajouter du code pour que certaines des portes de ton monde de jeu soient verrouillées, et le joueur doit trouver la clé pour les ouvrir et accéder à la pièce suivante.

\--- task \--- Bascule sur le sprite `clé`. Clique sur `montrer`{: class = "blocklooks"} dans le menu Scripts pour que le sprite apparaisse sur la scène. \--- /task \---

\--- task \--- Modifie le costume du sprite `clé` de sorte qu'il soit bleu. \--- /task \---

\--- task \--- Bascule ton décor de scène sur la salle 3 et placez le sprite `clé` à un endroit difficile à atteindre!

![capture d'écran](images/world-key.png)

\--- /task \---

\--- task \--- Ajoute du code au sprite `clé` pour le rendre visible uniquement dans la salle 3. \--- /task \---

\--- task \--- Crée une nouvelle liste appelée `inventaire`{: class = "block3variables"} pour stocker les objets que ton sprite `joueur` collecte.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- task \--- Le code que tu dois ajouter pour collecter la clé est très similaire au code pour collecter des pièces. La différence est que tu ajoutes la clé à `l'inventaire`{: class = "block3variables"}.

![clé](images/key.png)

```blocks3
lorsque le drapeau est cliqué
attendre jusqu'à <touching (player v)?>
ajoute la [touche bleue] à [inventaire v]
masquer
arrêtez [autres scripts dans le sprite v]
```

\--- /task \---

\--- task \--- Ajoute du code sur ta scène pour vider ton inventaire au début de la partie.

```blocks3
supprimer l'élément (tout v) de la liste [inventaire v]
```

\--- /task \---

\--- task \--- Teste ton jeu pour vérifier si tu peux collecter le sprite `clé` et l'ajouter à ton inventaire. \--- /task \---

\--- task \--- Ajoute maintenant la porte verrouillée. Sélectionne le sprite `porte-bleue` et clique sur `montrer`{: class = "blocklooks} dans le menu Scripts, puis positionnez le sprite sur l'interstice entre les deux murs.

![capture d'écran](images/world-door.png) \--- /task \---

\--- task \--- Ajoute du code dans le sprite `porte-bleue` afin qu'il ne soit visible que dans la salle 3. \--- /task \---

\--- task \--- Ajoute du code au sprite `porte-bleue` de sorte que, lorsque la clé est dans `l'inventaire`: {class = "block3variables"}, le sprite `cache`{:class = "block3looks"} pour permettre à ton sprite `joueur` de passer.

![porte](images/door.png)

```blocks3
lorsque le drapeau est cliqué 
attendre jusque <[inventaire v] contienne [clé bleue]>
stop [autres scripts dans le sprite v]
masquer
```

\--- /task \---

\--- task \--- Teste ton jeu et vois si tu peux récupérer la clé bleue pour ouvrir la porte! \--- /task \---