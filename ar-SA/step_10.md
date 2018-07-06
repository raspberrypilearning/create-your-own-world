## جمع العملات الذهبية

أثناء تحرك كائن `اللاعب` في اللعبة، يمكنه أن يجمع العملات الذهبية.

+ أضف متغير جديد يُسمى`العملات الذهبية`{:class="blockdata"} إلى مشروعك.

+ انقر بزر الفأره الأيمن فوق كائن`العملات الذهبية` واختر **إظهار**.

![screenshot](images/world-coins.png)

+ أضف تعليمة برمجية إلى كائن `العملات الذهبية` بحيث لا يظهر إلا في الغرفة 1.

+ أضف تعليمة برمجية لكائن `العملات الذهبية` بحيث يضاف `1` إلى متغير `العملات الذهبية`{:class="blockdata"} عندما يلمس كائن `اللاعب` كائن `العملات الذهبية` لكي يلتقطها.
    
    ```blocks
        when flag clicked
        wait until <touching [player v]?>
        change [coins v] by (1)
        stop [other scripts in sprite v]
        hide
    ```
    
    The code `stop other scripts in sprite`{:class="blockcontrol"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

+ You'll also need to add code to set your `coins`{:class="blockdata"} variable to `0` at the start of your game.

+ Test your project — collecting a coin should change your `coins` score to `1`.

\--- challenge \---

### Challenge: more coins

Can you add more coins to your game? They can be in different rooms, and some coins could even be guarded by patrolling enemies!

\--- /challenge \---