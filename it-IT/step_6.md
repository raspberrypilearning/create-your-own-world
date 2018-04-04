## Raccogli monete

+ Aggiungi al tuo progetto una nuova variabile chiamata `monete`{:class="blockdata"}.

+ Fai clic col pulsante destro sullo sprite della 'moneta' e scegli 'mostra'.

![screenshot](images/world-coins.png)

+ Aggiungi un codice alla tua moneta, in modo che appaia solo nella stanza 1.

+ Aggiungi un codice allo sprite della tua moneta per aggiungere 1 alle tue `monete`{:class="blockdata"} quando vengono raccolte:

	```blocchi
		quando si clicca la bandiera
		aspetta finché <tocca [giocatore v]>?
		modifica [monete v] di (1)
		stop [altre scritte in sprite v]
		nascondi
	```

	Il codice `stop altre scritte in sprite`{:class="blockcontrol"} è necessario perché la moneta non venga più visualizzata nella stanza 1 una volta che viene raccolta.

+ Dovrai anche aggiungere un codice per impostare la variabile delle tue `monete`{:class="blockdata"} a 0 all'inizio del gioco.

+ Prova il tuo progetto - raccogliere le monete cambierà il tuo punteggio a 1.

## Sfida: Altre monete
Puoi aggiungere altre monete al gioco? Possono essere in stanze diverse, e alcune monete potrebbero essere custodite dai nemici in pattuglia.
