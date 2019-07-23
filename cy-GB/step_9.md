## Her: ychwanegu gelyn

Os hoffet ti, mae modd ychwanegu gelynion i dy gêm. Pan mae'r `chwaraewr` yn cyffwrdd gelyn, daw'r gêm i ben.

+ Mae dy gêm yn cynnwys `gelyn` yn barod. Ychwanega gôd i'r `gelyn` fel ei fod ond yn ymddangos yn ystafell 2.

+ Ychwanega gôd i symud y `gelyn` i ddiwedd y gêm os yw'r `gelyn` yn cyffwrdd y `chwaraewr`. Mae'n haws gwneud hyn mewn blociau côd ar wahân. Dyma sut bydd côd y `gelyn` yn edrych o bosib:

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
  os <(ystafell :: variables) = [2]> yna 
    dangos
  fel arall 
    cuddio
  end
end

pan fo'r flag werdd yn cael ei glicio
am byth 
  os <cyffwrdd (player v) ?> yna 
    aros [all v]
  end
end

pan fo'r flag werdd yn cael ei glicio
mynd i x: (170) y: (0)
am byth 
  ailadrodd (130) 
    newid x gan (-1)
  end
  ailadrodd (130) 
    newid x gan (1)
  end
end
```

+ Profa dy gôd i sicrhau fod: 
    + Y `gelyn` ond yn ymddangos yn ystafell 2
    + Bod y `gelyn` yn symud o gwmpas yr ystafell
    + Bod y gêm yn dod i ben pan mae'r `chwaraewr` yn cyffwrdd y `gelyn`

Wyt ti'n gallu creu `gelyn` yn ystafell 3 sy'n symud lan a lawr trwy'r gap yn y wal?

![sgrinlun](images/world-enemy2.png)