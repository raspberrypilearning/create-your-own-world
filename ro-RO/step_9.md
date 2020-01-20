## Provocare: adaugă un inamic

Dacă vrei, poți, de asemenea, să adaugi inamici care patrulează. Dacă `personajul` atinge un inamic, jocul se termină.

+ Jocul tău conține deja un `inamic`. Adăugă niște cod `inamicului` astfel încât să apară doar în camera 2.

+ Adăugă cod pentru a mișca `inamicul` și pentru a încheia jocul dacă `inamicul` atinge `personajul`. Este mai ușor să faci acest lucru în mai multe căsuțe. Iată cum ar putea arăta codul pentru `inamicul` tău:

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

+ Testează-ți noul cod pentru a te asigura că funcționează: 
    + `Inamicul` este vizibil doar în camera 2
    + `Inamicul` patrulează camera
    + Jocul se încheie dacă `personajul` atinge `inamicul`

Poți crea un alt `inamic` în camera 3 care patrulează în sus și în jos prin gaura din perete?

![captură de ecran](images/world-enemy2.png)