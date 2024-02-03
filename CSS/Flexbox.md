## Flexobox

Flexbox, o Flexible Box Layout, es un modelo de diseño unidimensional que permite crear diseños más flexibles y eficientes en CSS. Con Flexbox, puedes distribuir y alinear elementos de manera automática, lo que simplifica la creación de diseños complejos y responsivos.

### Propiedades

1. `display`: Define el contenedor como un contenedor flex. Esto cambia el diseño del contenedor y sus hijos a un modelo de caja flexible.
   
   - `display: flex;`: Establece el contenedor como un contenedor flex.
   - `display: inline-flex;`: Similar a `flex`, pero el contenedor se muestra como un elemento en línea.

   ```css
   .container {
       display: flex;
   }
   ```

2. `flex-direction`: Define la dirección principal en la que los elementos flexibles se distribuyen dentro del contenedor.
   
   - `flex-direction: row;`: Los elementos se distribuyen en la dirección del flujo del texto.
   - `flex-direction: row-reverse;`: Igual que `row`, pero en orden inverso.
   - `flex-direction: column;`: Los elementos se distribuyen verticalmente de arriba a abajo.
   - `flex-direction: column-reverse;`: Igual que `column`, pero en orden inverso.

   ```css
   .container {
       flex-direction: row;
   }
   ```

3. `justify-content`: Alinea los elementos flexibles a lo largo del eje principal del contenedor.
   
   - `justify-content: flex-start;`: Los elementos se alinean al principio del contenedor.
   - `justify-content: flex-end;`: Los elementos se alinean al final del contenedor.
   - `justify-content: center;`: Los elementos se alinean en el centro del contenedor.
   - `justify-content: space-between;`: Los elementos se distribuyen uniformemente con espacios iguales entre ellos.
   - `justify-content: space-around;`: Los elementos se distribuyen uniformemente con espacios iguales alrededor de ellos.
   - `justify-content: space-evenly;`: Los elementos se distribuyen uniformemente con espacios iguales entre ellos, incluido el espacio antes y después de la primera y última caja.

   ```css
   .container {
       justify-content: center;
   }
   ```

4. `align-items`: Alinea los elementos flexibles a lo largo del eje transversal del contenedor.
   
   - `align-items: stretch;`: Los elementos se estiran para llenar el contenedor.
   - `align-items: flex-start;`: Los elementos se alinean al principio del contenedor.
   - `align-items: flex-end;`: Los elementos se alinean al final del contenedor.
   - `align-items: center;`: Los elementos se alinean en el centro del contenedor.
   - `align-items: baseline;`: Los elementos se alinean a la línea base común.

   ```css
   .container {
       align-items: center;
   }
   ```

5. `flex`: Una propiedad abreviada que establece la flexibilidad de un elemento flexible dentro del contenedor. Tiene tres valores: `flex-grow`, `flex-shrink` y `flex-basis`.
   
   - `flex: 1;`: Equivalente a `flex: 1 1 0;`, los elementos flexibles se expanden para llenar el espacio disponible.
   - `flex: initial;`: Restaura los valores iniciales de `flex-grow`, `flex-shrink` y `flex-basis`.
   - `flex: none;`: Equivalente a `flex: 0 0 auto;`, los elementos no se expanden ni se contraen.

   ```css
   .item {
       flex: 1 1 auto;
   }
   ```

6. `align-self`: Permite anular la alineación predeterminada definida por `align-items` para un solo elemento.
   
   - `align-self: auto;`: Usa el valor predeterminado definido por `align-items`.
   - `align-self: flex-start;`: El elemento se alinea al principio del contenedor.
   - `align-self: flex-end;`: El elemento se alinea al final del contenedor.
   - `align-self: center;`: El elemento se alinea en el centro del contenedor.
   - `align-self: baseline;`: El elemento se alinea a la línea base común.
   - `align-self: stretch;`: El elemento se estira para llenar el contenedor.

   ```css
   .item {
       align-self: center;
   }
   ```

Con estas propiedades, puedes controlar la disposición y el comportamiento de los elementos dentro de un contenedor flex, lo que facilita la creación de diseños flexibles y responsivos en CSS.
