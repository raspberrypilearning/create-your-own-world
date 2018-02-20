## Signs

Let's add signs to your world to guide the player on their journey.

+ Your project includes a `welcome sign` sprite:

![screenshot](images/world-sign.png)

+ The `welcome sign` sprite should only be visible in room 1, so add some code to the `welcome sign` sprite to make sure that this happens:

```blocks
    when flag clicked
    forever
        if < (room) = [1] > then
            show
        else
            hide
        end
    end
```

+ Test your `welcome sign` sprite by moving between rooms. Your sign should only be visible in room 1.
    
    ![screenshot](images/world-sign-test.png)

+ A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

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