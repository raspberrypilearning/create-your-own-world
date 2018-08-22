## Čvrsti zidovi

+ Isprobaj ponovo svoj lik `igrača`. Vjerovatno ćeš primijetiti da može da se kreće kroz svijetlosive zidove.

![screenshot](images/world-walls.png)

+ Da to popraviš, treba da vratiš lik `igrača` nazad kada dodirne svijetlosivi zid. Ovdje je kôd koji treba da dodaš unutar svog bloka `forever`{:class="blockcontrol"} (ponavljaj), ispod blokova za smjer:

```blocks
    if < touching color [#BABABA]? > then
        move (-4) steps
    end
```

+ Isprobaj ovaj novi kôd: pomjeri lik `igrača` ispod zida, a zatim provjeri da li možeš da ga pomjeriš nagore da prođe kroz zid. Ako tvoj kôd funkcioniše, ne bi trebalo da je moguće to uraditi.

![screenshot](images/world-walls-test.png)