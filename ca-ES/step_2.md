## Mou la icona del jugador

Comença per crear una icona ` jugador ` que pot moure's pel teu món.

\--- task \---

Obre el projecte d'arrencada de Scratch "Crea el teu propi món".

** en línia: ** obre el projecte d'inici a [ rpf.io/create-your-own-world-on ](http://rpf.io/create-your-own-world-on) {: target = "_ blank"}.

Si tens un compte a Scratch pots fer una còpia fent clic a **Reinventa**.

** Fora de línia: ** descarrega el projecte d'inici de [ rpf.io/p/en/create-your-own-world-go ](http://rpf.io/p/en/create-your-own-world-go) {: target = "_ blank"} i, a continuació, obre'l utilitzant l'editor fora de línia. Si necessites descarregar i instal·lar l'editor fora de línia d'Scratch, el pots trobar a [ rpf.io/scratchoff ](https://rpf.io/scratchoff).\--- /task"}.

![captura de pantalla](images/world-starter.png)

\--- /task \---

Prement les tecles de fletxa mouràs la icona ` jugador `tot al voltant. En prémer la fletxa cap amunt, la icona ` jugador ` respondrà movent-se cap amunt a l'escenari.

\--- task \---

Afegeix aquest codi a la icona `jugador `:

![jugador](images/player.png)

```blocks3
quan has fet clic a la bandera
per sempre
    si has apretat <tecles (fletxa amunt v)? > llavors
        punt de direcció (0)
        moure (4) passes
    fi
final
```

\--- /task \---

\--- task \---

Fes clic a la bandera i, a continuació, manté premuda la fletxa amunt. La icona `jugador ` es mou cap amunt?

![captura de pantalla](images/world-up.png)

\--- /task \---

\--- task \---

Per moure la icona `jugador ` a l'esquerra, has d'afegir un altre ` si ` {: class = "block3control"} bloc amb un codi similar:

![jugador](images/player.png)

```blocks3
quan has fet clic a la bandera
per sempre
    si has apretat <tecles (fletxa amunt v)? > llavors
        punt de direcció (0)
        moure (4) passes
    final
+ si has apretat <tecles (fletxa esquerra v)? > llavors
        punt de direcció (-90)
        moure (4) passes
    fi
final
```

\--- /task \---

\--- task \---

Afegeix més codi a la teva icona `jugador ` perquè també es pugui moure cap a baix i cap a la dreta. Utilitza el codi que ja tens per ajudar-te.

\--- hints \---

\--- hint \---

Per pujar cap amunt, apunta la icona ` jugador ` en la direcció ` 0 ` graus. Què ha de fer per fer baixar la icona?

Per moure'l cap a l'esquerra, apunta la icona jugador en la direcció ` -90 ` graus. Què has de fer per moure la icona cap a la dreta?

\--- /hint \---

\--- hint \---

Has de canviar aquests dos blocs:

![jugador](images/player.png)

```blocks3
<key ( v) pressed>

apunta en direcció ()
```

Duplica el codi que fa que la icona ` jugador ` es desplaçi cap amunt i canvia aquests dos blocs per fer què la icona es mogui cap avall. Duplica el codi de nou i canvia'l per tal què la icona es desplaci cap a la dreta.

\--- /hint \--- \--- hint \--- Això és el que hauria de tenir el teu codi:

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
        punt de direcció (180)
        moure (4) passes
    final
  si has apretat <tecles [fletxa dreta v]? > llavors
        punt de direcció (90)
        moure (4) passes
    fi
final
```

\--- /hint \--- \--- /hints \---

\--- /task \---