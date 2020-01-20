## Les personnes

Ajoute d'autres personnes à ton monde avec lesquelles ton sprite `joueur` peut interagir.

\--- task \---

Switch to the `person` sprite.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

Add some code to the `person` sprite so that the person talks to the `player` sprite. This code is very similar to the code you added to your `sign` sprite:

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

\--- /task \---

\--- task \---

Allow your `person` sprite to move by adding these two blocks in the `else`{:class="block3control"} section of your code:

![person](images/person.png)

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

\--- /task \---

Your `person` sprite will now move, but will stop to talk to the `player` sprite.

![screenshot](images/world-person-test.png)

\--- task \---

Add code to your new `person` sprite so that the sprite only appears in room 1. The code you need is exactly the same as the code that makes the `sign` sprite only visible in room 1.

Make sure you test out your new code.

\--- /task \---