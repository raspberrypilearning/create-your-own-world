## Desafío: enemigos

Si quieres, también puedes añadir enemigos patrullando a tu juego. Si el objeto `jugador` toca un enemigo, el juego termina.

+ Tu juego ya contiene un objeto `enemigo`. Añade código al objeto `enemigo` de manera que solamente aparezca en la habitación 2.

+ Añade código para mover el objeto `enemigo` y para terminar el juego si el objeto `enemigo` toca al objeto `jugador`. Es más fácil hacer esto en bloques de código separados. El código de tu objeto `enemigo` debería quedar así:

```blocks3
al presionar la bandera verde
para siempre
si <(habitación :: variables) =[2]> luego
muestra
si no
ocultar

al presionar la bandera verde
para siempre
si <touching (jugador v)?> luego
detiene [todos v]

al presionar la bandera verde
ir a x : (170) y: (0)
para siempre
repetir (130)
cambiar x por (-1)
fin
repetir (130)
cambiar x por (1)
```

+ Prueba tu nuevo código para asegurarte de que funciona: 
    + El objeto `enemigo` sólo debe ser visible en la habitación 2
    + El objeto `enemigo` patrulla la habitación
    + La partida termina si el objeto `jugador` toca el objeto `enemigo`

¿Puedes crear otro objeto `enemigo` en la habitación 3 que patrulle arriba y abajo a través del hueco en la pared?

![captura de pantalla](images/world-enemy2.png)