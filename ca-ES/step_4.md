## Mou-te pel teu món

El personatge del `jugador` hauria de poder entrar per les portes a altres habitacions.

El teu projecte conté escenaris per a habitacions addicionals:

![captura de pantalla](images/world-backdrops.png)

--- task ---

Crea una nova variable "per a tots els personatges" anomenada `habitació`{:class="block3variables"} per fer un seguiment de en quina habitació està el personatge del `jugador`.

[[[generic-scratch3-add-variable]]]

![captura de pantalla](images/world-room.png)

--- /task ---

--- task ---

Quan el personatge del `jugador` toca la porta taronja a la primera habitació, el joc hauria de mostrar el següent decorat i el personatge del `jugador` hauria de tornar al costat esquerre de l'Escenari. Afegeix aquest codi dins del bucle `per sempre`{:class="block3control"} del personatge del `jugador`:

![jugador](images/player.png)

```blocks3
when flag clicked
per sempre
    si < tecla (fletxa amunt v) premuda? > llavors
        apunta en direcció (0)
        mou-te (4) passos
    fi
    si < tecla (fletxa esquerra v) premuda? > llavors
        apunta en direcció (-90)
        mou-te (4) passos
    fi
    si < tecla (fletxa avall v) premuda? > llavors
        apunta en direcció (-180)
        mou-te (4) passos
    fi
    si < tecla [fletxa dreta v] premuda? > llavors
        apunta en direcció (90)
        mou-te (4) passos
    fi
    si < tocant el color [#BABABA]? > llavors
        mou-te (-4) passos
    fi
+   si < tocant color [#F2A24A] > llavors
        canvia el fons a (següent fons de pantalla v)
        vés a x: (-200) y: (0)
        augmenta [habitació v] en (1)
    end
end
```

--- /task ---

--- task ---

Cada cop que comença el joc, cal restablir l'habitació, la posició del personatge i el fons.

Afegeix codi a l'**inici** del codi del teu personatge `jugador` per sobre del bucle `per sempre`{:class="block3control"}, per restablir-ho tot quan es faci clic a la bandera:

--- hints ---


--- hint ---

Quan el joc comença:

+ El valor d'`habitació`{:class="block3variables"} s'ha de definir a `1`{:class="block3variables"}
+ El `fons`{:class="block3looks"} s'ha de definir a `habitació1`{:class="block3looks"}
+ La posició del personatge del `jugador` s'ha de definir a `x: -200 y: 0`{:class="block3motion"}

--- /hint ---

--- hint ---

Aquí tens els blocs addicionals que necessites:

![jugador](images/player.png)

```blocks3
vés a x: (-200) y: (0)

assigna a [habitació1 v] el valor (1)

canvia el fons a (habitació1 v)
```

--- /hint ---

--- hint ---

Així és com s'hauria de veure el teu codi una vegada acabat:

![jugador](images/player.png)

```blocks3
when flag clicked
+assigna a [habitació v] el valor (1)
+vés a x: (-200) y: (0)
+canvia el fons a (habitació1 v)
per sempre
    si < tecla (fletxa amunt v) premuda? > llavors
        apunta en direcció (0)
        mou-te (4) passos
    fi
    si < tecla (fletxa esquerra v) premuda? > llavors
        apunta en direcció (-90)
        mou-te (4) passos
    fi
    si < tecla (fletxa avall v) premuda? > llavors
        apunta en direcció (-180)
        mou-te (4) passos
    fi
    si < tecla [fletxa dreta v] premuda? > llavors
        apunta en direcció (90)
        mou-te (4) passos
    fi
    si < tocant el color [#BABABA]? > llavors
        mou-te (-4) passos
    fi
    si < tocant el color [#F2A24A]? > llavors
        canvia el fons a (següent fons de pantalla v)
        vés a x: (-200) y: (0)
        augmenta [habitació v] en (1)
    end
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Fes clic a la bandera i, a continuació, mou el teu personatge de `jugador` fins que toqui la porta taronja. El personatge passa a la pantalla següent? La variable `habitació`{:class="block3variables"} canvia a `2`?

![captura de pantalla](images/world-room-test.png)

--- /task ---