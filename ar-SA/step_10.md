## جمع العملات الذهبية

`لاعبك` يجب أن يكون قادراً على جمع العملات الذهبية أثناء تحركه عبر العالم.

--- task ---

أضف متغير جديد يُسمى`العملات الذهبية`{:class="blockdata"} إلى مشروعك.

--- /task ---

--- task ---

انقر بزر الماوس الأيمن فوق كائن `coin` واختر **إظهار**.

![لقطة الشاشة](images/coin.png)

--- /task ---

--- task ---

أضف تعليمة برمجية إلى كائن `العملات الذهبية` بحيث لا يظهر إلا في الغرفة 1.

![لقطة الشاشة](images/coin.png)

```blocks3
when flag clicked
forever
if <(room :: variables)=[1]> then
show
else
hide
```

--- /task ---

--- task ---

أضف تعليمة برمجية لكائن `العملات الذهبية` بحيث `يختف` {:class="block3looks"} الكائن ويضاف `1 `{:class="block3variables"} الى المتغير `العملات الذهبية`{:class="block3variables"} عندما يلمس كائن `player` الكائن `coin` لكي "يلتقطها".

![العملات الذهبية](images/coin.png)

```blocks3
when flag clicked
wait until <touching (player v)?>
change [coins v] by (1)
hide
stop [other scripts in sprite v]
```

يجب استخدام التعليمة البرمجية `أوقف النصوص الأخرى في الكائن`{:class="blockcontrol"} بحيث يختفي كائن `العملات الذهبية` من الغرفة 1 بمجرد جمعِها.

--- /task ---

--- task ---

الآن أضف تعليمة برمجية إلى المرحلة لاضافة متغير `العملات الذهبية`{:class="block3variables"} الخاص بك إلى `0 `{:class="block3variables"} في بداية اللعبة.

![المنصة](images/stage.png)

```blocks3
when flag clicked
set [coins v] to [0]
```

--- /task ---

--- task ---

قم بإختبار لعبتك. جمع عملة ذهبية يجب أن يغير النتيجة `العملات الذهبية` إلى `1 `{:class="block3variables"}.

--- /task ---