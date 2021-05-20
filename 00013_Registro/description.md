Antes de enviar el [formulario de registro de cliente](mumukiproject/mumuki-guia-html-ejercitacion-formularios/4) creado con anterioridad, realizaremos algunas validaciones sobre este. Pero primero, agregaremos una etiqueta small debajo de cada input con un color rojo y de inicio no va a visualizarse.

Los errores y las validaciones a mostrar deben ser las siguientes:

- **Nombre:** "El campo nombre solo puede contener texto";
- **Apellido:** "El campo apellido solo puede contener texto";
- **DNI:** "El DNI no puede ser mayor a 8 caracteres";
- **Email:** "El formato del email no es válido";
- **Contraseña:** En este caso utilizaremos 2. "La contraseña debe tener al menos 8, al menos un dígito, al menos una minúscula, al menos una mayúscula y al menos un caracter especial" y "Las contraseñas no coinciden";
- **Términos y condiciones de uso:** "Debe aceptar los términos y condiciones".

En el caso de que alguno de los inputs no cumpla con las características solicitadas, debemos visualizar el error correspondiente a ese input.

Usar las siguientes funciones para validar los datos con expresiones regulares:

```javascript
function esEmailValido(email) {
  const regex = /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
  return regex.test(email.toLowerCase())
}

function esPasswordValida(password) {
  const regex = /^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$/gm
  return regex.test(password)
}
```
> Creá el código HTML y JavaScript que acabamos de describir.