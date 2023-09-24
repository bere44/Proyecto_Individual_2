<p align=center><img src=https://raw.githubusercontent.com/bere44/Proyecto_Individual_2/master/src/vial.jpg><p>


<h1 align="center"> Proyecto Individual 2 </h1>

#  Análisis de Datos de Siniestros Viales en la Ciudad de Buenos Aires


¡Bienvenido al proyecto de análisis de datos de siniestros viales en la ciudad de Buenos Aires! 
Este proyecto tiene el objetivo de descubrir insights y proponer sugerencias para su mitigación.


## Problemática
Buenos Aires, al igual que muchas capitales del mundo, enfrenta una gran problemática de siniestros viales. Estos siniestros son una prioridad para las autoridades, quienes han tomado diversas medidas para su reducción. Una de estas medidas ha sido el registro de datos generados por los siniestros, lo cual brinda la oportunidad de analizarlos y obtener hallazgos significativos.


## Estructura del Repositorio 

-   **Archivos csv**: Son los archivos donde estan en el archivo los dataset reducidos para hacer las transformaciones de los datos.

-   **.gitignore**: Archivo que especifica los archivos y directorios que deben ser ignorados por Git.

-   **ETL**: Archivo en donde ser hace la carga de datos y algunas transformaciones.

-   **EDA.ipynb**: Archivo Jupyter Notebook que contiene el análisis exploratorio de datos.

-   **src**: Carpeta que contiene archivos fuente del proyecto.


## Desarrollo del Proyecto

Durante el desarrollo del proyecto, se han generado los siguientes archivos:

1. **Datasets**: Se disponen de varios archivos CSV para su análisis en el proyecto. Estos archivos incluyen información sobre homicidios, lesiones, víctimas de homicidios y víctimas de lesiones. Estos datasets han sido procesados mediante un proceso ETL (Extract, Transform, Load) y serán utilizados en el EDA (Exploratory Data Analysis) y en Power BI.

2. **ETL**: En este archivo en Python, se han realizado transformaciones y limpieza de los datos para que sean más manejables durante el análisis. Algunas de las   acciones realizadas incluyen:

- Eliminación de columnas redundantes, como año, mes y día.
- Limpieza de datos en columnas con valores diferentes, como "SD", ".", etc.
- Cambio de tipos de datos para facilitar su manipulación.
- Renombrar columnas para que tengan nombres homogéneos entre los archivos.
- Agregar una columna de gravedad al dataset de homicidios para distinguirlo del dataset de lesiones.
- Agregar una columna de rango etario en lugar de la columna de edad.
- Reemplazo de valores faltantes y atípicos con NaN.
- Cambio de formato de fechas para su correcto procesamiento.

3. **EDA**: Se han realizado visualizaciones y tablas para explorar los datos en detalle. Algunas de las acciones realizadas incluyen:

  Creación de tablas para analizar información relacionada con el lugar de los accidentes, el vehículo involucrado, el número de víctimas y otros aspectos relacionados con las fechas.
  Análisis de datos de víctimas para entender características como edad, sexo, vehículo de la víctima, entre otros.

