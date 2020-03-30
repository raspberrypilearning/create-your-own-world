## Paredes macizas

--- task ---

Prueba de nuevo tu objeto `jugador`. ¿Ves que puede atravesar las paredes de color gris claro?

![captura de pantalla](images/world-walls.png)

--- /task ---

--- task ---

Para arreglar esto, tendrás que hacer que tu `jugador` retroceda si toca una pared de color gris claro. Este es el código que necesitas añadir dentro de tu bloque `para siempre`{:class="block3control"} debajo de los bloques de dirección:

![jugador](images/player.png)

```blocks3
al hacer clic en la bandera verde
por siempre 
  si <¿tecla (flecha arriba v) presionada? > entonces 
    apuntar en dirección (0)
    mover (4) pasos
  end
  si <¿tecla (flecha izquierda v) está presionada? > entonces 
    apuntar en dirección (-90)
    mover (4) pasos
  end
  si <¿tecla (flecha abajo v) presionada? > entonces 
    apuntar en dirección (-180)
    mover (4) pasos
  end
  si <¿tecla [flecha derecha v] presionada? > entonces 
        apuntar en dirección (90)
        mover (4) pasos
    fin
    si < toca el color [#BABABA]? > entonces 
  mover (-4) pasos
end
```

--- /task ---

--- task ---

Intenta hacer que el objeto `jugador` se mueva a través de una pared. Si tu nuevo código funciona, esto no debería ser posible.

![captura de pantalla](images/world-walls-test.png)

--- /task ---