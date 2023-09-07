# Ejercicio 1
---
Eres el propietario de un parking y necesitas crear un sistema capaz de calcular el precio de la estancia de un vehículo en el parking. Para ello, el sistema debe ser capaz de a partir de la hora de entrada y salida de un vehículo, calcular el precio de la estancia. El precio de la estancia se calcula de la siguiente manera:

- Existe un precio base por hora de 4€, si un usuario sobrepasa por 1 minuto, se le cobrará la hora entera.
- A razón de la hora y minutos de entrada/salida se calculará el precio total.
- No se tendrá en cuenta el día de la semana, ni el mes, ni el año.
- No se tendrá en cuenta que el usuario introduzca una hora de salida anterior a la de entrada.
- No se tendrá en cuenta que el usuario introduzca una hora de entrada/salida que no existe (Ej: 25:00:00).
- No se tendrá en cuenta que el usuario introduzca una hora de entrada/salida con un formato incorrecto (Ej: 25:00:00).
- Los parámetros de entrada siempre serán números enteros.
  - En el caso de las horas se tratará de un número entero entre 0 y 23.
  - En el caso de los minutos se tratará de un número entero entre 0 y 59.

## Ejemplo
```js
function calcularPrecio(horaEntrada, minutoEntrada, horaSalida, minutoSalida) {
  // ...
}

calcularPrecio(10, 0, 11, 0); // 4€
calcularPrecio(10, 0, 11, 1); // 8€
calcularPrecio(10, 0, 11, 59); // 8€
calcularPrecio(10, 0, 12, 0); // 8€
calcularPrecio(10, 0, 12, 1); // 12€
calcularPrecio(10, 0, 10, 0); // 0€
```

## Tips
- Puedes usar la función `Math.ceil()` para redondear un número hacia arriba.
- Puedes usar la función `Math.floor()` para redondear un número hacia abajo.
- Una hora tiene 60 minutos.