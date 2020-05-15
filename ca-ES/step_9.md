## Repte: afegeix un enemic

Si vols, també pots afegir patrulles d'enemics al teu joc. Si el personatge del `jugador` toca un enemic, el joc s’acaba.

+ El teu joc ja conté un personatge d'`enemic`. Afegeix codi al teu personatge d'`enemic` de manera que només aparegui a l'habitació 2.

+ Afegeix codi per moure el personatge `enemic` i per acabar el joc si l'`enemic `toca el personatge del `jugador`. És més fàcil fer-ho en blocs de codi separats. Aquí tens com hauria de ser el codi del personatge `enemic`:

```blocks3
when flag clicked
per sempre
si <(habitació :: variables) =[2]> llavors
mostra't
si no
amaga't

when flag clicked
per sempre
si <touching (player v)?> llavors
atura [tot v]

when flag clicked
vés a x: (170) y:(0)
per sempre
repeteix (130)
suma (-1) a x
fi
repeteix (130)
suma (1) a x
```

+ Prova el teu nou codi per assegurar-te que: 
    + El personatge `enemic` només és visible a l'habitació 2
    + El personatge `enemic` es mou per tota l'habitació
    + El joc s’acaba si el personatge `jugador` toca el personatge `enemic`

Pots crear un altre personatge `enemic` a l'habitació 3 que faci ronda amunt i avall per l'escletxa de la paret?

![captura de pantalla](images/world-enemy2.png)