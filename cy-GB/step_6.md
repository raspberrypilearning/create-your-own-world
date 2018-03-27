## Casglu darnau arian

+ Ychwanega newidyn newydd o'r enw 'arian' {.blockdata} i dy brosiect.

+ Gwna clic-dde ar giplun 'darn arian' ('coin') a dewis 'dangos'.

![screenshot](images/world-coins.png)

+ Ychwanega côd i dy ddarn arian, fel ei fod ond yn ymddangos yn ystafell 1.

+ Ychwanega gôd i giplun dy ddarn arian, i ychwanegu 1 i dy 'arian' {.blockdata} unwaith maent yn cael eu casglu:

	```blocks
		pan fo ⚑ wedi ei glicio
		aros hyd at <cyffwrdd [player v]?>
		newid [coins v] gan (1)
		stopiwch [sgriptiau eraill yn y ciplun v]
		cuddio
	```

	Mae angen y côd 'stopiwch sgriptiau eraill yn y ciplun' {.blockcontrol} fel bod y darn arian yn stopio ymddangos yn ystafell 1 unwaith mae'n cael ei gasglu.

+ Bydd hefyd angen i ti ychwanegu côd fel bod newidyn dy 'arian' {.blockdata} yn cael ei osod i 0 ar ddechrau dy gêm.

+ Profa dy brosiect - fe ddylai casglu dy ddarn arian newid dy sgôr i 1.

--- challenge ---

## Her: Mwy o ddarnau o arian
Wyt ti'n gallu ychwanegu mwy o ddarnau arian i dy gêm? Mae modd iddynt fod mewn ystafelloedd gwahanol, ac fe all rhai dadrnau arian gael eu gwarchod gan elynion.

--- /challenge ---