## Symud dy chwareuwr

Fe awn ati i greu `chwareuwr` sydd yn symud o gwmpas dy fydysawd.

--- task ---

Agora'r prosiect cychwynnol 'Creu dy fyd dy hunan'.

**Arlein:** agora brosiect Scratch newydd yma [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"}.

Os oes ganddot ti gyfrif Scratch galli di wneud copi drwy glicio ar **Remix**.

**All-lein:** lawrlwytha'r prosiect cychwynnol o [rpf.io/p/cy-GB/create-your-own-world-go](http://rpf.io/p/cy-GB/create-your-own-world-go){:target="_blank"} ac yna ei agor gan ddefnyddio'r golygydd all-lein. Os oes angen i ti lawrlwytho a gosod golygydd Scratch all-lein, mae modd dod o hyd iddo yma [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![sgrinlun](images/world-starter.png)

--- /task ---

Dylai gwasgu'r bysellau saeth symud y `chwaraewr` o gwmpas. Pan fydd y saeth i fyny yn cael ei gwasgu, fe ddylai y `chwaraewr` symud i fyny ar y Llwyfan mewn ymateb.

--- task ---

Ychwanega’r côd canlynol i’r corlun `chwareuwr`:

![chwaraewr](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
  os <bysell (saeth i fyny v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (0)
    symud (4) cam
  end
end
```

--- /task ---

--- task ---

Clicia'r faner a dal y saeth i fyny. Ydy'r `chwareuwr` yn symud fyny?

![sgrinlun](images/world-up.png)

--- /task ---

--- task ---

I symud y `chwareuwr` i'r chwith, bydd angen i ti ychwanegu bloc arall `os`{:class="block3control"} gyda chôd tebyg:

![chwaraewr](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
  os <bysell (saeth i fyny v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (0)
    symud (4) cam
  end
+ os <bysell (saeth chwith v) wedi ei phwyso? > yna 
     pwyntio i gyfeiriad (-90)
     symud (4) cam
   end
end
```

--- /task ---

--- task ---

Ychwanega mwy o gôd i'r `chwareuwr` fel ei fod yn symud lawr ac i'r dde hefyd. Defnyddia'r côd sydd gen ti yn barod i dy helpu.

--- hints ---


--- hint ---

I symud fyny, pwyntia'r `chwareuwr` yng nghyfeiriad `0` gradd. Beth sydd angen i ti wneud i symud y corlun lawr?

I symud i'r chwith, pwyntia'r corlun yng nghyfeiriad `90` gradd. Beth sydd angen i ti ei wneud i symud y corlun i'r dde?

--- /hint ---

--- hint ---

Mae angen i ti newid y ddau floc yma:

![chwaraewr](images/player.png)

```blocks3
<bysell ( v) wedi ei phwyso?>

pwyntio i gyfeiriad ()
```

Dyblyga'r côd sy'n gwneud i'r `chwareuwr` symud fyny, ac yna newidia'r ddau floc i wneud i'r corlun symud lawr. Dyblyga'r côd eto a'i newid fel fod y corlun yn symud i'r dde.

--- /hint --- --- hint --- Dyma sut ddylai dy gôd edrych:

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

+  os <bysell (saeth i lawr v) wedi ei phwyso? > yna 
     pwyntio i gyfeiriad (180)
     symud (4) cam
   end
   os <bysell [saeth de v] wedi ei phwyso? > yna 
     pwyntio i gyfeiriad (90)
     symud (4) cam
   end
end
```

--- /hint ------ /hints ---

--- /task ---
