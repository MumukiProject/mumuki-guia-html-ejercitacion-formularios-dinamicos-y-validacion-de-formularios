Necesitamos crear una página que nos ayude a convertir valores de distancia :straight_ruler:, se espera que la misma:

- tenga:
  - un `input` para ingresar el valor a convertir;
  - un `select` para seleccionar la unidad del valor convertido;
  - un `select` para seleccionar la unidad a convertir;
  - un botón que diga `Intercambiar`;
  - un texto que muestre el resultado;
- cuyos `select`s tengan las siguientes opciones:
  - kilómetros (km);
  - metros (m);
  - decímetros (dm);
  - centímetros (cm);
  - milímetros (mm);
- ambos `select` comiencen con la opción `metros` seleccionada y el `input` comience con el valor `1`;
- al seleccionar una nueva opción en cualquiera de los `select` o al modificar el valor del input, se actualice el texto con el resultado de la conversión del valor ingresado de una unidad a la otra;
- al clickear el botón `Intercambiar` se intercambien las opciones de los `select`s y se actualice el texto.


:warning: Consideraciones:

Para realizar este ejercicio, el `value` de cada option del `select` deben ser los siguientes:

- para `Kilómetros`, el value debe ser `1000`;
- para `Metros`, el value debe ser `1`;
- para `Decímetros`, el value debe ser `0.1`;
- para `Centímetros`, el value debe ser `0.01`;
- para `Milímetros`, el value debe ser `0.001`.


> Creá el código HTML y JavaScript que acabamos de describir.
