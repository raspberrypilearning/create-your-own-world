## Les personnes

Ajoute d'autres personnes à ton monde avec lesquelles ton sprite `joueur` peut interagir.

--- task --- Basculez vers le sprite `personne`.

![Personne sprite](images/person.png) --- /task ---

--- task --- Ajoute du code au sprite `personne` pour que la personne parle au sprite `joueur`. Ce code est très similaire à celui que tu as ajouté à ton sprite `panneau`:

![personne](images/person.png)

```blocks3
lorsque le drapeau est cliqué
aller à x: (0) y: (-150)
répéter indéfiniment
    si < touche le (joueur v)? > alors
        dire [Saviez-vous que vous pouvez passer par les portes orange et jaune?]
    sinon
        dire []
    end
end
```

--- /task ---

--- task --- Permet à ton sprite `personne` de se déplacer en ajoutant ces deux blocs à la section `sinon`{:class="block3control"} de ton code:

![personne](images/person.png)

```blocks3
lorsque le drapeau est cliqué 
aller à x: (0) y: (-150)
répéter indéfiniment
    si < touche le (joueur v)? > alors
        dire [Sais-tu que tu peux passer par les portes orange et jaune?]
    sinon
        dire []
+        avancer de (1) pas
+        rebondir si le bord est atteint
    end
end

```

--- /task ---

Ton sprite `personne` va maintenant bouger, et va s'arrêter pour parler au sprite `joueur`.

![capture d'écran](images/world-person-test.png)

--- task --- Ajoute le code à ton nouveau sprite `personne` afin que ce dernier n'apparaisse que dans la salle 1. Le code dont tu as besoin est exactement le même que le code qui rend le sprite `panneau` visible seulement dans la chambre 1.

Assure-toi de tester ton nouveau code. --- /task ---