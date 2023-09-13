# Proyecto Individual 2 - Análisis de Datos de Siniestros Viales en la Ciudad de Buenos Aires

¡Bienvenido al proyecto de análisis de datos de siniestros viales en la ciudad de Buenos Aires! 
Este proyecto tiene el objetivo de descubrir insights y proponer sugerencias para su mitigación.

## Problemática
Buenos Aires, al igual que muchas capitales del mundo, enfrenta una gran problemática de siniestros viales. Estos siniestros son una prioridad para las autoridades, quienes han tomado diversas medidas para su reducción. Una de estas medidas ha sido el registro de datos generados por los siniestros, lo cual brinda la oportunidad de analizarlos y obtener hallazgos significativos.

## Desarrollo del Proyecto

Durante el desarrollo del proyecto, se han generado los siguientes archivos:

1. Datasets: Se disponen de varios archivos CSV para su análisis en el proyecto. Estos archivos incluyen información sobre homicidios, lesiones, víctimas de homicidios y víctimas de lesiones. Estos datasets han sido procesados mediante un proceso ETL (Extract, Transform, Load) y serán utilizados en el EDA (Exploratory Data Analysis) y en Power BI.

2. ETL: En este archivo en Python, se han realizado transformaciones y limpieza de los datos para que sean más manejables durante el análisis. Algunas de las acciones realizadas incluyen:

- Eliminación de columnas redundantes, como año, mes y día.
- Limpieza de datos en columnas con valores diferentes, como "SD", ".", etc.
- Cambio de tipos de datos para facilitar su manipulación.
- Renombrar columnas para que tengan nombres homogéneos entre los archivos.
- Agregar una columna de gravedad al dataset de homicidios para distinguirlo del dataset de lesiones.
- Agregar una columna de rango etario en lugar de la columna de edad.
- Reemplazo de valores faltantes y atípicos con NaN.
- Cambio de formato de fechas para su correcto procesamiento.

3. EDA: Se han realizado visualizaciones y tablas para explorar los datos en detalle. Algunas de las acciones realizadas incluyen:

Creación de tablas para analizar información relacionada con el lugar de los accidentes, el vehículo involucrado, el número de víctimas y otros aspectos relacionados con las fechas.
Análisis de datos de víctimas para entender características como edad, sexo, vehículo de la víctima, entre otros.

4. Dashboard en Power BI:
El dashboard en Power BI consta de varias páginas que muestran información relevante sobre los siniestros viales y las víctimas. Veamos en detalle cada una de estas páginas:

- Página de Hechos: Esta página muestra cómo ocurren los siniestros viales, ya sea accidentes fatales, con lesiones graves o lesiones leves. Aquí se puede identificar la comuna donde son más frecuentes los siniestros, los años, meses y horas en los que ocurren con mayor frecuencia. Esta información es especialmente útil para que el gobierno de Buenos Aires pueda implementar medidas preventivas y correctivas para reducir el número de siniestros.

- Página de Víctimas: En esta página se muestra el perfil de las víctimas tanto de accidentes fatales como de lesiones. Se observa que con mayor frecuencia, las víctimas son de sexo masculino, con edades comprendidas entre 19 y 39 años. Además, se identifica que muchas de las víctimas son conductores de motocicletas y peatones. Conocer el perfil de las víctimas ayuda a enfocar los esfuerzos para reducir la cantidad de víctimas y siniestros.

- Página de KPI: En esta página se presentan los KPI (Key Performance Indicators) que permiten evaluar las acciones tomadas por el gobierno para disminuir los siniestros y la cantidad de víctimas. Los KPIs incluyen:

Tasa de Homicidios: Este KPI mide la variación de la tasa de homicidios en los últimos 6 meses. Es importante para evaluar si las acciones implementadas han contribuido a reducir la tasa de homicidios en los siniestros viales.

Accidentes Mortales de Motociclistas: Este KPI mide la cantidad de accidentes mortales en los que las víctimas conducían motocicletas. Es relevante porque la mayoría de las víctimas mortales son personas que conducen este tipo de vehículo.

Víctimas Peatones Fallecidos y Gravemente Heridos: Estos KPIs miden la cantidad de peatones que fallecen y quedan gravemente heridos como resultado de los accidentes. Es importante porque las medidas tomadas deben incluir la concientización de los peatones sobre la cantidad de muertes, ya que la mayoría de la población actúa como peatón en algún momento de su vida.

El dashboard en Power BI brinda una visión clara y concisa de la problemática de los siniestros viales y permite tomar acciones basadas en datos para reducir su incidencia y proteger a las víctimas.

## Autora ✒️
* **Berenisse de la Cruz**  - [bere44](https://github.com/bere44/)