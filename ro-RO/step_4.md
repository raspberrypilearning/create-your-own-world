## Mișcă-te în jurul lumii tale

`Personajul` ar trebui să poată să treacă prin uși în alte camere.

Proiectul tău conține fundaluri pentru noi camere:

![captură de ecran](images/world-backdrops.png)

\--- task \---

Crează o nouă variabilă „pentru toate personajele” numită `room`{:class="block3variables"} pentru a monitoriza în care dintre camere se află `personajul`.

[[[generic-scratch3-add-variable]]]

![captură de ecran](images/world-room.png) \--- /task \---

\--- task \--- Când `personajul` atinge ușa portocalie în prima cameră, jocul ar trebui să afișeze următorul fundal și `personajul` ar trebui să se deplaseze înapoi în partea stângă a ferestrei. Adaugă acest cod în bucla `forever`{:class="block3control"} a `personajului`:

![personaj](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
+   if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
    end
end
```

\--- /task \---

\--- task \--- De fiecare dată când va începe jocul, camera, poziția personajului și fundalul trebuie resetate.

Adaugă codul la **începutul** codului `personajului` care se află deasupra buclei `forever`{:class="block3control"}, pentru a reseta totul atunci când se dă click pe steag:

\--- hints \--- \--- hint \--- Când începe jocul:

+ Valoarea `room`{:class="block3variables"} ar trebui setată ca `1`{:class="block3variables"}
+ Fundalul `backdrop`{:class="block3looks"} ar trebui setat ca `room1`{:class="block3looks"}
+ Poziția `personajului` er trebui setată ca `x: -200 y: 0`{:class="block3motion"} \--- /hint \--- \--- hint \--- Aici sunt căsuțele suplimentare de care ai nevoie:

![personaj](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

\--- /hint \--- \--- hint \--- Uite cum ar trebui să arate codul:

![personaj](images/player.png)

```blocks3
when flag clicked
+set [room v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to (room1 v)
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
    if < touching color [#BABABA]? > then
    move (-4) steps
    end
    if < touching color [#F2A24A] > then
    switch backdrop to (next backdrop v)
    go to x: (-200) y: (0)
    change [room v] by (1)
end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Dă click pe steag și apoi mișcă `personajul` până când atinge ușa portocalie. Personajul s-a mutat în următoarea cameră? Valoarea variabilei `room`{:class="block3variables"} s-a modificat în `2`?

![captură de ecran](images/world-room-test.png) \--- /task \---