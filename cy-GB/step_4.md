## Symud o gwmpas dy fyd

Fe ddylai'r `chwaraewr` allu gerdded trwy ddrysau i ystafelloedd eraill.

Mae dy brosiect yn cynnwys cefndir ar gyfer ystafelloedd ychwanegol:

![sgrinlun](images/world-backdrops.png)

\--- task \---

Byddi di angen newidyn newydd ‘ar gyfer pob ciplun’ o’r enw `ystafell`{:class="block3variables"} i wybod pa ystafell mae’r `chwaraewr` ynddo.

[[[generic-scratch3-add-variable]]]

![sgrinlun](images/world-room.png) \--- /task \---

\--- task \--- Pan mae’r `chwaraewr` yn cyffwrdd y drws oren yn yr ystafell gyntaf, fe ddylai’r cefndir nesaf ymddangos ac fe ddylai’r `chwaraewr` symud yn ôl i ochr chwith y llwyfan. Dyma’r côd fydd ei angen arno ti - fe ddylai gael ei osod tu fewn dolen `am byth`{:class="block3control"} y `chwaraewr`:

![chwaraewr](images/player.png)

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

\--- task \--- Bob tro mae'r gêm yn cychwyn, bydd angen ailosod yr ystafell, lleoliad y cymeriad a'r cefndir.

Ychwaneda'r côd i **ddechrau** côd dy `chwaraewr` uwchben y ddolen `am byth`{:class="block3control"} i ailosod popeth pan mae'r faner yn cael ei glicio:

\--- hints \--- \--- hint \--- Pan mae'r gêm yn cychwyn:

+ Fe ddylai gwerth `ystafell`{:class="block3variables"} gael ei osod i `1`{:class="block3variables"}
+ Fe ddylai y `cefndir`{:class="block3looks"} gael ei osod i `room1`{:class="block3looks"}
+ Fe ddylai lleoliad y `chwaraewr` gael ei osod i `x: -200 y: 0`{:class="block3motion"} \--- /hint \--- \--- hint \--- Dyma'r blociau ychwanegol sydd eu hangen:

![chwaraewr](images/player.png)

```blocks3
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to (room1 v)
```

\--- /hint \--- \--- hint \--- Dyma sut ddylai dy gôd edrych:

![chwaraewr](images/player.png)

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

\--- task \--- Clicia'r faner ac yna symud y `chwaraewr` tan ei fod yn cyffwrdd y drws oren. Ydy'r corlun yn symud i'r sgrin nesaf? Ydy'r `ystafell`{:class="block3variables"} yn newid i `2`?

![sgrinlun](images/world-room-test.png) \--- /task \---