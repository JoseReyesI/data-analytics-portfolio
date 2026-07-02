# Análisis de ConnectaTel

## Descripción del proyecto

Este proyecto analiza el comportamiento de clientes de ConnectaTel, una empresa de telecomunicaciones con operaciones en México y Colombia.

El objetivo es identificar patrones de uso de llamadas y mensajes, detectar comportamientos atípicos, segmentar clientes y proponer recomendaciones para mejorar los planes ofrecidos.

## Objetivos

- Explorar y limpiar los datasets disponibles.
- Detectar valores faltantes, sentinels y fechas inválidas.
- Analizar el uso de llamadas, mensajes y minutos por cliente.
- Identificar outliers mediante histogramas, boxplots y el método IQR.
- Segmentar clientes por edad y nivel de uso.
- Generar insights y recomendaciones comerciales.

## Datasets utilizados

- `plans.csv`: catálogo de planes, precios, beneficios y costos extra.
- `users_latam.csv`: información de usuarios, edad, ciudad, fecha de registro, plan y churn.
- `usage.csv`: registros de llamadas, mensajes, duración y longitud de mensajes.

## Herramientas utilizadas

- Python
- pandas
- seaborn
- matplotlib
- Jupyter Notebook

## Etapas del análisis

1. Carga y exploración inicial de los datasets.
2. Identificación de valores nulos, sentinels y fechas fuera de rango.
3. Limpieza básica de datos.
4. Creación de métricas de uso por usuario.
5. Estadísticas descriptivas.
6. Visualización de distribuciones.
7. Detección de outliers con boxplots e IQR.
8. Segmentación de clientes por edad y nivel de uso.
9. Elaboración de insights ejecutivos y recomendaciones.

## Hallazgos principales

- La mayoría de los clientes pertenece al grupo de uso medio.
- El grupo de edad predominante es el de adultos entre 30 y 59 años.
- Se detectaron outliers superiores en mensajes, llamadas y especialmente en minutos de llamada.
- Los usuarios de alto uso representan una oportunidad para campañas de upselling o migración a planes Premium.
- Los usuarios de bajo uso pueden beneficiarse de planes más económicos, descuentos o campañas de activación.
- Se identificaron problemas de calidad como ciudades faltantes o registradas como `?`, edades con el valor sentinel `-999` y fechas de registro fuera del periodo de análisis.

## Estructura del proyecto

```text
connectatel/
│
├── README.md
└── S7 Version-Estudiante-Project-ConnectaTel.ipynb
