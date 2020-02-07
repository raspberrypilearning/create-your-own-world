## Desafío: Amplía tu mundo

¡Ahora puedes seguir creando tu propio mundo! Aquí tienes algunas sugerencias:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Añade sonido y música a tu juego
+ Add more people, enemies, and signs
+ Añade puertas rojas y amarillas, y llaves especiales para abrirlas
+ Añade más habitaciones a tu mundo
+ Añade otros objetos útiles a tu juego
    
    + Usa monedas para obtener información de otras personas:

![captura de pantalla](images/world-bribe.png)

+ Incluso podrías añadir puertas en las paredes norte y sur de la habitación 1, de modo que el jugador pueda moverse entre habitaciones en las cuatro direcciones. For example, your game can have nine rooms in a 3×3 grid. Entonces podrías sumar `3` al número de habitación para moverte al nivel inferior.

![captura de pantalla](images/north-south-rooms.png)

![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```