4. **Dashboard en Power BI**:
  El dashboard en Power BI consta de varias páginas que muestran información relevante sobre los siniestros viales y las víctimas. Veamos en detalle cada una de     estas páginas:
  
  - Página de Hechos: Esta página muestra cómo ocurren los siniestros viales, ya sea accidentes fatales, con lesiones graves o lesiones leves. Aquí se puede identificar la comuna donde son más frecuentes los siniestros, los años, meses y horas en los que ocurren con mayor frecuencia. Esta información es especialmente útil para que el gobierno de Buenos Aires pueda implementar medidas preventivas y correctivas para reducir el número de siniestros.
  
  - Página de Víctimas: En esta página se muestra el perfil de las víctimas tanto de accidentes fatales como de lesiones. Se observa que con mayor frecuencia, las víctimas son de sexo masculino, con edades comprendidas entre 19 y 39 años. Además, se identifica que muchas de las víctimas son conductores de motocicletas y peatones. Conocer el perfil de las víctimas ayuda a enfocar los esfuerzos para reducir la cantidad de víctimas y siniestros.
  
  - Página de KPI: En esta página se presentan los KPI (Key Performance Indicators) que permiten evaluar las acciones tomadas por el gobierno para disminuir los siniestros y la cantidad de víctimas. Los KPIs incluyen:
  
  **Tasa de Homicidios**: 
  + KPI1: Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior
    
    + Se define como el número total de víctimas fatales que hay en dataset por cada 100,000 un área geográfica durante un período de tiempo específico
    + Este KPI mide la variación de la tasa de homicidios en los últimos 6 meses. Es importante para evaluar si las acciones implementadas han contribuido a reducir la tasa de homicidios en los siniestros viales.
  
  **Accidentes Mortales de Motociclistas**: 
  + KP12: Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.
    
    + Se define como el numero de accidentes fatales con víctimas que viajaban en moto en un determinado periodo temporal. Su fórmula para medir la evolución: (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100
    + Este KPI mide la cantidad de accidentes mortales en los que las víctimas conducían motocicletas. Es relevante porque la mayoría de las víctimas mortales son personas que conducen este tipo de vehículo.
  
  **Víctimas Peatones Fallecidos y Gravemente Heridos**: 
  + KPI3: Reducir en un 5% la cantidad de peatones fallecidos en el ultimo año respecto al trimestre anterior, en CABA.
  + KPI4: Reducir en un 15% la cantidad de peatones con heridas graves en el ultimo año respecto al trimestre anterior, en CABA.
    
    + Se definen como el número de accidentes fatales y accidentes con víctimas con hervidas graves que sean peatones en un determinado periodo temporal. Su fórmula para medir la evolución: (Número de accidentes peatones (muertes fatales o heridas graves) en el trimestre anterior - Número de accidentes peatones(muertes fatales o heridas graves) en el trimestre actual) / (Número de accidentes peatones(muertes fatales o heridas graves) en el trimestre anterior) * 100
    + Estos KPIs miden la cantidad de peatones que fallecen y quedan gravemente heridos como resultado de los accidentes. Es importante porque las medidas tomadas deben incluir la concientización de los peatones sobre la cantidad de muertes, ya que la mayoría de la población actúa como peatón en algún momento de su vida.
  
  El dashboard en Power BI brinda una visión clara y concisa de la problemática de los siniestros viales y permite tomar acciones basadas en datos para reducir su incidencia y proteger a las víctimas.

5. **Conclusiones**

La ciudad de Buenos Aires cuenta con plan de gestión de tránsito puede ser complementado con ciertas recomendaciones que a continuación daremos de acuerdo a los hallazgos encontrados en cada una de las páginas del dashboard:

+ Gracias a la página hechos hemos podido llegar a las siguientes conclusiones y recomendaciones:
  + Se tiene que hacer una evaluación de diferentes alternativas de circulación en principales avenidas
  + Se debe hacer uso de carteles con mensajes variables en los semáforos para los conductores de autos; estos mensajes se deben activar solo durante las señales rojas para evitar distracciones
  + Fomentar el transporte público en la ciudad de Buenos Aires
  + Contar con más cantidad de agentes de control de tránsito en hora punta
  + Contar con un carril exclusivo para motos en la medida que esto sea posible
+ En  la página de víctimas vamos a tener las siguientes conclusiones y recomendaciones:
  + Se deben definir pasos peatonales bien establecidos
  + Se debe contar con carteles informativos y preventivos para peatones
  + Se debe verificar el uso de implementos de seguridad en quienes hacen uso de moto



## Autora ✒️
* **Berenisse de la Cruz**  - [Berenisse de la cruz](www.linkedin.com/in/berenisse-de-la-cruz-moreno)
