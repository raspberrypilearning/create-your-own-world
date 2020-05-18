## اللافتات

أضف الآن إشارات إلى عالمك لإرشاد اللاعبين في رحلتهم.

يحتوي مشروعك على كائن `لافتة الترحيب`:

![لقطة شاشة](images/world-sign.png)

--- task ---

يجب أن يكون كائن `علامة الترحيب` مرئيًا فقط في الغرفة 1، لذلك أضف بعض التعليمات البرمجية إلى الكائن للتأكد من حدوث ذلك:

--- hints ---


--- hint ---

`عند النقر على العلم`{:class="block3events"}, في حلقة `كرر باستمرار`{:class="block3events"}, تحقق من `اذا`{:class="block3control"} كانت `الغرفة هي 1`{:class="block3variables"} في هذه الحالة `أظهر `{:class="block3looks"} كائن `علامة الترحيب` و`الا`{:class="block3control"} قم بـ`اخفاء`{:class="block3looks"} الكائن.

--- /hint ---

--- hint ---

إليك التعليمات البرمجية التي تحتاجها:

![لافتة](images/sign.png)

```blocks3
if < > then
else
end

< (غرفة :: variables) = [1] >

hide

show

forever
end

when flag clicked

```

--- /hint ---

--- hint ---

اليك التعليمة البرمجية الكاملة:

![لافتة](images/sign.png)

```blocks3
when flag clicked
forever
    if < (غرفة :: variables) = [1] > then
        show
    else
        hide
    end
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

اختبر الرمز الخاص بكائن `علامة الترحيب` عن طريق الانتقال بين الغرف. يجب أن تظهر اللافتة في الغرفة 1 فقط.

![لقطة الشاشة](images/world-sign-test.png)

--- /task ---

--- task ---

لا يكون للافتة ميزة في اللعبة إذا لم تظهر أي رسالة! أضف بعض الرموز لعرض رسالة إذا كان كائن `لافتة الترحيب` يلامس كائن `اللاعب`:

![لافتة](images/sign.png)

```blocks3
when flag clicked
forever
if < (غرفة :: variables) = [1] > then
show
else
hide
end
+if < touching (اللاعب v)? > then
say [مرحبا! هل يمكنك الوصول إلى الكنز؟]
else
say []
end
end
```

--- /task ---

--- task ---

اختبر كائن `علامة الترحيب` مرة أخرى. يجب أن تشاهد الآن رسالة عندما يتلامس `اللاعب` و `علامة الترحيب`.

![لقطة الشاشة](images/world-sign-test2.png)

--- /task ---