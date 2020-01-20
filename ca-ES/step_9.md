## Repte: afegeix un enemic

Si vols, també pots afegir patrulles d'enemics al vostre joc. Si la icona del `jugador ` toca un enemic, el joc s’acaba.

+ El teu joc ja conté una icona d' `enemic `. Afegeix codi a la teva icona d' `enemic` de manera que només aparegui a l'habitació 2.

+ Afegeix codi per moure la icona `enemic ` i per acabar el joc si l'` enemic ` toca el ` jugador`. És més fàcil fer-ho en blocs de codi separats. Aquí tenses podria veure el teu codi de la icona ` enemic `:

```blocks3
quan has fet clic a la bandera
per sempre
si <(habitació :: variables) =[2]> llavors
mostrar
si no
amagar

quan has fet clic a la bandera
per sempre
si <touching (player v)?> llavors
aturar [tot v]

quan has fet clic a la bandera
anar a x : (170) y: (0)
per sempre
repetir (130)
canviar x per (-1)
final
repetir (130)
canviar x per (1)
```

+ Prova el teu nou codi per assegurar-te que: 
    + La icona ` enemic ` només és visible a l'habitació 2
    + La icona ` enemic ` es mou per tota l'habitació
    + El joc s’acaba si la icona `jugador ` toca la icona ` enemic `

Pots crear una altra icona `enemic ` a l'habitació 3 que fa ronda amunt i avall per l'escletxa de la paret?

![captura de pantalla](images/world-enemy2.png)