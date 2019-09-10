## Symud o gwmpas dy fyd

Fe ddylai'r `chwaraewr` allu gerdded trwy ddrysau i ystafelloedd eraill.

Mae dy brosiect yn cynnwys cefndir ar gyfer ystafelloedd ychwanegol:

![sgrinlun](images/world-backdrops.png)

--- task ---

Byddi di angen newidyn newydd ‘ar gyfer pob ciplun’ o’r enw `ystafell`{:class="block3variables"} i wybod pa ystafell mae’r `chwaraewr` ynddo.

[[[generic-scratch3-add-variable]]]

![sgrinlun](images/world-room.png) --- /task ---

--- task --- Pan mae’r `chwaraewr` yn cyffwrdd y drws oren yn yr ystafell gyntaf, fe ddylai’r cefndir nesaf ymddangos ac fe ddylai’r `chwaraewr` symud yn ôl i ochr chwith y llwyfan. Dyma’r côd fydd ei angen arno ti - fe ddylai gael ei osod tu fewn dolen `am byth`{:class="block3control"} y `chwaraewr`:

![chwaraewr](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
    os <bysell (saeth i fyny v) wedi ei phwyso? > yna 
      pwyntio i gyfeiriad (0)
      symud (4) cam
    end
    os <bysell (saeth chwith v) wedi ei phwyso? > yna 
      pwyntio i gyfeiriad (-90)
      symud (4) cam
    end
      os <bysell (saeth i lawr v) wedi ei phwyso? > yna 
      pwyntio i gyfeiriad (-180)
      symud (4) cam
    end
      os <bysell [saeth de v] wedi ei phwyso? > yna 
      pwyntio i gyfeiriad (90)
      symud (4) cam
    end
    os <cyffwrdd lliw [#BABABA] ? > yna 
    symud (-4) cam
    end
+   os <cyffwrdd lliw [#F2A24A] ?> yna 
    newid cefndir i (cefnlen nesaf v)
    mynd i x: (-200) y: (0)
    newid [ystafell v] gan (1)
    end
end
```

--- /task ---

--- task --- Bob tro mae'r gêm yn cychwyn, bydd angen ailosod yr ystafell, lleoliad y cymeriad a'r cefndir.

Ychwaneda'r côd i **ddechrau** côd dy `chwaraewr` uwchben y ddolen `am byth`{:class="block3control"} i ailosod popeth pan mae'r faner yn cael ei glicio:

--- hints ---
 --- hint --- Pan mae'r gêm yn cychwyn:

+ Fe ddylai gwerth `ystafell`{:class="block3variables"} gael ei osod i `1`{:class="block3variables"}
+ Fe ddylai y `cefndir`{:class="block3looks"} gael ei osod i `room1`{:class="block3looks"}
+ Fe ddylai lleoliad y `chwaraewr` gael ei osod i `x: -200 y: 0`{:class="block3motion"}
--- /hint ---
 --- hint --- Dyma'r blociau ychwanegol sydd eu hangen:

![chwaraewr](images/player.png)

```blocks3
mynd i x: (-200) y: (0)

gosod [ystafell v] i (1)

newid cefndir i (room1 v)
```

--- /hint --- --- hint --- Dyma sut ddylai dy gôd edrych:

![chwaraewr](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
+gosod [ystafell v] i (1)
+mynd i x: (-200) y: (0)
+newid cefndir i (room1 v)
am byth 
  os <bysell (saeth i fyny v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (0)
    symud (4) cam
  end
  os <bysell (saeth chwith v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (-90)
    symud (4) cam
  end
  os <bysell (saeth i lawr v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (-180)
    symud (4) cam
  end
  os <bysell [saeth de v] wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (90)
    symud (4) cam
  end
  os <cyffwrdd lliw [#BABABA] ? > yna 
    symud (-4) cam
  end
  os <cyffwrdd lliw [#F2A24A] ?> yna 
    newid cefndir i (cefnlen nesaf v)
    mynd i x: (-200) y: (0)
    newid [ystafell v] gan (1)
  end
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task --- Clicia'r faner ac yna symud y `chwaraewr` tan ei fod yn cyffwrdd y drws oren. Ydy'r corlun yn symud i'r sgrin nesaf? Ydy'r `ystafell`{:class="block3variables"} yn newid i `2`?

![sgrinlun](images/world-room-test.png) --- /task ---