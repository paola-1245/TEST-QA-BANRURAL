# Estrategia de Testeo y Correcciones

## Error 1: No se puede leer la propiedad 'null'
**Descripción**: La consola arrojaba un error cuando se intentaba acceder a un elemento del DOM que no existía o cuyo ID era incorrecto.
**Solución**: Revisé los IDs y aseguré que el JavaScript se ejecutara después de cargar el DOM usando `window.onload`.

## Error 2: Validación de entrada no permitía manejar correctamente números no enteros.
**Descripción**: El usuario podía ingresar valores no enteros o fuera del rango, lo cual causaba que el juego fallara.
**Solución**: Implementé validación para asegurarme de que el valor ingresado sea un número entero entre 1 y 100. Si la entrada es incorrecta, no se cuenta como intento y se muestra una alerta.

## Error 3: Los mensajes no mostraban el color correcto al comparar números.
**Descripción**: Los mensajes "El número es mayor" y "El número es menor" no aparecían con el color negro requerido.
**Solución**: Apliqué el estilo directamente desde el JavaScript con `element.style.color`.

## Error 4: El juego no terminaba al adivinar el número o llegar al límite de intentos.
**Descripción**: No había lógica para finalizar el juego cuando el jugador ganaba o perdía.
**Solución**: Agregué la lógica que deshabilita el campo de entrada y muestra los mensajes correctos cuando el jugador gana o pierde.
