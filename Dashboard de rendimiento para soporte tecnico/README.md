# Dashboard de rendimiento para soporte técnico

## Contexto

En operaciones de soporte técnico se generan múltiples registros asociados a solicitudes, actividades y requerimientos. Sin una adecuada visualización y seguimiento, puede resultar difícil identificar tendencias, distribución de carga y comportamiento de la operación.

Este proyecto presenta el desarrollo de un dashboard orientado al análisis y visualización de información de soporte técnico.

## Objetivos

A partir de los datos disponibles se plantearon las siguientes preguntas de análisis:

1. ¿Cuál es el volumen total de soportes durante el periodo de análisis?
2. ¿Cómo evoluciona el volumen de soportes a través del tiempo?
3. ¿Cuál es la distribución de los soportes durante la semana?
4. ¿Cómo se distribuyen los soportes entre los responsables?
5. ¿Qué productos concentran la mayor cantidad de soportes?
6. ¿Cómo se distribuyen los soportes según su prioridad?

## Fuente y estructura de datos

Para el desarrollo del proyecto se utilizó una base de datos simulada de seguimiento de soportes.

Con el objetivo de mantener el proyecto libre de información sensible, los datos utilizados fueron anonimizados y adaptados para fines demostrativos.

La estructura de datos contiene las siguientes variables:

- Ticket
- Estatus
- Prioridad
- Fecha
- Agente
- Producto

## Preparación y transformación

Durante la etapa de preparación se realizaron diferentes transformaciones para adecuar los datos al análisis:

- Definición del periodo de análisis.
- Conversión de tipos de datos.
- Normalización de variables categóricas.
- Conversión de la variable Fecha al tipo de dato correspondiente.
- Creación de variables derivadas para facilitar el análisis temporal.

Entre las variables derivadas se encuentran:

- Día
- Mes
- Año
- Mes_Año
- Día de la semana

## Modelado y lógica

<img src="https://github.com/Walle-Chingg-Uparela/Mis-proyectos/blob/main/img/Tabla%20de%20soportes.jpg" alt="Modelo de datos" width="900">


El modelo se estructuró a partir de una tabla principal de registros de soporte.

La variable Fecha se utilizó como base para el análisis temporal, mientras que las variables Agente y Producto permitieron realizar análisis comparativos y de distribución.

A partir del modelo se desarrollaron medidas en DAX para obtener indicadores como:

- Total de soportes
- Promedio de soportes por día
- Promedio de soportes por mes
- Promedio de soportes por agente

## Diseño del tablero

### Wireframe inicial

La propuesta inicial buscó establecer una distribución sencilla que permitiera visualizar los principales indicadores y facilitar la interacción con los datos.

### Primera implementación

Se desarrolló una primera versión funcional del dashboard con los principales indicadores y visualizaciones.

Esta versión permitió validar la estructura, distribución de los elementos y comportamiento de los datos.

### Iteraciones

Durante el desarrollo se realizaron diferentes ajustes relacionados con:

- Distribución de los elementos.
- Organización de las visualizaciones.
- Ordenamiento temporal.
- Interacción entre filtros y gráficos.
- Presentación de indicadores.
- Legibilidad y aprovechamiento del espacio disponible.

### Diseño final

La versión final integra los principales indicadores y visualizaciones en una única interfaz, buscando facilitar la interpretación de los datos y mantener una presentación clara y compacta.

El resultado es un dashboard interactivo orientado a la visualización y análisis de registros de soporte técnico.La solución permite consultar indicadores generales, identificar tendencias y explorar la distribución de los registros mediante diferentes dimensiones de análisis.

<img src="https://github.com/Walle-Chingg-Uparela/Mis-proyectos/blob/main/img/P1.jpg" width="800"/>

## Elementos visuales

### KPIs

Se incorporaron indicadores para mostrar:

- Soportes Totales
- Soportes por mes
- Soportes por día

### Tendencia mensual - Demanda de casos en el tiempo

Gráfico de área utilizado para visualizar la evolución del volumen de soportes a través del tiempo.

### Soportes por día - Promedio de casos en la semana

Gráfico de barras vertical utilizado para analizar la distribución de los soportes durante los diferentes días de la semana.

### Rendimiento de agentes

Gráfico de barras horizontal utilizado para comparar el volumen de soportes asociado a cada responsable.

### Demanda de soportes por producto

Treemap utilizado para identificar los productos con mayor cantidad de registros de soporte.

### Soportes por prioridad

Gráfico circular utilizado para visualizar la distribución de los registros según su nivel de prioridad.

## Interactividad

Se incorporaron filtros para permitir diferentes perspectivas de análisis sobre la información.

Los filtros utilizados permiten segmentar los datos por:

- Fecha
- Mes
- Año
- Agente
- Producto

También se incorporó una opción para restablecer los filtros aplicados.

## Tecnologías utilizadas
- Microsoft Excel
- Power Query
- Microsoft Power BI
- DAX

## Escalabilidad del proyecto a corto y mediano plazo 

### en el corto plazo
- Se pretende ir mejorando las métricas mostradas en el tablero y automatizar la generación y él envió del reporte a cada una de las partes interesadas, mediante Power Automate utilizando un flujo simple para el envio automatico del reporte desde el correo electronico.
### en el mediano plazo 
- Se busca optimizar el registro de los datos desde una plataforma amigable con clientes externos e internos.
