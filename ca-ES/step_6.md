## Senyals

Ara afegeix senyals al teu món per guiar els jugadors en el seu viatge.

El teu projecte inclou un personatge de `senyal de benvinguda`:

![captura de pantalla](images/world-sign.png)

--- task ---

El personatge de `senyal de benvinguda` només hauria de ser visible a l'habitació 1, així que afegeix algun codi al personatge per assegurar-te que això passi:

--- hints ---


--- hint ---

`Quan la bandera es cliqui`{:class="block3events"}, en un bucle `per sempre`{:class="block3control"}, comprova `si`{:class="block3control"} l'`habitació és 1`{:class="block3variables"} i en aquest cas `mostra`{:class="block3looks"} el personatge `senyal de benvinguda`, `si no`{:class="block3control"} `amaga`{:class="block3looks"} el personatge.

--- /hint ---

--- hint ---

Aquí tens els blocs que necessites:

![senyal](images/sign.png)

```blocks3
si < > llavors
si no
fi

< (habitació :: variables) = [1] >

amaga't

mostra't

per sempre
fi

quan la bandera es cliqui

```

--- /hint ---

--- hint ---

Aquí tens el codi complet:

![senyal](images/sign.png)

```blocks3
quan la bandera es cliqui
per sempre
    si < (habitació :: variables) = [1] > llavors,
        mostra't
    si no
        amaga't
    fi
fi
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Prova el codi del teu personatge `senyal de benvinguda` movent-te entre habitacions. El senyal només ha de ser visible a l'habitació 1.

![captura de pantalla](images/world-sign-test.png)

--- /task ---

--- task ---

Un senyal no és gaire bo si no diu res! Afegeix més codi per mostrar un missatge si el personatge de `senyal de benvinguda` toca el personatge `jugador`:

![senyal](images/sign.png)

```blocks3
quan la bandera es cliqui
per sempre
si < (habitació :: variables) = [1] > llavors,
mostra't
si no
amaga't
fi
+ si < tocant (jugador v)? > llavors
digues [Benvingut! Pots arribar al tresor?]
si no
digues []
fi
fi
```

--- /task ---

--- task ---

Prova el teu personatge `senyal de benvinguda` de nou. Ara hauries de veure un missatge quan el personatge del `jugador` toca el personatge `senyal de benvinguda`.

![captura de pantalla](images/world-sign-test2.png)

--- /task ---