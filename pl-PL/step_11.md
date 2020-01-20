## Drzwi i klucze

Teraz dodasz kod, aby niektóre drzwi w twoim świecie gry były zamknięte, a gracz musi znaleźć klucz, aby je otworzyć i przejść do następnego pokoju.

\--- task \---

Switch to the `key` sprite. Click on `show`{:class="blocklooks"} in the Scripts menu so that the sprite appears on the Stage.

\--- /task \---

\--- task \---

Edit the `key` sprite's costume so that it is blue.

\--- /task \---

\--- task \---

Switch your Stage backdrop to room 3, and place the `key` sprite somewhere difficult to reach!

![screenshot](images/world-key.png)

\--- /task \---

\--- task \---

Add code to the `key` sprite to make it only visible in room 3.

\--- /task \---

\--- task \---

Create a new list called `inventory`{:class="block3variables"} to store the items your `player` sprite collects.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

The code you need to add for collecting the key is very similar to the code for collecting coins. The difference is that you add the key to the `inventory`{:class="block3variables"}.

![key](images/key.png)

```blocks3
kiedy kliknięto zieloną flagę
czekaj aż < dotyka [gracz v]?>
dodaj [niebieski klucz] do [inwentarz v]
ukryj
zatrzymaj [inne skrypty duszka v]
```

\--- /task \---

\--- task \---

Add code to your Stage to empty your inventory at the start of the game.

```blocks3
usuń (wszystko v) z [inwentarz v]
```

\--- /task \---

\--- task \---

Test out your game to check whether you can collect the `key` sprite and add it to your inventory.

\--- /task \---

\--- task \---

Now add the locked door. Select the `door-blue` sprite and click on `show`{:class="blocklooks} in the Scripts menu, and then position the sprite across the gap between the two walls.

![screenshot](images/world-door.png)

\--- /task \---

\--- task \---

Add code to the `door-blue` sprite so that it is only visible in room 3.

\--- /task \---

\--- task \---

Add code to the `door-blue` sprite so that, when the key is in the `inventory`{:class="block3variables"}, the sprite `hides`{:class="block3looks"} to allow your `player` sprite to pass.

![door](images/door.png)

```blocks3
kiedy kliknięto zieloną flagę
czekaj aż <[inwentarz v] zawiera [niebieski klucz]?>
zatrzymaj [inne skrypty duszka v]
ukryj
```

\--- /task \---

\--- task \---

Test out your game and see if you can collect the blue key to open the door!

\--- /task \---