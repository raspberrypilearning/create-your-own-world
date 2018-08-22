## Cartelli

Aggiungiamo cartelli al tuo mondo per guidare il giocatore nel suo viaggio.

+ Il tuo progetto contiene uno sprite `cartello di benvenuto`:

![screenshot](images/world-sign.png)

+ Lo sprite `cartello di benvenuto` dovrebbe essere visibile solo nella stanza 1, quindi aggiungi del codice allo sprite `cartello di benvenuto` per assicurarti che ciò avvenga:

```blocks
    quando si clicca su ⚑
	per sempre 
	  se < (stanza) = [1] > allora 
		mostra
	  altrimenti 
		nascondi
	  fine
	fine
```

+ Metti alla prova il tuo sprite `cartello di benvenuto` muovendoti tra le stanze. Il tuo cartello dovrebbe essere visibile solo nella stanza 1.
    
    ![screenshot](images/world-sign-test.png)

+ Un cartello non è molto utile se non dice nulla! Aggiungi del codice per far visualizzare un messaggio se lo sprite `cartello di benvenuto` sta toccando lo sprite `giocatore`:

```blocks
    quando si clicca su ⚑
	per sempre 
	  se < (stanza) = [1] > allora 
		mostra
	  altrimenti 
		nascondi
	  fine
	  se < sta toccando [giocatore v] > allora 
		dire [Benvenuto! Riesci a trovare il tesoro?]
	  altrimenti 
		dire []
	  fine
	fine
```

+ Prova il tuo sprite `cartello di benvenuto`. Ora dovrebbe apparire un messaggio quando lo sprite `giocatore` lo tocca.

![screenshot](images/world-sign-test2.png)