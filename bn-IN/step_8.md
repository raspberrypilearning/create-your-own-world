## জনগণ

আপনার `player` sprite র সাথে যোগাযোগ করতে পারে এমন জনগণ আপনার বিশ্বে যুক্ত করুন।.

\--- task \---

`person` sprite তে স্যুইচ করুন।.

![Person sprite](images/person.png)

\--- /task \---

\--- task \---

`person` sprite কিছু কোড যুক্ত করুন যাতে ব্যক্তিটির `player` sprite র সাথে কথা হয়।. এই কোডটি আপনার `sign` sprite এ যুক্ত কোডের সাথে খুব মিল:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
    end
end
```

\--- /task \---

\--- task \---

`person` sprit কে আপনার অনুমতি দিন, এই দুটি ব্লক যুক্ত করে সরাতে `else`{:class="block3control"} স্থানে আপনার কোড বিভাগে:

![person](images/person.png)

```blocks3
when flag clicked
go to x: (0) y: (-150)
forever
    if < touching (player v)? > then
        say [Did you know that you can go through orange and yellow doors?]
    else
        say []
+       move (1) steps
+       if on edge, bounce
    end
end
```

\--- /task \---

আপনার `person` sprite এখন স্থানান্তরিত হবে, তবে `player` sprite র সাথে কথা বলা বন্ধ করবে।.

![screenshot](images/world-person-test.png)

\--- task \---

আপনার নতুন `person` sprite কোড যুক্ত করুন যাতে sprite টি কেবলমাত্র রুম 1 এ উপস্থিত হয়।. আপনার প্রয়োজনীয় কোডটি কোডের মতো হ'ল `sign` sprite কে কেবল রুম 1 এ দৃশ্যমান করে তোলে।.

নিশ্চিত হয়ে নিন যে আপনি আপনার নতুন কোডটি পরীক্ষা করেছেন।.

\--- /task \---