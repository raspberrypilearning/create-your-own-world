## اللافتات

لنُضِف لافتات إلى لعبتك لتوجيه اللاعب على مدار اللعبة.

+ يحتوي مشروعك على كائن `لافتة الترحيب`:

![screenshot](images/world-sign.png)

+ يجب أن يظهر كائن ` لافتة الترحيب` في الغرفة الأول فقط، لذا أضف بعض التعليمات البرمجية إلى كائن `لافتة الترحيب` لتضمن حدوث ذلك:

```blocks
    عند نقر العلم 
كرر باستمرار
        إذا < (room) = [1] > then
إظهر 
else
اختفِ 
النهاية 
النهاية
```

+ اختبر كائن `لافتة الترحيب` بتحريك اللاعب بين الغرف. يجب أن تظهر الافتة في الغرفة 1 فقط.
    
    ![screenshot](images/world-sign-test.png)

+ لا يكون للافتة ميزة في اللعبة إذا لم تظهر أي رسالة! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

```blocks
    when flag clicked
    forever
        if < (room) = [1] > then
            show
        else
            hide
        end
        if < touching [player v]? > then
            say [Welcome! Can you get to the treasure?]
        else
            say []
        end
    end
```

+ Test out your `welcome sign` sprite — you should now see a message when the `player` sprite touches it.

![screenshot](images/world-sign-test2.png)