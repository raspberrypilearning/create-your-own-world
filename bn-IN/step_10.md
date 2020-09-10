## মুদ্রা সংগ্রহ

আপনার `player` sprite বিশ্বব্যাপী চলার সাথে সাথে কয়েন সংগ্রহ করতে সক্ষম হওয়া উচিত।.

\--- task \---

আপনার প্রকল্পে একটি নতুন variable যুক্ত করুন `coins`{:class="block3variables"}.

\--- /task \---

\--- task \---

`coin` sprite নির্বাচন করুন এবং **show** ক্লিক করুন।.

![screenshot](images/coin.png)

\--- /task \---

\--- task \---

আপনার নতুন কোড `coin` sprite যুক্ত করুন যাতে sprite কেবলমাত্র রুম 1 এ উপস্থিত হয়।.

![screenshot](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

\--- /task \---

\--- task \---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

কোড `stop other scripts in sprite`{:class="block3control"} যাতে প্রয়োজন হয় যে `coin` sprite একবার সংগ্রহ করার পরে রুম 1 এ প্রদর্শিত হবে।.

\--- /task \---

\--- task \---

গেমের শুরুতে আপনার`coins`{:class="block3variables"} সেট করতে স্টেজটিতে কোড যুক্ত করুন ভেরিয়েবল `0`{:class="block3variables"} গেমের শুরুতে।.

![stage](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

\--- /task \---

\--- task \---

আপনার খেলা পরীক্ষা করুন।. একটি মুদ্রা সংগ্রহ করলে আপনার স্কোর পরিবর্তন হওয়া উচিত`coins`থেকে `1`{:class="block3variables"}.

\--- /task \---