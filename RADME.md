# Proyecto Individual 2 - Las Telecomunicaciones en Argentina
![logo](https://neurona-ba.com/wp-content/uploads/2021/07/HenryLogo.jpg)


## Contexto
Estamos habitando un mundo cada vez más interconectado, sin barreras geograficas, donde la comunicación se convierte en un importante mecanismo de conexión con en el exterior y es necesario que fluya de manera instantánea. En este escenario, las telecomunicaciones desempeñan un papel fundamental, conectando personas, negocios y comunidades en todo el mundo. Hoy, nos enfocaremos en explorar el fascinante panorama de las telecomunicaciones en Argentina, un país donde la conectividad y la transformación digital han experimentado un crecimiento sin precedentes, para lo cual tomamos como referencia la información que provee ENACOM sobre el comportamiento y evolución de las telecomunicaciones en este importante país de América Latina y se explicarán los hallazgos por medio de un dashboard en Power BI

## Objetivos

- Conocer el panorama actual del comportamiento de las telecomunicaciones en Argentina, proporcionando una descripcion clara y detallada sobre aspectos como la cobertura y servicios disponibles

- Analizar como ha sido el crecimiento de las telecomunicaciones a lo largo del tiempo.

## Desarrollo del Proyecto


## 1. EDA

Una vez realizadas las transformaciones necesarias sobre los dataset que se van a usar, se realiza una exploración de los datos con el fin de entenderlos mejor y poderlos usar de la mejor forma en el dashboard de Power BI. Para esto, se usan algunas gráficas que nos muestran información relevante sobre la conectividad en Argentina, tales como:

- Analisis estadístico con la cantidad de variables incluidas en el dataset.
- Histograma, donde se puede observar la distribución de la población.
- un mapa de calor donde se relacionan las variables del dataset
- un gráfico de barras apiladas que muestra la cantidad de poblacion que tiene acceso a las diferentes tecnologías.
- un gráfico de línea que permite ver como ha sido el crecimiento de los accesos por cada 100 hogares por trimestre.
- un gráfico circular que muestra los tipos de tecnologías mas utilizados.

Adicionalmente, en la carpeta PI02 del repositorio se incluyó el EDA automatico que provee la libreria pandas_profiling, como información general, sin embargo, el EDA se realizó de forma manual, debido a que los datos encontrados en los archivos csv no contienen información a profundidad de los temas analizados.

## 2. Dashboard

Para la presentación del dashboard se hace uso de la herramienta Power BI, en donde se cargan los archivos que resultaron de la transformación, los cuales se llaman 'conectividad por provincia' y 'penetración'.

Con este dashboard se hace una descripción general de la cobertura de las telecomunicaciones en Argentina, describiendo el comportamiento de los diferentes servicios que se encuentran disponibles.

Adicionalmente, se presenta la tendencia de crecimiento del acceso a internet por cada 100 hogares de manera trimestral.

Finalmente, como resultado de este analisis se crean los siguientes KPIs, que le permitirán a la compañia mejorar la cobertura de las telecomunicaciones:

 - Porcentaje de cobertura
 - Cobertura por año
 - Indicador de tendencia de crecimiento de Accesos a internet por trimestre
 - Porcentaje de la población con acceso a internet por cada tecnología.

 ## Vista previa del dashboard
![Telecomunicaciones en Argentina](imagenes\Dashboard.JPG)
