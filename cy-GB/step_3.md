## Waliau cadarn

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
  os <bysell (up arrow v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (0)
    symud (4) cam
  end
  os <bysell (left arrow v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (-90)
    symud (4) cam
  end
  os <bysell (down arrow v) wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (-180)
    symud (4) cam
  end
  os <bysell [right arrow v] wedi ei phwyso? > yna 
    pwyntio i gyfeiriad (90)
    symud (4) cam
  end
  + os <cyffwrdd lliw [#BABABA] ? > yna 
  +   symud (-4) cam
  + end
end
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---