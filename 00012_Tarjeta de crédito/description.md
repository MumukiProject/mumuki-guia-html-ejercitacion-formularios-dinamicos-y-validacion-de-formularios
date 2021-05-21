Continuemos trabajando sobre el formulario de pago que realizamos anteriormente :grin:. Para eso vamos a aplicar las siguientes validaciones:

**Número de la tarjeta de crédito:** :credit_card:

- el campo debe tener 16 caracteres. Al salirse del foco de este `input`, y en el caso de no cumplir con este requerimiento, el borde del mismo debe colorearse de rojo y debemos borrar su contenido. El error se muestra mediante un `alert` _La tarjeta debe contener 16 caracteres_.
- vamos a agregar un `input` de tipo selector con las opciones _Visa_ y _Mastercard_. Esto no debe estar disponible para la edición del usuario, pero el cambio se aplicará dada la siguiente condición:
  - Si el número ingresado por el usuario inicia con 5 será Mastercard.
  - Si comienza con 3 o 4 será visa.
  - Si inicia con otro valor mostraremos un alert con el mensaje _El número ingresado es erróneo_.

**Nombre:** :bust_in_silhouette:

- validaremos a través de una regex que este campo solo debe contener texto. En caso de no cumplir con este requerimiento mostraremos un `alert` que diga: _El nombre debe contener solo letras_.

**CCV:** :asterisk_symbol::asterisk_symbol::asterisk_symbol:

- este campo solo debe contener números;
- su contenido debe tener 3 caracteres en el caso de visa y 4 en el caso de mastercard. Por lo que habilitaremos esta opción una vez haya completado correctamente el campo con el número de la tarjeta de crédito.
- en caso que el CCV no sea válido mostraremos un `alert` con el mensaje: _El CCV no es válido_.

Para el número de tarjeta de crédito utilizaremos los eventos `blur` y `change`. En cambio, las validaciones del nombre y el CCV las haremos al clickear el botón _Pagar_.

> Creá el código HTML y JavaScript que acabamos de describir.
