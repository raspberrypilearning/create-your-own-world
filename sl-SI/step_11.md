## Vrata in ključi

Zdaj boš dodal-a kodo, ki bo poskrbela, da bodo nekatera vrata tvojega sveta zaklenjena, igralec pa mora najti ključ, da jih odpre, da bi lahko prišel v naslednjo sobo.

\--- task \--- Preklopi na figuro `ključ`. Klikni na oko zraven napisa `Pokaži` {:class="blocklooks"} v meniju figur, tako da se figura prikaže na odru. \--- /task \---

\--- task \--- Uredi figuro `ključ`, da bo modre barve. \--- /task \---

\--- task \--- Zamenjaj ozadje na sobo 3, in postavi figuro `ključ` nekam, kjer jo je težko doseči!

![posnetek zaslona](images/world-key.png)

\--- /task \---

\--- task \--- Figuri `ključ` dodaj kodo, da bo vidna le v sobi 3. \--- /task \---

\--- task \--- Ustvari nov seznam imenovan `imetje`{:class="block3variables"}, v katerega se bodo shranili predmeti, ki jih figura `igralec` pobere.

[[[generic-scratch3-make-list]]] \--- /task \---

\--- task \--- Za to potrebna koda je zelo podobna kodi, ki skrbi za pobiranje kovancev. Razlika je v tem, da ključe dodajaš v `imetje`{:class="block3variables"}.

![ključ](images/key.png)

```blocks3
ko kliknemo na zastavo
počakaj dokler ni < se dotika (igralec v)?>
dodaj [modri ključ] k [imetje v]
skrij
ustavi [ostale ukaze za to figuro v]
```

\--- /task \---

\--- task \--- Odru dodaj kodo, ki bo izpraznila imetje na začetku igre.

```blocks3
zbriši (all v) [imetje v]
```

\--- /task \---

\--- task \--- Preizkusi svoj program, da preveriš ali lahko pobereš figuro `ključ` in jo dodaš v svoje imetje. \--- /task \---

\--- task \--- Zdaj dodaj zaklenjena vrata. Izberi figuro `vrata-modra` in klikni na oko zraven napisa`Pokaži`{:class="blocklooks} v menuju figure, potem pa postavi figuro v prehod med dvema stenama.

![posnetek zaslona](images/world-door.png) \--- /task \---

\--- task \--- Dodaj kodo v figuro `vrata-modra`, tako da bo vidna le v tretji sobi. \--- /task \---

\--- task \--- Dodaj kodo v `vrata-modra`, da sebo, ko se ključ nahaja v `imetju`{:class="block3variables"}, figura `skrila`{:class="block3looks"} in oogočila figuri `igralec` prehod.

![vrata](images/door.png)

```blocks3
ko kliknemo na zastavo
počakaj dokler ni < Ali [imetje v] vsebuje (modri ključ)?
ustavi [ostale ukaze za to figuro v]
skrij
```

\--- /task \---

\--- task \--- Preizkusi svojo igro, da vidiš, ali lahko pobereš modri ključ in odpreš vrata! \--- /task \---