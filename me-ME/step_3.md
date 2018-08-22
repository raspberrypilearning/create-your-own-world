## Pomjeranje lika `igrača`

Počnimo tako što ćemo kreirati lik `igrača` koji može da se kreće po tvom svijetu.

+ Ako koristiš Scratch online, otvori Scratch projekat 'Create your own world' na <http://jumpto.cc/world-go>{:target="_blank"}. Ako koristiš Scratch offline, preuzmi projekat [ovdje](http://jumpto.cc/world-get){:target="_blank"} i otvori ga koristeći offline editor. 

![screenshot](images/world-starter.png)

Osoba koja igra igru koristiće tastere sa strelicama za pomjeranje lika `igrača`. Kada osoba pritisne strelicu nagore, treba da kažeš liku `igrača` da odgovori kretanjem prema gore, kako bi se kretao u ispravnom smjeru.

+ Dodaj ovaj kôd liku `igrača`:

```blocks
    when flag clicked
    forever
        if <key [up arrow v] pressed? > then
            point in direction (0)
            move (4) steps
        end
    end
```

+ Isprobaj lik `igrača` tako što ćeš kliknuti na zastavicu, a zatim držati pritisnutu strelicu nagore. Da li se lik `igrača` kreće nagore?
    
    ![screenshot](images/world-up.png)

+ Za pomjeranje lika `igrača` ulijevo, treba da mu dodaš još jedan blok `if`{:class="blockcontrol"} (ako) sa sličnim kôdom:

```blocks
    when flag clicked
    forever
        if <key [up arrow v] pressed? > then
            point in direction (0)
            move (4) steps
        end
        if <key [left arrow v] pressed? > then
            point in direction (-90)
            move (4) steps
        end
    end
```

+ Dodaj još kôda svom liku `igrača`, tako da može da se kreće nadolje i udesno. Kao pomoć, koristi kôd koji već imaš.

\--- hints \--- \--- hint \--- Da bismo lik `igrača` pomjerali nagore, okrenuli smo ga u smjeru `0` stepeni. Šta bi trebalo da uradiš za pomjeranje lika nadolje?

Da bismo lik igrača pomjerali ulijevo, okrenuli smo ga u smjeru `-90` stepeni. Šta bi trebalo da uradiš za pomjeranje lika udesno? \--- /hint \--- \--- hint \--- Treba da izmijeniš ova dva bloka:

```blocks
<key [ v] pressed>
```

```blocks
point in direction ()
```

Umnoži (duplicate) kôd koji si koristio/koristila za kretanje nagore, ali izmijeni ova dva bloka da napraviš da se lik `igrača` kreće nadolje. Uradi isto za kretanje udesno. \--- /hint \--- \--- hint \--- Ovako treba da izgleda tvoj kôd:

![Kretanje nadolje i udesno](images/finished-move-down-right.png) \--- /hint \--- \--- /hints \---