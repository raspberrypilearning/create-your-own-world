## Türen und Schlüssel

Jetzt wirst du Code hinzufügen, damit einige Türen in deiner Spielwelt gesperrt sind, und der Spieler den Schlüssel findenmuss, um sie zu öffnen und zum nächsten Raum zu gelangen.

--- task --- Wechsel zur `Schlüssel`-Figur. Klicke auf `zeige dich`{:class="block3looks"}, damit das Objekt auf der Bühne erscheint. --- /task ---

--- task --- Bearbeite das Kostüm des `Schlüssels` so, dass es blau ist. --- /task ---

--- task --- Wechsle nun zum Bühnenbil in Raum 3 und platziere die `Schlüssel`-Figur an einer schwer erreichbaren Stelle!

![Screenshot](images/world-key.png)

--- /task ---

--- task --- Füge Code zu deiner `Schlüssel`-Figur hinzu, sodass sie nur in Raum 3 erscheint. --- /task ---

--- task --- Erstelle eine neue Liste namens `Inventar`{:class="block3variables"}, um die Gegenstände zu speichern, die deine `Spieler`-Figur sammelt.

[[[generic-scratch3-make-list]]] --- /task ---

--- task --- Der Code zum Einsammeln des Schlüssels ist dem Code zum Einsammeln von Münzen sehr ähnlich. Der Unterschied ist, dass du den Schlüssel zum `Inventar`{:class="block3variables"}} hinzufügst.

![key](images/key.png)

```blocks3
Wenn die grüne Flagge angeklickt
warte bis <wird (Spieler v) berührt?>
füge [blauer Schlüssel] zu [Inventar v] hinzu
verstecke dich
stoppe [andere Skripte der Figur v]
```

--- /task ---

--- task --- Füge Code zu deiner Bühne hinzu, um das Inventar bei Spielbeginn zu leeren.

```blocks3
lösche (alles v) aus [Inventar v]
```

--- /task ---

--- task --- Teste dein Spiel, um zu überprüfen, ob du den `Schlüssel` sammeln und in dein Inventar einfügen kannst. --- /task ---

--- task --- Nun füge die verschlossene Tür hinzu. Wähle die `Tür-blau`-Figur aus und klicke auf `zeige dich`{:class="block3looks}. Und platziere die Figur dann über die Lücke zwischen den beiden Wänden.

![Screenshot](images/world-door.png) --- /task ---

--- task --- Füge Code zur `Tür-blau`-Figur hinzu, sodass sie nur in Raum 3 erscheint. --- /task ---

--- task --- Füge Code zur `Tür-blau`-Figur hinzu damit sich die Figur `versteckt`{:class="block3looks"}, wenn der Schlüssel im `Inventar`{:class="block3variables"} ist, sodass deine `Spieler`-Figur durchgehen kann.

![Tür](images/door.png)

```blocks3
Wenn die grüne Flagge angeklickt
warte bis <[Inventar v] enthält [blauer Schlüssel] ?>
stoppe [andere Skripte der Figur v]
verstecke dich
```

--- /task ---

--- task --- Teste dein Spiel und überprüfe, ob du den blauen Schlüssel einsammeln kannst um die Tür zu öffnen! --- /task ---