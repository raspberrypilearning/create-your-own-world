## Σημάδια

Ας προσθέσουμε σημάδια στον κόσμο μας που θα καθοδηγούν τους παίκτες στο ταξίδι τους.

Το έργο περιλαμβάνει ένα `σημάδι καλωσορίσματος`:

![screenshot](images/world-sign.png)

\--- task \--- Το ` σημάδι καλωσορίσματος` θα πρέπει να είναι ορατό μονάχα στην αίθουσα 1, έτσι θα πρέπει να προσθέσεις κώδικα στο αντικείμενο αυτό, προκειμένου να βεβαιωθείς πως αυτό επιτυγχάνεται:

\--- hints \--- \--- hint \--- `Όταν η σημαία πατηθεί`{:class="block3events"}, μέσα σε ένα `για πάντα`{:class="block3control"} βρόγχο επανάληψης, έλεγξε `εάν`{:class="block3control"} η `αίθουσα έχει τιμή 1`{:class="block3variables"} και τότε `εμφάνισε` το {:class="block3looks"} `σημάδι καλωσορίσματος`, `διαφορετικά`{:class="block3control"} `εξαφάνισε`{:class="block3looks"} το αντικείμενο. \--- /hint \--- \--- hint \--- Εδώ είναι τα μπλοκ εντολών που θα χρειαστείς:

![sign](images/sign.png)

```blocks3
<br />εάν &lt; &gt; τότε
αλλιώς
end

&lt; (αίθουσα :: variables) = [1] &gt;

εξαφάνισε

εμφάνισε

για πάντα
end

Όταν γίνει κλικ σε σημαία

```

\--- /hint \--- \--- hint \--- Here is the complete code:

![sign](images/sign.png)

```blocks3
when flag clicked
forever
    if < (room :: variables) = [1] > then
        show
    else
        hide
    end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \--- Test the code for your `welcome sign` sprite by moving between rooms. The sign should only be visible in room 1.

![screenshot](images/world-sign-test.png) \--- /task \---

\--- task \--- A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

```blocks3
when flag clicked
forever
if < (room :: variables) = [1] > then
show
else
hide
end
+if < touching (player v)? > then
say [Welcome! Can you get to the treasure?]
else
say []
end
end
```

\--- /task \---

\--- task \--- Test your `welcome sign` sprite again. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![screenshot](images/world-sign-test2.png) \--- /task \---