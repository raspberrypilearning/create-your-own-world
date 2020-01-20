## Mou-te pel teu món

La icona `jugador ` hauria de poder entrar per les portes a altres habitacions.

El teu projecte conté escenaris per a habitacions addicionals:

![captura de pantalla](images/world-backdrops.png)

\--- task \---

Crea una nova variable "per a totes les icones" anomenada ` habitació ` {: class = "block3variables"} per fer un seguiment de en quina habitació està la icona ` jugador`.

[[[generic-scratch3-add-variable]]]

![captura de pantalla](images/world-room.png) \--- /task \---

\--- task \--- Quan la icona `jugador ` toca la porta taronja a la primera habitació, el joc hauria de mostrar el següent decorat i la icona del `jugador ` hauria de tornar al costat esquerre de l'escenari. Afegeix aquest codi dins del bucle ` per sempre `{: class = "block3control"} de la icona `jugador `:

![jugador](images/player.png)

```blocks3
quan has fet clic a la bandera
per sempre
    si has apretat <tecles (fletxa amunt v)? > llavors
        punt de direcció (0)
        moure (4) passes
    final
  si has apretat <tecles (fletxa esquerra v)? > llavors
        punt de direcció (-90)
        moure (4) passes
    final
  si has apretat <tecles (fletxa avall v)? > llavors
        punt de direcció (-180)
        moure (4) passes
    final
  si has apretat <tecles [fletxa dreta v]? > llavors
        punt de direcció (90)
        moure (4) passes
    final
 si < tocant el color [#BABABA]? > llavors
    moure (-4) passes
    final
+ si < tocant color [# F2A24A] > llavors
    canviar el teló de fons a (següent teló de fons v)
    anar a x: (-200) y: (0)
    canviar [habitació v] per (1)
    final
final
```

\--- /task \---

\--- task \--- Cada cop que comença el joc, cal restablir l'habitació, la posició del personatge i el teló de fons.

Afegeix codi al **inici ** del codi de la teva icona de `jugador ` per sobre del bucle ` per sempre `{: class = "block3control"}, per restablir-ho tot quan es faci clic a la bandera:

\--- hints \--- \--- hint \--- Quan comença el joc:

+ El valor de ` habitació ` {: class = "block3variables"} s'ha de definir a ` 1 ` {: class = "block3variables"}
+ El ` telo de fons ` {: class = "block3variables"} s'ha de definir a ` habitació 1 ` {: class = "block3variables"}
+ La posició dela icona del ` personatge ` s'ha de definir a ` x: -200 y: 0 ` {: class = "block3motion"} \--- / hint \--- \--- hint \--- Aquests són els blocs addicionals que necessites:

![jugador](images/player.png)

```blocks3
ves a x: (-200) y: (0)

estableix [habitació v] a (1)

canvia el teló de fons a (habitació1 v)
```

\--- /hint \--- \--- hint \--- Això és el que hauria de tenir el teu codi:

![jugador](images/player.png)

```blocks3
quan has fet clic a la bandera
+ estableix [habitació v] a (1)
+ ves a x: (-200) y: (0)
+ canvia el teló de fons a (sala1 v)
per sempre
    si has apretat <tecles (fletxa amunt v)? > llavors
        punt de direcció (0)
        moure (4) passes
    final
  si has apretat <tecles (fletxa esquerra v)? > llavors
        punt de direcció (-90)
        moure (4) passes
    final
  si has apretat <tecles (fletxa avall v)? > llavors
        punt de direcció (-180)
        moure (4) passes
    final
  si has apretat <tecles [fletxa dreta v]? > llavors
        punt de direcció (90)
        moure (4) passes
    final
 si < tocant el color [#BABABA]? > llavors
    moure (-4) passes
    final
+ si < tocant color [# F2A24A] > llavors
    canviar el teló de fons a (següent teló de fons v)
    anar a x: (-200) y: (0)
    canviar [habitació v] per (1)
    final
final
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Fes clic a la bandera i, a continuació, mou la icona del teu `jugador ` fins que toqui la porta taronja. La icona passa a la pantalla següent? La `habitació ` {: class = "block3variables"} variable canvia a ` 2 `?

![captura de pantalla](images/world-room-test.png) \--- /task \---