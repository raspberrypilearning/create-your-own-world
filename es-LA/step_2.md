## Mueve el objeto jugador

Empieza creando un objeto `jugador` que se pueda mover por tu mundo.

--- task ---

Abre el proyecto de inicio de Scratch "Crea tu propio mundo".

**En línea:** abre el proyecto de inicio en [scratch.mit.edu/projects/414615338](https://scratch.mit.edu/projects/414615338){:target="_blank"}.

Si tiene una cuenta de Scratch, puede hacer una copia haciendo clic en **Remix**.

**Sin conexión:** descarga el proyecto de inicio desde [rpf.io/p/es-LA/create-your-own-world-go](http://rpf.io/p/es-LA/create-your-own-world-go) y luego ábrelo con el editor de Scratch sin conexión. Si necesitas descargar e instalar el editor offline de Scratch, puedes encontrarlo en [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![captura de pantalla](images/world-starter.png)

--- /task ---

Al presionar las teclas de flecha se moverá al objeto `jugador`. Cuando se presiona la flecha hacia arriba, el objeto `jugador` debe moverse hacia arriba en el escenario.

--- task ---

Añade este código al objeto `jugador`:

![jugador](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
end
```

--- /task ---

--- task ---

Haz clic en la bandera y mantén presionada la flecha hacia arriba. ¿El objeto `jugador` se mueve hacia arriba?

![captura de pantalla](images/world-up.png)

--- /task ---

--- task ---

Para mover el `jugador` hacia la izquierda tienes que añadir otro bloque `si`{:class="block3control"} con un código similar:

![jugador](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
+   if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end
end
```

--- /task ---

--- task ---

Añade más código a tu objeto `jugador` para que pueda moverse también hacia abajo y hacia la derecha. Usa el código que ya tienes como ayuda.

--- hints ---


--- hint ---

Para moverse hacia arriba, apunta el objeto `jugador` en la dirección `0` grados. ¿Qué tienes que hacer para mover el objeto hacia abajo?

Para moverse hacia la izquierda, apunta el objeto jugador en la dirección `90` grados. ¿Qué tienes que hacer para mover el objeto hacia la derecha?

--- /hint ---

--- hint ---

Necesitas cambiar estos dos bloques:

![jugador](images/player.png)

```blocks3
<key ( v) pressed>

point in direction ()
```

Duplica el código que hace que el objeto `jugador` se mueva hacia arriba y cambia estos dos bloques para que el objeto se mueva hacia abajo. Duplica el código nuevamente y cámbialo para que el objeto se mueva hacia la derecha.

--- /hint ---

--- hint ---

Así es como debería verse tu código:

![jugador](images/player.png)

```blocks3
when flag clicked
forever
    if <key (up arrow v) pressed? > then
        point in direction (0)
        move (4) steps
    end
    if <key (left arrow v) pressed? > then
        point in direction (-90)
        move (4) steps
    end

+    if <key (down arrow v) pressed? > then
        point in direction (180)
        move (4) steps
    end
+    if <key (right arrow v) pressed? > then
        point in direction (90)
        move (4) steps
    end
end
```

--- /hint ---

--- /hints ---

--- /task ---