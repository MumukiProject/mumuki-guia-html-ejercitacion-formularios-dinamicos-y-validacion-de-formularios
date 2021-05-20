Queremos crear una página que nos permita enviar comentarios :speech_balloon:, se espera que la misma:

- tenga un `textarea` que inicialmente está vacío;
- un `span` debajo de este que comience diciendo `0/240 caracteres`;
- un botón que diga `Enviar`;
- cuando se escribe algo en el `textarea`, se actualice el texto para reflejar la cantidad de caracteres restantes. Por ejemplo: si en el `textarea` escribimos un texto de 10 caracteres debería decir `230/240 caracteres`;
- al presionar el botón `Enviar`, si hay 240 caracteres o menos, se borre el contenido del input y se actualice el texto para que diga `Comentario enviado`;
- el color del borde del `textarea` cambie de la siguiente forma:
  - normal si está vacío;
  - verde si tiene texto y 240 caracteres o menos;
  - rojo si tiene más de 240 caracteres.

> Creá el código HTML y JavaScript que acabamos de describir.