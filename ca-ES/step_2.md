## Mou el personatge del jugador

Comença per crear un personatge `jugador` que pugui moure's pel teu món.

--- task ---

Obre el projecte d'arrencada de Scratch "Crea el teu propi món".

**En línia**: obre el projecte d'inici a [scratch.mit.edu/projects/395712734](https://scratch.mit.edu/projects/395712734){:target="_blank"}.

Si tens un compte a Scratch pots fer una còpia fent clic a **Reinventa**.

**Fora de línia:** descarrega el projecte d'inici de [rpf.io/p/ca-ES/create-your-own-world-go](http://rpf.io/p/ca-ES/create-your-own-world-go){:target="_blank"} i, a continuació, obre'l utilitzant l'editor fora de línia. Si necessites descarregar i instal·lar l'editor fora de línia d'Scratch, el pots trobar a [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![captura de pantalla](images/world-starter.png)

--- /task ---

Prement les tecles de fletxa hauries de moure el personatge del `jugador` pels voltants. En prémer la fletxa cap amunt, el personatge del `jugador` hauria de moure's cap a l'Escenari com a resposta.

--- task ---

Afegeix aquest codi al personatge del `jugador`:

![jugador](images/player.png)

```blocks3
when flag clicked
per sempre
    si <tecla (fletxa amunt v) premuda? > llavors
        apunta en direcció (0)
        mou-te (4) passos
    fi
fi
```

--- /task ---

--- task ---

Fes clic a la bandera i, a continuació, mantén premuda la fletxa amunt. El personatge del `jugador` es mou cap amunt?

![captura de pantalla](images/world-up.png)

--- /task ---

--- task ---

Per moure el personatge del `jugador` a l'esquerra, has d'afegir un altre bloc `si`{:class="block3control"} amb un codi com aquest:

![jugador](images/player.png)

```blocks3
when flag clicked
per sempre
    si <tecla (fletxa amunt v) premuda? > llavors
        apunta en direcció (0)
        mou-te (4) passos
    fi
+   si <tecla (fletxa esquerra v) premuda? > llavors
        apunta en direcció (-90)
        mou-te (4) passos
    fi
fi
```

--- /task ---

--- task ---

Afegeix més codi al teu personatge del `jugador` perquè també es pugui moure cap a baix i cap a la dreta. Utilitza el codi que ja tens per ajudar-te.

--- hints ---


--- hint ---

Per pujar cap amunt, apunta el personatge del `jugador` en la direcció `0` graus. Què has de fer per fer baixar el personatge?

Per moure'l cap a l'esquerra, apunta el personatge en la direcció `-90` graus. Què has de fer per moure el personatge cap a la dreta?

--- /hint ---

--- hint ---

Has de canviar aquests dos blocs:

![jugador](images/player.png)

```blocks3
<key ( v) pressed>

apunta en direcció ()
```

Duplica el codi que fa que el personatge del `jugador` es desplaci cap amunt i canvia aquests dos blocs per fer què el personatge es mogui cap avall. Duplica el codi de nou i canvia'l per tal què el personatge es desplaci cap a la dreta.

--- /hint ---

--- hint ---

Així és com s'hauria de veure el teu codi:

![jugador](images/player.png)

```blocks3
when flag clicked
per sempre
    si <tecla (fletxa amunt v) premuda? > llavors
        apunta en direcció (0)
        mou-te (4) passos
    fi
    si <tecla (fletxa esquerra v) premuda? > llavors
        apunta en direcció (-90)
        mou-te (4) passos
    fi

+   si <tecla (fletxa avall v) premuda? > llavors
        apunta en direcció (180)
        mou-te (4) passos
    fi
+   si <tecla (fletxa dreta v) premuda? > llavors
        apunta en direcció (90)
        mou-te (4) passos
    fi
fi
```

--- /hint ---

--- /hints ---

--- /task ---