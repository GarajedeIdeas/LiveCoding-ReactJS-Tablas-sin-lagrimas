# ReactJS Tablas sin lágrimas

Evento [Garaje Live Coding](https://livecoding.garajedeideas.com/) con [Gerardo Fernández](https://www.linkedin.com/in/gerardofernandezmoreno).

## React Table

La principal característica de **React Table** radica en ser una "headless utility", lo que significa que no representa ni proporciona ningún componente para construir la UI de nuestras tablas. Por tanto, es nuestra responsabilidad usar el estado y los callbacks de sus hooks para generar la vista de la tabla.

Frente a otras librerías como Material Table, React Table favorece:

- La **separación de conceptos**. El diseño de las tablas y la experiencia que tiene el usuario interactuando con ellas es lo marca la diferencia en una aplicación. React Table se encarga de abstraer la lógica y delega en nosotros todo lo referente al diseño.

- **Mantenimiento**. Eliminar toda la API referente a la interfaz gráfica permite a React Table ser una librería ligera, fácil de usar y simple de mantener y actualizar.

- **Extensibilidad**. React Table empodera al desarrollador para diseñar e implementar cualquier caso de uso y añadir funcionalidad a las tablas conforme el producto evoluciona. Su sistema de plugins facilita enormemente esta tarea, adaptándose a los distintos casos de uso.

### Documentación de React Table

Puedes leer más sobre React Table en la siguiente documentación:

https://react-table.tanstack.com/

## Grabación

Puedes ver la grabación completa del evento [en este enlace](https://www.youtube.com/watch?v=a0Zwk2cTsew)

## Código de ejemplo

### Ejemplo básico

Este ejemplo presenta el código básico para construir una tabla empleando React Table.

https://codesandbox.io/s/react-table-1-hu6hp

### Agrupando columnas

React Table simplifica enormemente la construcción de tablas con columnas agrupadas y footers que agregan información como puedes ver en el siguiente ejemplo:

https://codesandbox.io/s/react-table-2-r5qc0

### Filtros y ordenación

Gracias al sistema de plugins de **React Table**, filtrar una tabla u ordenarla según los valores en una columna resulta muy sencillo:

https://codesandbox.io/s/react-table-3-f8cl0

### Paginación y tablas asíncronas

Si los datos de tu tabla proceden de una API, React Table permite también controlar la paginación y recuperar los nuevos registros a medida que el usuario navega por las distintas páginas.

https://codesandbox.io/s/react-table-4-4xpzx

### Seleccionar filas

React Table proporciona un plugin para implementar la selección de filas, lo cual nos permitirá implementar casos de uso como la exportación o borrado masivo.

https://codesandbox.io/s/react-table-select-x471lt

### useDeferredValue

Aunque no sea específico de React Table, la llegada de React 18 ha abierto la puerta a optimizaciones a nivel de rendimiento. El nuevo hook `useDeferredValue` nos permite añadir un cierto "delay" a un valor de modo que podamos evitar la renderización de componentes pesados hasta que sea estrictamente necesario.

En el siguiente ejemplo puedes alternar entre pasar el valor `defPageIndex` y `pageIndex` al componente `MemoFooter` para ver la diferencia.

https://codesandbox.io/s/react-table-5-deferred-jbygdz

## Gracias

Ahora sí, ya puedes construir tablas sin lágrimas con React.

Muchas gracias al equipo de Garaje de Ideas por fomentar este tipo de directos y ayudar a enriquecer la comunidad.

💛 Gerardo Fernández. Latte and Code.
