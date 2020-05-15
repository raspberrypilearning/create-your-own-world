## Murs massissos

\--- task \---

Prova el teu personatge de `jugador` de nou. Do you see that it can walk through the light grey walls?

![captura de pantalla](images/world-walls.png)

\--- /task \---

\--- task \---

Per solucionar-ho, has de fer que el personatge del `jugador` es desplaci enrere si toca una paret de color gris clar. Aquí tens el codi que cal afegir dins del teu bloc `per sempre`{:class="block3control"} sota els blocs de direcció:

![jugador](images/player.png)

```blocks3
quan la bandera es cliqui
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
    si < tecla (fletxa dreta v) premuda? > llavors
        apunta en direcció (90)
        mou-te (4) passos
    fi
+   si < tocant el color [#BABABA]? > llavors
        mou-te (-4) passos
    fi
fi
```

\--- /task \---

\--- task \---

Prova de fer moure el personatge del `jugador` per una paret. Si el teu codi nou funciona, això no hauria de ser possible.

![captura de pantalla](images/world-walls-test.png)

\--- /task \---