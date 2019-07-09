## Panneaux

Ajoutez maintenant des signes à votre monde pour guider les joueurs dans leur voyage.

Ton project inclut un `panneau de bienvenue` sprite :

![capture d'écran](images/world-sign.png)

\--- \--- tâche Le `signe de bienvenue` sprite ne devrait être visible dans la chambre 1, il faut donc ajouter un code à l'image - objet pour vous assurer que cela se produit:

\--- astuces \--- \--- astuces \--- `Lorsque le drapeau est cliqué`{: class = "block3events"}, dans une boucle `toujours`{: class = "block3control"}, cochez `si`{: class = "block3control"} la `chambre est 1`{: class = "block3variables"} et dans ce cas, `affiche`{: class = "block3looks"} `signe de bienvenue` sprite, `sinon`{: class = "block3control"} `masquer`{: class = "block3looks"} le sprite. \--- / allusion \--- \--- allusion \--- Voici les blocs dont vous avez besoin:

![signe](images/sign.png)

```blocks3
<br />si &lt; &gt; alors
sinon
fin

&lt; (salle :: variables) = [1] &gt;

masquer

montrer

pour toujours
fin

lorsque le drapeau est cliqué

```

\--- / hint \--- \--- hint \--- Voici le code complet:

![signe](images/sign.png)

```blocks3
lorsque le drapeau est cliqué sur
pour toujours
    si < (room :: variables) = [1] > puis
        affichent
    sinon
        masquer
    fin
fin
```

\--- / allusion \--- \--- / allusions \---

\--- /task \---

\--- tâche \--- Testez le code de votre `panneau de bienvenue` en passant d'une pièce à une autre. Le panneau ne devrait être visible que dans la salle 1.

![capture d'écran](images/world-sign-test.png) \--- /task \---

\--- tâche \--- Un signe n'est pas très bon s'il ne dit rien! Ajoute du code supplémentaire pour afficher un message si le sprite `panneau de bienvenue` touche le sprite `du joueur`:

![signe](images/sign.png)

```blocks3
lorsque le drapeau est cliqué sur
pour toujours
si < (salle :: variables) = [1] > puis
indiquent
sinon
masquer
fin
+ si < contacts (joueur v)? > puis
dire [Bienvenue! Pouvez-vous aller au trésor?]
sinon
dire []
fin
fin
```

\--- /task \---

\--- tâche \--- Testez à nouveau votre `signe de bienvenue` sprite. Vous devriez maintenant voir un message lorsque le sprite `joueur` touche le signe `bienvenue` sprite.

![capture d'écran](images/world-sign-test2.png) \--- /task \---