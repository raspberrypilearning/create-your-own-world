## Challenge: sovražniki

Če želiš, lahko dodaš sovražnike, ki oprezajo po igri. Če se figura `igralec` dotakne sovražnika, je igre konec.

+ Tvoja igra že vsebuje figuro `sovražnik`. Figuri `sovražnik` dodaj kodo, da se bo pojavila le v drugi sobi.

+ Dodaj kodo, ki bo premikala figuro `sovražnik` in končala igro, če se figura `sovražnik` dotakne figure `igralec`. To je lažje narediti v ločenih blokih kode. Tako bi lahko tvoja koda figure `sovražnik` izgledala:

```blocks3
ko kliknemo na zastavo
ponavljaj
če <(soba :: Spremenljivka)=[2]> potem
pokaži
sicer
skrij

ko kliknemo na zastavo
ponavljaj
če <se dotika (igralec v)?> potem
ustavi (vse v)

ko kliknemo na zastavo
pojdi na x: (170) y:(0)
ponavljaj
ponovi (130) krat
spremeni x za (-1)
konec
ponovi (130) krat
spremeni x za (1)
konec
konec
```

+ Preizkusi svojo igro in se prepričaj, da: 
    + Je figura `sovražnik` vidna le v sobi 2
    + Figura `sovražnik` patruljira po sobi
    + Se igra konča, ko se figura `igralec` dotakne figure `sovražnik`

Ali lahko ustvariš še eno figuro `sovražnik` v sobi 3, ki se bo premikala goro in dol po zarezi v steni?

![posnetek zaslona](images/world-enemy2.png)