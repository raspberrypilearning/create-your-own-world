## Люди

Додай інших людей до свого світу, з якими міг би взаємодіяти спрайт `гравець`.

\--- task \---

Вибери спрайт `персонаж`.

![Спрайт персонажа](images/person.png)

\--- /task \---

\--- task \---

Додай код до спрайта `персонаж`, щоб він говорив до спрайта `гравець`. Цей код дуже схожий до коду, який ти додав(-ла) до свого спрайту `табличка`:

![персонаж](images/person.png)

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

Дозволь своєму спрайту `персонаж` переміщуватися, додавши наступні два блоки в частину коду `інакше`{:class="block3control"}:

![персонаж](images/person.png)

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

Твій спрайт `персонаж` тепер рухатиметься, але перестане говорити зі спрайтом `гравець`.

![знімок екрана](images/world-person-test.png)

\--- task \---

Додай код до нового спрайта `персонаж`, щоб він з’являвся тільки в кімнаті 1. Необхідний для цього код точно такий же, як і код для того, щоб спрайт `табличка` відображався тільки в кімнаті 1.

Обовʼязково протестуй свій новий код.

\--- /task \---