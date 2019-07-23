## Collecter des pièces

Ton sprite `joueur` devrait pouvoir collecter des pièces lorsqu'il se déplace dans le monde.

\--- task \--- Ajouter une nouvelle variable appelée `pièces`{:class="block3variables"} à ton projet. \--- /task \---

\--- task \--- Sélectionne le sprite `pièce` et clique sur **afficher**.

![capture d'écran](images/coin.png) \--- /task \---

\--- tâche \--- Ajoute le code à ta `pièce` sprite afin qu'elle n'apparaisse que dans la salle 1. ![capture d'écran](images/coin.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
si <(salle :: variables) =[1]> alors
montrer 
sinon
cacher
```

\--- /task \---

\--- task \---

Ajoute du code à ton sprite `pièce` de façon à ce que le sprite `se cache`{:class="block3looks"} et `1`{:class="block3variables"} soit ajouté à la variable `pièces`{:class="block3variables"} une fois que le sprite `joueur` touche le sprite `pièce` pour le «ramasser».

![pièce de monnaie](images/coin.png)

```blocks3
quand le drapeau est cliqué 
attendre jusque <touching (player v)?>
changez [pièces v] par (1)
masquer
arrêtez [autres scripts dans le sprite v]
```

Le code `stop d'autres scripts du sprite`{: class = "block3control"} est nécessaire pour que le sprite `pièce` ne soit plus affiché dans la salle 1 une fois qu’elle a été collectée.

\--- /task \---

\--- task \--- Ajoute maintenant du code sur la scène pour définir ta variable `pièces`{: class = "block3variables"} à `0`{: class = "block3variables"} au début du jeu.

![scène](images/stage.png)

```blocks3
quand le drapeau est cliqué
définir [pièces v] à [0]
```

\--- /task \---

\--- task \--- Teste ton jeu. La collecte d'une pièce devrait changer ton `pièces` score en `1`{: class = "block3variables"}. \--- /task \---