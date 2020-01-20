## Mișcarea personajului

Începe prin a crea un `personaj` care se poate mișca în lumea creată de tine.

\--- task \---

Deschide proiectul Scratch de început „Crează-ți propria lume”.

**Online:** deschide proiectul de început la [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"}.

Dacă ai un cont Scratch poți face o copie dând click pe **Remix**.

**Offline:** descărcă proiectul de început de la [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_blank"}, apoi deschide-l folosind editorul offline. Dacă ai nevoie să descarci și să instalezi editorul Scratch offline, îl poți găsi la [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![captură de ecran](images/world-starter.png)

\--- /task \---

Apăsarea tastelor săgeată ar trebui să mute `personajul`. Când este apăsată săgeata sus, `personajul` ar trebui să se deplaseze în sus ca răspuns.

\--- task \---

Adaugă acest cod `personajului`:

![personaj](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

Dă click pe steag și apoi ține apăsată săgeata sus. `Personajul` se mișcă în sus?

![captură de ecran](images/world-up.png)

\--- /task \---

\--- task \---

Pentru a muta `personajul` la stânga, trebuie să adaugi o altă căsuță cu `variabilă`{:class="block3control"} cu cod similar:

![personaj](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

Adăugă mai mult cod `personajului` pentru ca acesta să se poată mișca în jos și spre dreapta. Folosește codul pe care îl ai deja pentru a vă ajuta.

\--- hints \---

\--- hint \---

Pentru a se deplasa în sus, indică `personajul` în direcția `0` grade. Ce trebuie să faci pentru a muta personajul în jos?

Pentru a se deplasa spre stânga, indică personajul în direcția `-90` grade. Ce trebuie să faci pentru a mișca personajul spre dreapta?

\--- /hint \---

\--- hint \---

Trebuie să schimbi aceste două căsuțe:

![personaj](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Copiază codul care face `personajul` să se deplasează în sus și schimbă aceste două căsuțe pentru a-l face să se miște în jos. Copiază din nou codul și modifică-l pentru a face personajul să se deplaseze spre dreapta.

\--- /hint \---

\--- hint \---

Here is how your code should look:

![player](images/player.png)

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

+    if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
+    if <key [right arrow v] pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---