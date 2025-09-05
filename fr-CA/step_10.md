## Collecter des pièces

Ton sprite `joueur` devrait pouvoir collecter des pièces lorsqu'il se déplace dans le monde.

\--- task \---

Ajoute une nouvelle variable appelé `pièces` {:class="blockdata"} à ton projet.

\--- /task \---

\--- task \---

Fais un clic droit sur le lutin ` pièce` et choisis **montrer** .

![capture d'écran](images/coin.png)

\--- /task \---

\--- task \---

Ajouter du code au lutin `pièce` pour qu'il n'apparaisse que dans la salle 1.

![capture d'écran](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

Ajoute du code à ton sprite `pièce` de façon à ce que le sprite `se cache`{:class="block3looks"} et `1`{:class="block3variables"} soit ajouté à la variable `pièces`{:class="block3variables"} une fois que le sprite `joueur` touche le sprite `pièce` pour le «ramasser».

![pièces](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

Le code `stop autres scripts dans sprite`{:class="block3control"} est nécessaire pour que le sprite `pièce` ne soit plus affiché dans la salle 1 une fois qu’elle a été collectée.

\--- /task \---

\--- task \---

Maintenant, ajoute du code à la scène pour définir ta variable `pièces`{:class="block3variables"} à `0`{:class="block3variables"} au début du jeu.

![scène](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

Testez votre jeu. La collecte d'une pièce devrait changer ton score `pièces` en `1`{:class="block3variables"}.

\--- /task \---