## جمع العملات الذهبية

أثناء تحرك كائن `اللاعب` في اللعبة، يمكنه أن يجمع العملات الذهبية.

+ أضف متغير جديد يُسمى`العملات الذهبية`{:class="blockdata"} إلى مشروعك.

+ انقر بزر الفأره الأيمن فوق كائن`العملات الذهبية` واختر **إظهار**.

![screenshot](images/world-coins.png)

+ أضف تعليمة برمجية إلى كائن `العملات الذهبية` بحيث لا يظهر إلا في الغرفة 1.

+ أضف تعليمة برمجية لكائن `العملات الذهبية` بحيث يضاف `1` إلى متغير `العملات الذهبية`{:class="blockdata"} عندما يلمس كائن `اللاعب` كائن `العملات الذهبية` لكي يلتقطها.
    
    ```blocks
        عند نقر العلم 
    انتظهر حتى <touching [player v]?>
    غير [coins v] بمقدار (1)
    أوقف [other scripts in sprite v]
    أخفِ
    ```
    
    يجب استخدام التعليمة البرمجية `أوقف النصوص الأخرى في الكائن` بحيث يختفي كائن `العملات الذهبية` من الغرفة 1 بمجرد جمعِها.

+ وستحتاج أيضا إلى إضافة تعليمة برمجية لضبط متغير `العملات الذهبية`{:class="blockdata"} إلى `0` في بداية اللعبة.

+ Test your project — collecting a coin should change your `coins` score to `1`.

\--- challenge \---

### Challenge: more coins

Can you add more coins to your game? They can be in different rooms, and some coins could even be guarded by patrolling enemies!

\--- /challenge \---