## প্লেয়ার sprite টি সরান

`player` sprite তৈরি করে শুরু করুন যা আপনার বিশ্বজুড়ে চলাফেরা করতে পারে।.

\--- task \---

'Create your own world' scratch স্টার্টার প্রকল্পটি খুলুন।.

**online**: [rpf.io/create-your-own-world-on](http://rpf.io/create-your-own-world-on){:target="_blank"} অনলাইন স্টার্টার প্রকল্পটি খুলুন.

আপনার যদি scratch অ্যাকাউন্ট থাকে তবে আপনি **Remix** ক্লিক করে একটি অনুলিপি তৈরি করতে পারেন।.

** offline **: স্টার্টার প্রকল্পটি ডাউনলোড করুন [rpf.io/p/en/create-your-own-world-go](http://rpf.io/p/en/create-your-own-world-go){:target="_blank"}এবং এটি খুলুন অফলাইন সম্পাদক ব্যবহার করে।. আপনার যদি স্ক্র্যাচ অফলাইন সম্পাদক ডাউনলোড ও ইনস্টল করতে হয় তবে আপনি এটি [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"} এ খুঁজে পেতে পারেন.

![screenshot](images/world-starter.png)

\--- /task \---

তীর কীগুলি টিপলে ` player ` স্প্রিটকে চারদিকে সরিয়ে নেওয়া উচিত।. যখন উপরের তীরটি টিপানো হয় তখন ` player ` sprite র প্রতিক্রিয়া হিসাবে স্টেজের উপরের দিকে সরে যেতে হবে।.

\--- task \---

` player ` স্প্রাইটে এই কোডটি যুক্ত করুন:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

পতাকাটিতে ক্লিক করুন এবং তারপরে উপরের তীরটি ধরে রাখুন।. ` player ` sprite কি উপরে চলেছে?

![screenshot](images/world-up.png)

\--- /task \---

\--- task \---

`player` sprite কে বাম দিকে সরানোর জন্য, আপনাকে অনুরূপ কোড সহ `if`{:class="block3control"} ব্লক যোগ করতে হবে:

![player](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

\--- /task \---

\--- task \---

আপনার ` player ` sprite আরও কোড যুক্ত করুন যাতে এটি নীচে এবং ডানদিকেও যেতে পারে।. সাহায্য পেতে যে কোডটি আপনার কাছে রয়েছে সেটি ব্যবহার করুন।.

\--- hints \---

\--- hint \---

উপরে যেতে, আপনি `player` sprite ` 0 ` ডিগ্রি দিকে নির্দেশ করুন।. Sprite টি নীচে নামাতে আপনাকে কী করতে হবে?

বাম দিকে যেতে, আপনি sprite টি `-90` ডিগ্রি দিকে নির্দেশ করুন।. স্প্রাইটটি ডানদিকে সরানোর জন্য আপনাকে কী করতে হবে?

\--- /hint \---

\--- hint \---

আপনাকে এই দুটি ব্লক পরিবর্তন করতে হবে:

![player](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

কোডটিকে নকল করুন যা `player` sprite কে উপরের দিকে সরায় এবং sprite টি নীচে সরানোর জন্য এই দুটি ব্লক পরিবর্তন করুন।. কোডটি আবার নকল করুন এবং sprite টি ডানদিকে সরানোর জন্য এটি পরিবর্তন করুন।.

\--- /hint \---

\--- hint \---

আপনার কোডটি দেখতে কেমন হবে তা এখানে:

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

+    if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
+    if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---