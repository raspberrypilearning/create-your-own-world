## Sfida: espandi il tuo mondo

Ora puoi continuare a creare il tuo mondo! Ecco alcune idee:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Aggiungi suoni e musica al tuo gioco
+ Add more people, enemies, and signs
+ Aggiungi porte rosse e gialle e chiavi speciali per aprirle
+ Aggiungi più stanze al tuo mondo
+ Aggiungi altri oggetti utili al tuo gioco
    
    + Usa le monete per ottenere informazioni dalle altre persone:

![screenshot](images/world-bribe.png)

+ Potresti persino aggiungere porte nelle pareti nord e sud della stanza 1, in modo che il giocatore possa spostarsi tra le stanze in tutte e quattro le direzioni. For example, your game can have nine rooms in a 3×3 grid. Potresti quindi aggiungere `3` al numero delle stanze per scendere di un livello.

![screenshot](images/north-south-rooms.png) ![schermata](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```