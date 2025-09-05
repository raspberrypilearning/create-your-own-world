## Portes et clés

Maintenant tu vas ajouter du code pour que certaines des portes de ton monde de jeu soient verrouillées, et le joueur doit trouver la clé pour les ouvrir et arriver à la pièce suivante.

\--- task \---

Change au lutin `clé`. Clique sur `montrer`{:class="blocklooks"} dans le menu Scripts pour que le sprite apparaisse sur la scène.

\--- /task \---

\--- task \---

Modifier le costume du lutin `clé` pour qu’il soit bleu.

\--- /task \---

\--- task \---

Change l'arrière plan du scène de la salle 3, et met le lutin `clé` quelque part difficile à atteindre !

![capture d'écran](images/world-key.png)

\--- /task \---

\--- task \---

Ajouter du code au lutin `clé` pour qu'il n'est visible que dans la salle 3.

\--- /task \---

\--- task \---

Crée une nouvelle liste appelée `inventaire`{:class="block3variables"} pour stocker les objets que ton sprite `joueur` collecte.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

Le code pour ramasser la clé est très similaire au code pour ramasser des pièces. La différence est que tu ajoutes la clé à `l'inventaire`{:class="block3variables"}.

![clé](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```

\--- /task \---

\--- task \---

Ajoute du code sur ta scène pour vider ton inventaire au début de la partie.

```blocks3
delete all of [inventory v]
```

\--- /task \---

\--- task \---

Teste ton jeu pour vérifier si tu peux collecter le sprite `clé` et l'ajouter à ton inventaire.

\--- /task \---

\--- task \---

Ajoutons maintenant la porte verrouillée. Sélectionne le sprite `porte-bleue` et clique sur `montrer`{:class="blocklooks} dans le menu Scripts, puis positionne le sprite sur l'interstice entre les deux murs.

![capture d'écran](images/world-door.png)

\--- /task \---

\--- task \---

Ajouter du code au lutin `porte bleue` pour qu'il n'est visible que dans la salle 3.

\--- /task \---

\--- task \---

Ajoute du code au sprite `porte-bleue` de sorte que, lorsque la clé est dans `l'inventaire`{:class="block3variables"}, le sprite `se cache`{:class="block3looks"} pour permettre à ton sprite `joueur` de passer.

![porte](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \---

Teste ton projet et vois si tu peux récupérer la clé bleue pour ouvrir la porte !

\--- /task \---