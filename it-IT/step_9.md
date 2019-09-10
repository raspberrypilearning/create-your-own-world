## Sfida: aggiungi un nemico

Se vuoi, puoi anche aggiungere dei nemici pattugliatori al tuo gioco. Se lo sprite `player` tocca un nemico, il gioco termina.

+ Il tuo gioco contiene già uno sprite `nemico`. Aggiungi del codice allo sprite `nemico` per far sì che appaia solo nella stanza 2.

+ Aggiungi del codice per far muovere lo sprite `nemico` e per far terminare il gioco se lo sprite `nemico` tocca lo sprite `giocatore`. È più facile farlo in blocchi di codice separati. Ecco come il codice del tuo sprite `nemico` potrebbe apparire:

```blocks3
quando si clicca sulla bandiera verde
per sempre 
 se <(stanza :: variables) = [2]> allora 
 mostra
 altrimenti 
 nascondi
 end
end

quando si clicca sulla bandiera verde
per sempre 
 se <touching (player v)?> allora 
 ferma [all v]
 end
end

quando si clicca sulla bandiera verde
vai a x: (170) y: (0)
per sempre 
 ripeti (130) volte 
 cambia x di (-1)
 end
 ripeti (130) volte 
 cambia x di (1)
 end
end
```

+ Prova il tuo nuovo codice per assicurarti che: 
    + Lo sprite `nemico` sia visibile solo nella stanza 2
    + Il `nemico` pattugli la stanza
    + Il gioco finisca se lo sprite `giocatore` tocca lo sprite `nemico`

Sapresti creare un altro sprite `nemico` nella stanza 3 che pattugli su e giù attraverso lo spazio nel muro?

![screenshot](images/world-enemy2.png)