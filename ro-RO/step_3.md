## Pereți solizi

\--- task \--- Testează-ți din nou `personajul`. Vezi că poate trece prin pereții de culoare gri deschis.

![captură de ecran](images/world-walls.png) \--- /task \---

\--- task \--- Pentru a remedia acestă situație, va trebui să faci `personajul` să se dea în spate dacă atinge vreun perete gri deschis. Acesta este codul pe care trebuie să îl adăugi în căsuța `forever`{:class="block3control"}, sub căsuțele cu instrucțiuni:

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
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

\--- /task \---

\--- task \---

Încearcă să faci ca `personajul` să treacă printr-un perete. Dacă noul cod funcționează, acest lucru n-ar trebui să fie posibil.

![captură de ecran](images/world-walls-test.png) \--- /task \---