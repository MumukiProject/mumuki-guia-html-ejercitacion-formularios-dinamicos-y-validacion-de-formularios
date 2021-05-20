Continuemos trabajando sobre el formulario de pago que realizamos anteriormente :grin:. Aplicá las siguientes validaciones:

**Paso 1: Campo del número de la tarjeta de crédito.**

- El campo debe tener 16 caracteres. Al salirse del foco de este input, y en el caso de no cumplir con este requerimiento, el borde del input debe colorearse de rojo, borraremos el contenido el input y mostraremos el siguiente mensaje de error mediante un `alert`:  _La tarjeta debe contener 16 caracteres._ 
- Adicionaremos un input de tipo selector con 2 opciones. Visa y Mastercard. Esto no debe estar disponible para la edición del usuario, pero aplicaremos un cambio dada la siguiente condición: Si el número ingresado por el usuario inicia con 5. Será Mastercard, si comienza con 3 o 4 será visa. Y si inicia con otro valor mostraremos un mensaje de error indicando el número ingresado es erróneo.

**Paso 2: Campo nombre.**

- Validar que el campo de nombre posea solo texto. Lo validaremos con una regex, en el caso de no cumplir con este requerimiento mostraremos el siguiente mensaje de error mediante un `alert`: _El nombre debe contener solo letras._

**Paso 3: CCV.**

- Valida que posea solo números
- Que su contenido sea 3 caracteres en el caso de visa y 4 en el caso de mastercard. Por lo que habilitaremos esta opción una vez haya completado correctamente el campo numérico.

En el Paso 1: Usaremos `blur` y `change`

Mientras que las validaciones del Paso 2 y Paso 3 las haremos al clickear el botón Pagar.

> Creá el código HTML y JavaScript que acabamos de describir.
