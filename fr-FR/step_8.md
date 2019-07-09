## Les personnes

Ajoutez d'autres personnes à votre monde avec lesquelles votre `joueur avec` sprite peut interagir.

\--- tâche \--- Basculez vers le sprite `personne`.

![Personne sprite](images/person.png) \--- /task \---

\--- tâche \--- Ajoutez du code au sprite `personne` pour qu'il parle au sprite `joueurs` Ce code est très similaire à celui que tu as ajouté à ton sprite `panneau`:

![la personne](images/person.png)

```blocks3
lorsque le drapeau a cliqué sur
aller à x: (0) y: (-150)
pour toujours
    si < contacts (joueur v)? > puis
        dire [Saviez-vous que vous pouvez passer par les portes orange et jaune?]
    sinon
        dites []
    fin
fin
```

\--- /task \---

\--- task \--- Permettez à votre sprite `personne` de se déplacer en ajoutant ces deux blocs à la section `{`class = "block3control"} de votre code:

![la personne](images/person.png)

```blocks3
lorsque le drapeau a cliqué sur
aller à x: (0) y: (-150)
pour toujours
    si < contacts (joueur v)? > puis
        dire [Saviez-vous que vous pouvez passer par les portes orange et jaune?]
    sinon
        dites []
+ déplacez (1) étapes
+ si sur le bord, rebondissez
    bout


```

\--- /task \---

Ton sprite `personne` va maintenant bouger, et va s'arrêter pour parler au sprite `joueur`.

![capture d'écran](images/world-person-test.png)

\--- tâche \--- Ajoutez le code à votre nouveau sprite `personne` afin que ce dernier n'apparaisse que dans la salle 1. Le code dont vous avez besoin est exactement le même que le code qui rend le `signe` sprite visibles dans la chambre 1.

Assure-toi de tester ton nouveau code. \--- /task \---