## Presuňte prehrávač scény

Začnite tým, že vytvoríte `hráčov` sprite, ktorý sa môže pohybovať po celom svete.

\--- úloha \---

Otvorte projekt "Vytvorte si vlastný svet" Scratch starter.

**Online**: otvorte online štartovací projekt na adrese [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){: target = "_ blank"}. Ak máte účet Scratch, môžete kliknúť na **Remix** v pravom hornom rohu a uložiť kópiu projektu do svojho účtu.

**Offline**: stiahnite štartovací projekt [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){: target = "_ blank"} a potom ho otvorte pomocou editora offline. Ak potrebujete stiahnuť a nainštalovať editor Scratch offline, môžete ho nájsť na adrese [rpf.io/scratchoff](https://rpf.io/scratchoff){: target = "_ blank"}.

![snímka obrazovky](images/world-starter.png)

\--- / úloha \---

Stlačenie klávesov so šípkami by malo presunúť prehrávač `prehrávača`. Keď stlačíte šípku hore, hráč `hráča` by sa mal v reakcii pohybovať smerom hore.

\--- úloha \---

Pridajte tento kód k prehrávaču `prehrávača`:

![prehrávač](images/player.png)

```blocks3
keď sa vlajka preklikne
navždy
    ak <stlačíte tlačidlo (šípka nahor v)? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
koniec
```

\--- / úloha \---

\--- úloha \---

Kliknite na príznak a podržte šípku nahor. Hráč `hráča` ťahá hore?

![snímka obrazovky](images/world-up.png)

\--- / úloha \---

\--- úloha \---

Ak chcete presunúť prehrávač `prehrávača` doľava, musíte pridať ďalší blok `ak je`{: class = "block3control"} s podobným kódom:

![prehrávač](images/player.png)

```blocks3
keď sa vlajka preklikne
navždy
    ak <stlačíte tlačidlo (šípka nahor v)? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
+ ak je stlačené tlačidlo <(ľavá šípka v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec
koniec
```

\--- / úloha \---

\--- úloha \---

Pridajte ďalší kód do vášho prehrávača `` tak, aby sa mohol posunúť dole aj napravo. Použite kód, ktorý už máte, aby vám pomohol.

\--- rady \---

\--- hint \---

Ak chcete prejsť hore, ukážte prehrávač `prehrávača` v smere `0` stupne. Čo musíte urobiť, aby ste posunuli sprite?

Pohyb doľava, ukážete sprite v smere `-90` stupňov. Čo musíte urobiť, aby ste správne presunuli skript?

\--- /hint \---

\--- hint \---

Tieto dva bloky musíte zmeniť:

![prehrávač](images/player.png)

```blocks3
<key ( v) pressed>

bod v smere ()
```

Duplikovať kód, ktorý spôsobí, že sa prehrávač `prehrávača` presunie smerom hore a zmení tieto dva bloky tak, aby sa spriahol dole. Duplikujte kód znova a zmeňte ho tak, aby sa sprite presunul doprava.

\--- / hint \--- \--- tip \--- Tu je návod, ako by mal vyzerať váš kód:

![prehrávač](images/player.png)

```blocks3
keď sa vlajka preklikne
navždy
    ak <stlačíte tlačidlo (šípka nahor v)? > potom
        bod v smere (0)
        posunúť (4) kroky
    koniec
    ak je stlačené tlačidlo <(šípka doľava v)? > potom
        bod v smere (-90)
        posunúť (4) kroky
    koniec

+ ak je stlačené tlačidlo <(šípka dole v)? > potom
        bod v smere (180)
        posunúť (4) kroky
    koniec
+ ak <kláves [šípka vpravo v] stlačené? > potom
        bod v smere (90)
        posunúť (4) kroky
    koniec
koniec
```

\--- /hint \--- \--- /hints \---

\--- / úloha \---