## Casglu darnau arian

Fe ddylai dy `chwaraewr` allu casglu darnau arian wrth iddo symud trwy'r byd.

\--- task \--- Ychwanega newidyn newydd o’r enw `arian`{:class="block3variables"} i dy brosiect. \--- /task \---

\--- task \--- Dewisa'r `arian` a chlicio **dangos**.

![sgrinlun](images/coin.png) \--- /task \---

\--- task \--- Ychwanega gôd i dy `arian` fel ei fod ond yn ymddangos yn ystafell 1. ![sgrinlun](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

Ychwanega gôd i dy `arian` fel fod y corlun yn `cuddio`{:class="block3looks"} a bod `1`{:class="block3variables"} yn cael ei ychwanegu i'r newidyn `arian`{:class="block3variables"} unwaith mae'r `chwaraewr` yn cyffwrdd y darn `arian` i'w 'bigo fyny'.

![darn arian](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

Mae angen y côd `stopiwch sgriptiau eraill yn y ciplun`{:class="block3control"} fel bod y darn `arian` yn stopio ymddangos yn ystafell 1 unwaith mae’n cael ei gasglu.

\--- /task \---

Ychwanega gôd i dy Lwyfan i osod y newidyn `arian`{:class="block3variables"} i `0`{:class="block3variables"} ar ddechrau dy gêm.

![llwyfan](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \--- Profa dy gêm. Dylai casglu darn arian newid sgôr dy `arian` i `1`{:class="block3variables"}. \--- /task \---