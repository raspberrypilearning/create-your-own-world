## Dvere a kľúče

Now you are going to add code so that some of the doors in your game world are locked, and the player must find the key to open them and get to the next room.

\--- task \--- Prepnúť na `kľúč` sprite. Kliknite na `zobraziť`{: class = "blocklooks"} v ponuke Skripty tak, aby sa na scéne zobrazil skript. \--- / úloha \---

\--- úloha \--- Upravte kostým `kruhu` , aby bol modrý. \--- / úloha \---

\--- úloha \--- Prepnite si pozadie Scény do miestnosti 3 a umiestnite `kľúč` sprite niekde ťažko dosiahnuteľné!

![snímka obrazovky](images/world-key.png)

\--- / úloha \---

\--- úloha \--- Pridajte kód na `kľúč` sprite, aby bol viditeľný iba v miestnosti 3. \--- / úloha \---

\--- task \--- Vytvorte nový zoznam s názvom `inventár`{: class = "block3variables"} pre uloženie položiek, ktoré váš `hráč` sprite.

[[[generic-scratch3-make-list]]] \--- / úloha \---

\--- task \--- Kód, ktorý potrebujete pridať na zber kľúča, je veľmi podobný kódu pre zbieranie mincí. Rozdiel je v tom, že ste pridať kľúč do `inventári`{: class = "block3variables"}.

![kláves](images/key.png)

```blocks3
keď vlajka klikne
čakajte, až <touching (player v)?>
pridajte [blue key] do [inventory v]
skryť
stop [iné skripty v sprite v]
```

\--- / úloha \---

\--- task \--- Pridajte kód na svoju plochu, aby ste vyprázdnili inventár na začiatku hry.

```blocks3
odstrániť (všetky v) položky [inventár v]
```

\--- / úloha \---

\--- task \--- Vyskúšajte svoju hru, aby ste skontrolovali, či môžete zbierať `kľúč` sprite a pridať ho do vášho inventára. \--- / úloha \---

\--- úloha \--- Teraz pridajte zamknuté dvere. Zvoľte `dverí-modrý` sprite a kliknite na `zobraziť`{: class = "blocklooks} v ponuke Scripts a potom umiestnite sprite cez medzeru medzi dvoma stenami.

![snímka obrazovky](images/world-door.png) \--- / úloha \---

\--- úloha \--- Pridajte kód do `dverí-modrej` sprite tak, aby bol viditeľný len v miestnosti 3. \--- / úloha \---

\--- úloha \--- Pridajte kód do `dverí-modrá` sprite tak, že keď je kľúč v `inventári`{: class = "block3variables"}, sprite `skryje`{: class = "block3looks "}, aby váš `hráčov` sprite prešiel.

![dvere](images/door.png)

```blocks3
keď má príznak
počkajte, kým <[inventár v] neobsahuje [modrý kľúč]?>
stop [iné skripty v sprite v]
skryť
```

\--- / úloha \---

\--- task \--- Vyskúšajte hru a uvidíte, či môžete vyzdvihnúť modrý kľúč na otvorenie dverí! \--- / úloha \---