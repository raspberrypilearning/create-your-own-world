## Gent

Afegeix altres persones al teu món amb les que el teu personatge `jugador` pugui interaccionar.

--- task ---

Canvia al personatge `persona`.

![Personatge de persona](images/person.png)

--- /task ---

--- task ---

Afegeix algun codi al personatge `persona` de manera que parli amb el personatge `jugador`. Aquest codi és molt similar al que has afegit al teu personatge `senyal`:

![persona](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
	if < touching (jugador v)? > then
		say [Sabies que pots passar per les portes taronges i grogues?]
	else
		say []
	end
end
```

--- /task ---

--- task ---

Permet al teu personatge `persona` moure's afegint aquests dos blocs a la secció `si no`{:class="block3control"} del teu codi:

![persona](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
	if < touching (jugador v)? > then
		say [Sabies que pots passar per les portes taronges i grogues?]
	else
		say []
+		move (1) steps
+		if on edge, bounce
	end
end
```

--- /task ---

El teu personatge `persona` ara es mourà, però s’aturarà per parlar amb el personatge del `jugador`.

![captura de pantalla](images/world-person-test.png)

--- task ---

Afegeix codi al teu personatge `persona` de manera que aquest només aparegui a l'habitació 1. El codi que necessites és exactament el mateix que el que fa el personatge del `senyal` només visible a l'habitació 1.

Assegura't de provar el nou codi.

--- /task ---