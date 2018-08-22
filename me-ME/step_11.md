## Vrata i ključevi

Kako bi bilo da neka od vrata u tvom svijetu budu zaključana i da igrač mora da nađe ključ da bi nastavio dalje?

+ Pređi na lik `ključa`. Klikni desnim tasterom miša na njega i izaberi **show** (prikaži), tako da se ključ pojavi na pozornici.

+ Izmijeni kostim lika `ključa` da bude plave boje.

+ Postavi da pozadina Pozornice bude soba 3 i postavi lik `ključa` na neko mjesto do kojeg je teško doći!
    
    ![screenshot](images/world-key.png)

+ Dodaj kôd liku `ključa` tako da se pojavljuje samo u sobi 3.

+ Kreiraj novu listu (new list) i nazovi je `inventar`{:class="blockdata"}. U njoj ćeš čuvati sve stvari koje tvoj lik `igrača` sakupi.

[[[generic-scratch-make-list]]]

+ Kôd za sakupljanje ključa veoma je sličan kôdu za sakupljanje novčića. Razlika je u tome što ključ dodaješ u svoj inventar.

```blocks
    when flag clicked
    wait until <touching [player v]?>
    add [plavi ključ] to [inventar v]
    stop [other scripts in sprite v]
    hide
```

+ Isprobaj lik `ključa` da provjeriš da li možeš da ga pokupiš i dodaš u svoj inventar. Ne zaboravi da dodaš kôd Pozornici da se tvoj inventar isprazni na početku igre.

```blocks
    delete (all v) of [inventar v]
```

+ Sada dodajmo zaključana vrata. Klikni desnim tasterom miša na lik `vrata-plava` i izaberi **show** (prikaži), a zatim postavi lik na otvor između dva zida.

![screenshot](images/world-door.png)

+ Dodaj kôd liku `plavih vrata` tako da se pojavljuje samo u sobi 3.

+ Lik `plavih vrata` treba da se sakrije, kako bi dozvolio liku `igrača` da prođe kada imaš plavi ključ u svom inventaru.

```blocks
    when flag clicked
    wait until <[inventar v] contains [plavi ključ]>
    stop [other scripts in sprite v]
    hide
```

+ Isprobaj svoj projekat i provjeri da li možeš da pokupiš plavi ključ i otvoriš vrata!