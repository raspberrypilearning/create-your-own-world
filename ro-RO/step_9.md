## Provocare: adaugă un inamic

Dacă vrei, poți, de asemenea, să adaugi la joc inamici care patrulează. Dacă personajul `jucător` atinge un inamic, jocul se termină.

+ Jocul tău conține deja un personaj `inamic`. Adaugă niște cod personajului `inamic` astfel încât să apară doar în camera 2.

+ Adaugă cod pentru a mișca personajul `inamic` și pentru a încheia jocul dacă personajul `inamic` atinge personajul `jucător`. Este mai ușor să faci acest lucru în blocuri de cod separate. Iată cum ar putea arăta codul pentru personajul tău `inamic`:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ Testează-ți noul cod pentru a te asigura că: 
    + Personajul `inamic` este vizibil doar în camera 2
    + Personajul `inamic` patrulează camera
    + Jocul se încheie dacă personajul`jucător` atinge personajul `inamic`

Poți crea un alt personaj `inamic` în camera 3, care patrulează în sus și în jos prin gaura din perete?

![captură de ecran](images/world-enemy2.png)