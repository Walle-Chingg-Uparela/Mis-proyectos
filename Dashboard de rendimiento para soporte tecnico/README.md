## Dashboard de rendimiento para soporte técnico

## Contexto

En una oficina de ingeniería se generan diariamente múltiples actividades de soporte técnico. Sin una adecuada visualización y seguimiento, resulta difícil identificar tendencias, distribución de carga y comportamiento de la operación.

## Objetivos

De forma que, se plantean las siguientes preguntas para el debido análisis del volumen de información generado por el proceso de ingeniería.

1. ¿cuántos soportes van en total del año 2026?
2. ¿Como ha evolucionado el volumen de soportes mes a mes?
3. ¿cuál es la concentración de soportes por cada uno de los ingenieros del equipo?
4. ¿a qué productos se les presta mayor cantidad de soportes?
5. ¿Cuál es la distribución de los soportes en la semana?
6. ¿cuál es la distribución según la prioridad del soporte?

## Fuente y estructura de datos

La fuente de datos está basada en la simulación de una base de datos de seguimiento de soportes realizados desde el mes de junio del año 2025, sin embargo, a fin de proteger datos sensibles y de realizar una propuesta de visualización de los datos, la estructura se desarrolla de la siguiente manera.

- Ticket
- Estatus
- Prioridad
- Fecha
- Agente
- Producto

## preparación y transformación

- Dado que la solicitud entre las preguntas especifica hacer el reporte de los soportes realizados únicamente en el año 2026 se hace filtrado por año, descartando aquellos soportes realizados en el año 2025.
- Se hace cambios del tipo de dato en algunas columnas
  - La columna ticket pasa a ser una columna con valores de tipo entero
  - Las columnas de tipo Prioridad, Agente y Producto pasan a ser de tipo texto
  - La columna Fecha pasa a ser tipo Fecha

## Modelado y lógica

## Diseño del tablero
###  Wireframe inicial

### Primera implementación
### Iteraciones
### Diseño final

## Elementos visuales
### KPIs
### Tendencia mensual
### Soportes por agente
### Soportes por día
### Soportes por producto
### Soportes por prioridad

## Interactividad

## Resultado final

## Tecnologías usadas
