## দরজা এবং চাবি

এখন আপনি কোড যুক্ত করবেন যাতে আপনার গেম এ কয়েকটি দরজা লক হয়ে যায় এবং প্লেয়ারকে অবশ্যই সেগুলি খোলার জন্য এবং পরবর্তী ঘরে যেতে হবে চাবিটি খুঁজে পেতে.

\--- task \---

`key` sprite স্যুইচ করুন।. স্ক্রিপ্ট মেনুতে `show`{:class="blocklooks"} ক্লিক করুন যাতে sprite স্টেজটিতে উপস্থিত হয়।.

\--- /task \---

\--- task \---

`key` sprite's costume এমনভাবে সম্পাদনা করুন যাতে এটি নীল হয়.

\--- /task \---

\--- task \---

আপনার স্টেজের ব্যাকড্রপটি রুম 3 তে স্যুইচ করুন এবং `key` sprite কোথাও পৌঁছানোর পক্ষে শক্ত করুন!

![screenshot](images/world-key.png)

\--- /task \---

\--- task \---

কেবলমাত্র ঘরে 3 এ দৃশ্যমান করতে `Key` sprite কোড যুক্ত করুন।.

\--- /task \---

\--- task \---

নতুন লিস্ট তৈরী করুন `inventory`{:class="block3variables"}যেখানে আপনি আপনার `player` আইটেম স্টোরে করতে পারবেন এবং sprite সংগ্রহ করতে পারবেন.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

Key টি সংগ্রহ করার জন্য আপনার যে কোডটি যুক্ত করতে হবে তা মুদ্রা সংগ্রহের কোডের সাথে খুব মিল।. পার্থক্য হ'ল আপনি চাবি টি `inventory`{:class="block3variables"} যুক্ত করেছেন.

![key](images/key.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```

\--- /task \---

\--- task \---

গেমের শুরুতে আপনার জায়াগুলি খালি করতে আপনার পর্যায়ে কোড যুক্ত করুন।.

```blocks3
delete all of [inventory v]
```

\--- /task \---

\--- task \---

আপনি `key` sprite সংগ্রহ করতে এবং এটি আপনার জায়টিতে যুক্ত করতে পারেন কিনা তা পরীক্ষা করতে আপনার গেমটি পরীক্ষা করে দেখুন।.

\--- /task \---

\--- task \---

এবার তালাবদ্ধ দরজাটি যুক্ত করুন।. `door-blue` sprite নির্বাচন করুন এবং স্ক্রিপ্ট মেনুতে `show`{:class="blocklooks} এ ক্লিক করুন এবং তারপরে দুটি প্রাচীরের মধ্যবর্তী ফাঁক জুড়ে sprite অবস্থান দিন।.

![screenshot](images/world-door.png)

\--- /task \---

\--- task \---

`door-blue` sprite কোড যুক্ত করুন যাতে এটি কেবল 3 নম্বর ঘরে দৃশ্যমান হয়।.

\--- /task \---

\--- task \---

কোড যুক্ত করুন `door-blue` sprite যাতে চাবি `inventory`{:class="block3variables"}, sprite `hides`{:class="block3looks"} আপনাকে অনুমতি দিতে `player` sprite পাস করতে.

![door](images/door.png)

```blocks3
when flag clicked
wait until <[inventory v] contains [blue key]?>
stop [other scripts in sprite v]
hide
```

\--- /task \---

\--- task \---

আপনার গেমটি পরীক্ষা করুন এবং দেখুন যে আপনি দরজা খোলার জন্য নীল কীটি সংগ্রহ করতে পারেন কিনা!

\--- /task \---