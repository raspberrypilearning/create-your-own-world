## Codifica il tuo giocatore

Iniziamo a creare un giocatore che possa muoversi attorno al mondo.

+ Apri il progetto Scratch online 'Crea il Tuo Mondo' a <a href="http://jumpto.cc/world-go" target="_blank">jumpto.cc/world-go</a> o scaricalo da <a href="http://jumpto.cc/world-get" target="_blank">jumpto.cc/world-get</a> e poi apri se stai usando l'editore offline.

	![screenshot](images/world-starter.png)

+ Usiamo i tasti freccia per muovere il giocatore. Quando il giocatore preme la freccia in su, vogliamo che il giocatore si sposti verso l'alto, cambiando la sua coordinata y. Aggiungi questo codice allo sprite 'giocatore':

	```blocks
		quando si clicca la bandiera
		per sempre
			se < il tasto [freccia in su v] premuto? > allora
				cambia y di (2)
			fine
		fine
	```

+ Prova il tuo giocatore cliccando la bandiera e poi tenendo premuta la freccia in su. Il tuo giocatore si muove verso l'alto?

	![screenshot](images/world-up.png)

+ Per muovere il giocatore a sinistra, dovrai aggiungere un altro blocco `se`{:class="blockcontrol"} al tuo giocatore, che cambierà la coordinata x:

	```blocks
		quando si clicca la bandiera
		per sempre
			se < il tasto [freccia in su v] premuto? > allora
				cambia y di (2)
			fine
			se < il tasto [freccia a sinistra v] premuto? > allora
				cambia x di (-2)
			fine
		fine
	```

## Sfida: Muoversi nelle quattro direzioni 
Puoi aggiungere un altro codice al tuo giocatore, in modo che possa muoversi su, giù, a destra e a sinistra? Come aiuto, usa il codice che hai già!

+ Prova di nuovo il tuo giocatore, e vedrai che riuscirà a camminare attraverso i muri di colore grigio chiaro.

	![screenshot](images/world-walls.png)

+ Per risolverlo, dovrai muovere il giocatore, ma poi riportarlo indietro se tocca un muro grigio chiaro. Ecco il codice che ti servirà:

	```blocks
		quando si clicca la bandiera
		per sempre
			se < il tasto [freccia in su v] premuto? > allora
				cambia y di (2)
				se < tocca colore [#BABABA]? > allora
					cambia y di (-2)
				fine
			fine
		fine
	```

	Nota che il nuovo blocco `se`{:class="blockcontrol"}`tocca colore`{:class="blocksensing"} è _dentro_ il blocco `se`{:class="blockcontrol"}`tasto [freccia in su]`{:class="blocksensing"}.

+ Prova questo nuovo codice muovendoti sotto il muro - non sarai in grado di spostarti in alto nel muro.

	![screenshot](images/world-walls-test.png)

+ Facciamo la stessa cosa per la freccia sinistra, riportandoci indietro se il giocatore tocca il muro. Il codice del tuo giocatore dovrebbe essere così:

	![screenshot](images/world-wall-code.png)

## Sfida: Aggiustare il movimento del tuo giocatore 
Aggiungi un codice al tuo giocatore in modo che tu non possa camminare attraverso i muri in qualsiasi direzione. Come aiuto, usa il codice che hai già!
