## Συμπαγείς τοίχοι

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls?

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Εδώ είναι ο κώδικας που πρέπει να προσθέσεις στο εσωτερικό του μπλοκ `για πάντα`{:class="block3control"} κάτω από το μπλοκ κατεύθυνσης:

![παίκτης](images/player.png)

```blocks3
Όταν στην πράσινη σημαία γίνει κλικ
για πάντα 
  εάν <πατήθηκε το πλήκτρο (Πάνω βέλος v) :: sensing > τότε 
    στρίψε προς την κατεύθυνση των (0) μοιρών :: motion
    κινήσου (4) βήματα :: motion :: control
  end
  εάν <πατήθηκε το πλήκτρο (αριστερό βέλος v) :: sensing > τότε 
    στρίψε προς την κατεύθυνση των (-90) μοιρών :: motion
    κινήσου (4) βήματα :: motion :: control
  end
  εάν <πατήθηκε το πλήκτρο (κάτω βέλος v) :: sensing > then
        point in direction (180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > τότε 
    στρίψε προς την κατεύθυνση των (90) μοιρών :: motion
    κινήσου (4) βήματα :: motion :: control
  end
  + εάν <αγγίζει το χρώμα [#BABABA] :: sensing > τότε 
  +   κινήσου (-4) βήματα :: motion :: control
  + end :: control
end
```

\--- /task \---

\--- task \---

Προσπάθησε να κάνεις τον `παίκτη`να περάσει μέσα από έναν τοίχο. Αν ο νέος σου κώδικας λειτουργεί, αυτό θα πρέπει να είναι αδύνατον.

![screenshot](images/world-walls-test.png)

\--- /task \---