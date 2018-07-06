## الأشخاص

لنُضِيف أشخاصًا آخرين إلى لعبتك ليتعامل معها كائن `اللاعب`.

+ عُد إلى كائن `الشخص`.

![Person sprite](images/person-sprite.png)

+ أضف بعض التعليمات البرمجية إلى كائن `الشخص`، ليتحدث مع كائن `اللاعب`. هذه التعليمة البرمجية تشبه إلى حدٍ كبير التعليمة البرمجية التي أضفتها إلى كائن`لافتة `:

```blocks
    عند النقر على العلم
إذهب إلى موضع س:(0) ص:(-150)
كرر باستمرار
إذا < ملامس لـ [player v]؟ >
قل [Did you know that you can go through orange and yellow doors?]
  else
            قل []
        end
    end
```

+ ويمكنك أيضًا أن تسمح لكائن `الشخص` بالتحرك عن طريق إضافة هذين القالبين البرمجيين في التعليمة البرمجية `else`{:class="blockcontrol"}:

```blocks
تحرك (1) خطوات
ارتد إذا كنت عند الحافة
```

سيتحرك الآن كائن `الشخص`، لكن لن يتوقف ليتحدث مع كائن `اللاعب`.

![screenshot](images/world-person-test.png)

\--- challenge \---

### التحدي: تحسين الشخص

Can you add code to your new `person` sprite so that they only appear in room 1? Make sure you test out your new code.

\--- /challenge \---