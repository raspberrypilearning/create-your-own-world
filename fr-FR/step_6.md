## Panneaux

Ajoute maintenant des signes à ton monde pour guider les joueurs dans leur voyage.

Ton project inclut un `panneau de bienvenue` sprite :

![capture d'écran](images/world-sign.png)

\--- task \--- Le sprite `panneau de bienvenue` ne devrait être visible que dans la salle 1, alors ajoute un code au sprite pour s'assurer que cela se passe :

\--- hints \--- \--- hint \--- `Lorsque le drapeau est cliqué`{: class = "block3events"}, dans une boucle `répéter indéfiniment`{: class = "block3control"}, vérifie `si`{: class = "block3control"} la `salle est 1`{: class = "block3variables"} et dans ce cas, `affiche`{: class = "block3looks"} le sprite`panneau de bienvenue`, `sinon`{: class = "block3control"} `masquer`{: class = "block3looks"} le sprite. \--- /hint \--- \--- hint \--- Voici les blocs que tu as besoin :

![signe](images/sign.png)

```blocks3
<br />si &lt; &gt; alors
sinon
fin

&lt; (salle :: variables) = [1] &gt;

masquer

montrer

répéter indéfiniment
fin

lorsque le drapeau est cliqué

```

\--- / hint \--- \--- hint \--- Voici le code complet:

![signe](images/sign.png)

```blocks3
lorsque le drapeau est cliqué 
répéter indéfiniment
    si < (salle :: variables) = [1] > alors
        afficher
    sinon
        masquer
    fin
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Teste le code de ton sprite `panneau de bienvenue` en passant d'une salle à une autre. Le panneau ne devrait être visible que dans la salle 1.

![capture d'écran](images/world-sign-test.png) \--- /task \---

\--- task \--- Un panneau n'est pas très bon s'il ne dit rien! Ajoute du code supplémentaire pour afficher un message si le sprite `panneau de bienvenue` touche le sprite `du joueur`:

![signe](images/sign.png)

```blocks3
lorsque le drapeau est cliqué 
répéter indéfiniment
si < (salle :: variables) = [1] > alors
montrer
sinon
masquer
fin
+ si < touchant (joueur v)? > alors
dire [Bienvenue!] Pouvez-vous aller au trésor?]
sinon
dire []
fin
fin
```

\--- /task \---

\--- tâche \--- Testez à nouveau votre `signe de bienvenue` sprite. Vous devriez maintenant voir un message lorsque le sprite `joueur` touche le signe `bienvenue` sprite.

![capture d'écran](images/world-sign-test2.png) \--- /task \---