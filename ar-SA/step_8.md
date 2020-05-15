## الأشخاص

لنُضِيف أشخاصًا آخرين إلى لعبتك ليتعامل معها كائن `اللاعب`.

\--- task \---

عُد إلى كائن `الشخص`.

![كائن الشخص](images/person.png)

\--- /task \---

\--- task \---

أضف بعض التعليمات البرمجية إلى كائن `الشخص`، ليتحدث مع كائن `اللاعب`. هذه التعليمة البرمجية تشبه إلى حدٍ كبير التعليمة البرمجية التي أضفتها إلى كائن`لافتة`:

![شخص](images/person.png)

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

اسمح لكائن `الشخص` بالتحرك عن طريق إضافة هاتين الكتلتين البرمجيية في جزء كتلة`والا `{:class="block3control"}:

![شخص](images/person.png)

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

`شخصيتك` سوف تتحرك، لكن سوف تتوقف للتحدث مع كائن `اللاعب`.

![لقطة الشاشة](images/world-person-test.png)

\--- task \---

أضف تعليمة برمجية جديدة إلى كائن `الشخص` بحيث لا يظهر ذلك الكائن إلا في غرفة 1. التعليمية البرمجية التي تحتاجها هي بالضبط نفس التعليمية البرمجية التي تجعل الكائن `اللافتة` مرئيًا (ضاهرا) فقط في الغرفة 1.

تأكد من اختبار التعليمة البرمجية الجديدة.

\--- /task \---