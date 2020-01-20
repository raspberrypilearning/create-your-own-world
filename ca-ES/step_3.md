## Murs massissos

\--- task \--- Prova la teva icona `jugador ` de nou. Veus que pot caminar per les parets de color gris clar.

![captura de pantalla](images/world-walls.png) \--- /task \---

\--- task \--- Per solucionar-ho, has de fer que la icona `jugador ` es desplaçi enrere si toca una paret de color gris clar. Aquí tens el codi que cal afegir dins del teu ` per sempre ` {: class = "block3control"} bloc sota els blocs de direcció:

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
+ si < tocant el color [#BABABA]? > llavors
    moure (-4) passes
    final
final
```

\--- /task \---

\--- task \---

Prova de fer moure la icona ` jugador ` per una paret. Si el teu codi nou funciona, això no hauria de ser possible.

![captura de pantalla](images/world-walls-test.png) \--- /task \---