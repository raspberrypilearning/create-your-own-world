## Her: ychwanegu gelyn

Os hoffet ti, mae modd ychwanegu gelynion i dy gêm. Pan mae'r `chwaraewr` yn cyffwrdd gelyn, daw'r gêm i ben.

+ Mae dy gêm yn cynnwys `gelyn` yn barod. Ychwanega gôd i'r `gelyn` fel ei fod ond yn ymddangos yn ystafell 2.

+ Ychwanega gôd i symud y `gelyn` i ddiwedd y gêm os yw'r `gelyn` yn cyffwrdd y `chwaraewr`. Mae'n haws gwneud hyn mewn blociau côd ar wahân. Dyma sut bydd côd y `gelyn` yn edrych o bosib:

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

+ Profa dy gôd i sicrhau fod: 
    + Y `gelyn` ond yn ymddangos yn ystafell 2
    + Bod y `gelyn` yn symud o gwmpas yr ystafell
    + Bod y gêm yn dod i ben pan mae'r `chwaraewr` yn cyffwrdd y `gelyn`

Wyt ti'n gallu creu `gelyn` yn ystafell 3 sy'n symud lan a lawr trwy'r gap yn y wal?

![sgrinlun](images/world-enemy2.png)