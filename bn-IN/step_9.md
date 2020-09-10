## Challenge: একটি পতিপক্ষ যুক্ত করুন

আপনি যদি চান তবে আপনার গেমটিতে পতিপক্ষ দেরও টহল দিতে যুক্ত করতে পারেন।. যদি `player` sprite কোনও শত্রূকে স্পর্শ করে, খেলাটি শেষ হয়।.

+ আপনার গেমটিতে ইতিমধ্যে একটি `enemy` sprite রয়েছে।. `enemy` sprite কোড যুক্ত করুন যাতে এটি কেবল রুম 2 এ প্রদর্শিত হয়।.

+ `enemy` sprite স্থানান্তর করতে এবং `enemy` sprite যদি `player` sprite স্পর্শ করে তবে খেলাটি শেষ করতে কোড যুক্ত করুন।. এটি আলাদা কোড ব্লকগুলিতে করা সহজ।. আপনার `enemy` sprite কোডটি কি রকম দেখতে হবে:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ আপনার নতুন কোডটি পরীক্ষা করে নিশ্চিত করুন: 
    + `enemy` sprite কেবল রুম 2 এ দৃশ্যমান
    + `enemy` sprite কক্ষটি টহল দিচ্ছে
    + গেমটি শেষ হয় যদি `player` sprite যদি `enemy` sprite স্পর্শ করে

আপনি কি 3 নম্বর রুমে আরও `enemy` sprite তৈরি করতে পারেন যা উপর নিচে টহল দেবে?

![screenshot](images/world-enemy2.png)