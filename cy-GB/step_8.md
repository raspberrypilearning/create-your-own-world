## Pobl

Fe awn ati i ychwanegu pobl arall i dy fyd mae modd i dy `chwaraewr` ryngweithio â nhw.

\--- task \--- Newida i'r corlun `person`.

![Corlun person](images/person.png) \--- /task \---

\--- task \--- Ychwanega gôd i dy `berson` fel fod y person yn siarad â'r `chwaraewr`. Mae'r côd yn derbyg iawn i'r un wnes di ei ychwanegu i'r `arwydd`:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
    end
end
```

\--- /task \---

\--- task \--- Rho ganiatâd i'r `person` i symud trwy ychwanegu dau floc yn adran `fel arall`{:class="block3control"} dy gôd:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
+       move (1) steps
+       if on edge, bounce
    end
end

```

\--- /task \---

Bydd dy `berson` nawr yn symud, ond yn stopio i siarad gyda'r `chwaraewr`.

![sgrinlun](images/world-person-test.png)

\--- task \--- Ychwanega gôd i dy `berson` newydd fel ei fod ond yn ymddangos yn ystafell 1. Fe ddylai'r côd fod union yr un peth â'r côd sydd yn gwneud i'r `arwydd` ymddangos yn ystafell 1.

Gwna'n siwr dy fod di'n profi dy gôd. \--- /task \---