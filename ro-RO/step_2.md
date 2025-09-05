## Mută personajul jucător

Începe prin a crea un `jucător` care se poate mișca în lumea creată de tine.

\--- task \---

Deschide proiectul Scratch de început „Crează-ți propria lume”.

**Online**: open the online starter project at [rpf.io/create-your-own-world-on](https://rpf.io/create-your-own-world-on){:target="_blank"}.

Dacă ai un cont Scratch poți face o copie dând click pe **Remix**.

**Offline**: download the starter project [rpf.io/p/en/create-your-own-world-go](https://rpf.io/p/en/create-your-own-world-go){:target="_blank"}, and then open it using the offline editor. Dacă ai nevoie să descarci și să instalezi editorul Scratch offline, îl poți găsi la [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![captură de ecran](images/world-starter.png)

\--- /task \---

Apăsarea tastelor săgeată ar trebui să mute `jucătorul`. Când săgeata în sus este apăsată, personajul `jucător` trebuie să se miște în sus pe scenă ca răspuns.

\--- task \---

Adaugă acest cod la personajul `jucător`:

![jucător](images/player.png)

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

Dă click pe steag și apoi ține apăsată săgeata sus. Personajul `jucător` se mișcă în sus?

![captură de ecran](images/world-up.png)

\--- /task \---

\--- task \---

Pentru a muta personajul `jucător` la stânga, trebuie să adaugi un alt bloc `dacă`{:class="block3control"} cu cod similar:

![jucător](images/player.png)

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

Adăugă mai mult cod personajului `jucător` pentru ca acesta să se poată mișca în jos și spre dreapta. Folosește codul pe care îl ai deja pentru a te ajuta.

\--- hints \---

\--- hint \---

Pentru a se deplasa în sus, indică personajul `jucător` în direcția `0` grade. Ce trebuie să faci pentru a muta personajul în jos?

Pentru a se deplasa spre stânga, indică personajul în direcția `-90` grade. Ce trebuie să faci pentru a mișca personajul spre dreapta?

\--- /hint \---

\--- hint \---

Trebuie să schimbi aceste două blocuri:

![jucător](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Copiază codul care face personajul `jucător` să se deplaseze în sus și schimbă aceste două blocuri pentru a-l face să se miște în jos. Copiază din nou codul și modifică-l pentru a face personajul să se deplaseze spre dreapta.

\--- /hint \---

\--- hint \---

Așa ar trebui să arate codul tău:

![jucător](images/player.png)

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
+    if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---