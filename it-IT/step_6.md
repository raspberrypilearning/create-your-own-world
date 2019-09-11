## Cartelli

Aggiungiamo cartelli al tuo mondo per guidare il giocatore nel suo viaggio.

Il tuo progetto contiene uno sprite `cartello di benvenuto`:

![screenshot](images/world-sign.png)

\--- task \--- Il 0>cartello di benvenuto</code> dovrebbe vedersi solo nella stanza 1, quindi aggiungi del codice allo sprite per fare in modo che succeda ciò:

\--- hints \--- \--- hint \--- `Quando si clicca sulla bandiera verde`{:class="block3events"}, controlla `per sempre`{:class="block3control"} `se`{:class="block3control"} la `stanza è 1`{:class="block3sensing"}, ed in quel caso mostra `cartello di benvenuto`{:class="block3control"}, `altrimenti`{:class="block3control"} `nascondi`{:class="block3looks"} lo sprite. \--- /hint \--- \--- hint \--- Qui ci sono i blocchi di codice che ti serviranno:

![cartello](images/sign.png)

```blocks3
<br />se &lt;&gt; allora 
altrimenti
end

&lt;(stanza :: variables) = [1]&gt;

nascondi

mostra

per sempre
end

quando si clicca sulla bandiera verde

```

\--- /hint \--- \--- hint \--- Ecco il codice completo:

![cartello](images/sign.png)

```blocks3
quando si clicca sulla bandiera verde
per sempre 
  se <(stanza :: variables) = [1]> allora 
    mostra
  altrimenti 
    nascondi
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Metti alla prova il tuo sprite `cartello di benvenuto` muovendoti tra le stanze. Il tuo cartello dovrebbe essere visibile solo nella stanza 1.

![schermata](images/world-sign-test.png) \--- /task \---

\--- task \--- Un cartello non è molto utile se non dice nulla! Aggiungi del codice per far visualizzare un messaggio se lo sprite `cartello di benvenuto` sta toccando lo sprite `giocatore`:

![cartello](images/sign.png)

```blocks3
when flag clicked
forever
if < (stanza :: variables) = [1] > then
show
else
hide
end
+if < touching (giocatore v)? > then
say [Benvenuto! Riesci a raccogliere il tesoro?]
else
say []
end
end
```

\--- /task \---

\--- task \--- Prova di nuovo il tuo sprite `cartello di benvenuto`. Ora dovresti vedere un messaggio quando lo sprite ` player ` tocca il ` cartello di benvenuto`.

![schermata](images/world-sign-test2.png) \--- /task \---