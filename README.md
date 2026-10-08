# Multi-Agent Travel Recommender

Multi-Agent Travel Recommender es un proyecto académico desarrollado en Google Colab para la asignatura de Big Data de la UJI.

El objetivo del proyecto es analizar un conjunto de datos de viajes mediante Pandas y utilizar dos agentes con responsabilidades diferenciadas para procesar la información y generar recomendaciones de itinerarios.

## Descripción general

El proyecto aplica una arquitectura multiagente sencilla en la que cada agente se encarga de una parte concreta del proceso.

La idea principal es separar responsabilidades para que el análisis de datos y la generación de recomendaciones no dependan de un único componente.

El flujo general es:

```text
Dataset de viajes
        ↓
Procesamiento con Pandas
        ↓
Agente de análisis
        ↓
Información estructurada
        ↓
Agente de recomendación
        ↓
Itinerario recomendado
```

## Arquitectura multiagente

El sistema utiliza dos agentes especializados.

### Agente de análisis

El primer agente se encarga de trabajar con los datos disponibles y obtener información relevante a partir del DataFrame.

Entre sus responsabilidades se encuentran:

- analizar los datos del conjunto de viajes;
- filtrar información relevante;
- consultar características de destinos;
- estructurar los resultados para que puedan ser utilizados posteriormente;
- proporcionar información basada en los datos disponibles.

### Agente de recomendación

El segundo agente utiliza la información obtenida durante la fase de análisis para construir una recomendación de viaje.

Entre sus responsabilidades se encuentran:

- interpretar los resultados del análisis;
- evaluar las opciones disponibles;
- seleccionar alternativas adecuadas;
- generar una propuesta de itinerario;
- presentar la recomendación de forma comprensible para el usuario.

La separación entre ambos agentes permite dividir el problema en tareas más pequeñas y asignar una responsabilidad concreta a cada componente.

## Procesamiento de datos

El proyecto utiliza Pandas para trabajar con el conjunto de datos.

Entre las operaciones realizadas se encuentran tareas como:

- carga de datos;
- exploración del DataFrame;
- selección y filtrado de información;
- consulta de atributos;
- preparación de datos para los agentes.

El DataFrame funciona como la principal fuente estructurada de información utilizada durante el proceso de recomendación.

## Tecnologías

- Python
- Pandas
- Google Colab
- Data Analysis
- LLM Agents
- Arquitectura multiagente

## Objetivos del proyecto

Este proyecto me ha permitido trabajar conceptos relacionados con:

- análisis de datos con Pandas;
- procesamiento de información estructurada;
- separación de responsabilidades entre agentes;
- diseño de flujos multiagente;
- interacción entre análisis de datos y modelos de lenguaje;
- generación de recomendaciones a partir de datos.

## Entorno de desarrollo

El proyecto fue desarrollado inicialmente en Google Colab.

El notebook principal contiene:

- preparación y carga de datos;
- análisis del DataFrame;
- definición de los agentes;
- lógica de coordinación entre agentes;
- generación de recomendaciones;
- ejemplos de ejecución.

## Estructura del repositorio

```text
multi-agent-travel-recommender/
│
├── README.md
│
├── notebook/
│   └── travel_recommender.ipynb
│
├── images/
│   ├── architecture.png
│   └── example-output.png
│
└── data/
    └── sample_travel_data.csv
```

La estructura puede evolucionar según se añadan nuevos ejemplos, diagramas o documentación.

## Posibles mejoras

Entre las posibles extensiones del proyecto se encuentran:

- mejorar la coordinación entre agentes;
- incorporar nuevas fuentes de datos;
- añadir más criterios de recomendación;
- permitir preferencias personalizadas del usuario;
- evaluar la calidad de las recomendaciones;
- incorporar memoria o contexto entre interacciones;
- separar la lógica del notebook en módulos reutilizables;
- desarrollar una interfaz sencilla para interactuar con el sistema.

## Contexto académico

Este proyecto fue desarrollado como práctica de la asignatura de Big Data de la Universitat Jaume I.

El objetivo principal fue experimentar con análisis de datos y arquitecturas basadas en agentes, aplicando estos conceptos a un problema práctico de recomendación de viajes.

## Estado

Proyecto académico funcional desarrollado en Google Colab.

El repositorio se utiliza como parte de mi portfolio profesional para mostrar experiencia con Python, Pandas, análisis de datos y sistemas multiagente.
