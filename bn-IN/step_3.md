## শক্ত দেওয়াল

--- task ---

আপনার ` player` sprite আবার পরীক্ষা করুন।. এটি কি হালকা ধূসর দেওয়াল দিয়ে হাঁটতে পারে?

![screenshot](images/world-walls.png)

--- /task ---

--- task ---

এটি ঠিক করার জন্য, আপনাকে হালকা ধূসর প্রাচীরের ছোঁয়ায় `player` sprite টি আবার সরানো দরকার।. আপনার `forever`{:class="block3control"} নিচের দিকের ব্লকগুলিতে আপনার যে কোডটি যুক্ত করতে হবে তা এখানে:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
        if <key (down arrow v) pressed? > then
        point in direction (-180)
        move (4) steps
    end
        if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

--- /task ---

--- task ---

`player` sprite টিকে কোনও প্রাচীরের মধ্যে দিয়ে নিয়ে যাওয়ার চেষ্টা করুন।. যদি আপনার নতুন কোডটি কাজ করে তবে এটি সম্ভব হবে না।.

![screenshot](images/world-walls-test.png)

--- /task ---