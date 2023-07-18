# Proyecto Individual 2 - Las Telecomunicaciones en Argentina
![logo](https://neurona-ba.com/wp-content/uploads/2021/07/HenryLogo.jpg)


## Contexto
Estamos habitando un mundo cada vez más interconectado, sin barreras geograficas, donde la comunicacion se convierte en un importante mecanismo de conexion con en el exterior y es necesario que fluya de manera instantánea. En este escenario, las telecomunicaciones desempeñan un papel fundamental, conectando personas, negocios y comunidades en todo el mundo. Hoy, nos enfocaremos en explorar el fascinante panorama de las telecomunicaciones en Argentina, un país donde la conectividad y la transformación digital han experimentado un crecimiento sin precedentes, para lo cual tomamos como referencia la informacion que provee ENACOM sobre el comportamiento y evolucion de las telecomunicaciones en este importante pais de America Latina y explicaré los hallazgos por medio de un dashboard en Power BI

## Objetivos

- Conocer el panorama actual del comportamiento de las telecomunicaciones en Argentina, proporcionando una descripcion clara y detallada sobre aspectos como la cobertura y servicios disponibles

- Analizar como ha sido el crecimiento de las telecomunicaciones a lo largo del tiempo.



- budget	=	El presupuesto de la película, en dólares
- id	=	ID de la pelicula
- original_language	=	Idioma original en la que se grabo la pelicula
- overview	=	Pequeño resumen de la película
- popularity	=	Puntaje de popularidad de la película, asignado por TMDB (TheMoviesDataBase)
- release_date	=	Fecha de estreno de la película
- revenue	=	Recaudación de la pelicula, en dolares
- runtime	=	Duración de la película, en minutos
- spoken_languages	=	Lista con los idiomas que se hablan en la pelicula
- status	=	Estado de la pelicula actual (si fue anunciada, si ya se estreno, etc)
- tagline	=	Frase celebre asociadaa la pelicula
- title	=	Titulo de la pelicula
- vote_average	=	Puntaje promedio de reseñas de la pelicula
- vote_count	=	Numeros de votos recibidos por la pelicula, en TMDB
- name	=	Nombre de la franquicia
- backdrop_path	=	URL de la foto
- genres_name	=	Lista de generos
- countries	=	Lista de paises
- productor	=	Lista de productoras
- directors	=	Lista de directores
- release_year	=	Año de creacion
- return	=	Retorno de la pelicula, obtenido de la division de revenue y budget

## Desarrollo del Proyecto

## 1. ETL

- Algunos campos, como belongs_to_collection, production_companies y otros (ver diccionario de datos) están anidados, esto es o bien tienen un diccionario o una lista como valores en cada fila, ¡deberán desanidarlos para poder y unirlos al dataset de nuevo hacer alguna de las consultas de la API! O bien buscar la manera de acceder a esos datos sin desanidarlos.

- Los valores nulos de los campos revenue, budget deben ser rellenados por el número 0.

- Los valores nulos del campo release date deben eliminarse.

- De haber fechas, deberán tener el formato AAAA-mm-dd, además deberán crear la columna release_year donde extraerán el año de la fecha de estreno.

- Crear la columna con el retorno de inversión, llamada return con los campos revenue y budget, dividiendo estas dos últimas revenue / budget, cuando no hay datos disponibles para calcularlo, deberá tomar el valor 0.

-  Eliminar las columnas que no serán utilizadas, video,imdb_id,adult,original_title,poster_path y homepage


## 2. EDA

Se realiza una exploración de los datos ya transformados con el fin de entenderlos mejor y poderlos usar de la mejor forma para el desarrollo de la API. Incluyendo graficas interesantes para la extracción de los datos.
Nuestro EDA incluye:
-  Vista previa del contenido del dataset

- información general del contenido del dataset (Cantidad y tipos de datos)

- Análisis estadístico variables cuantitativas

- Análisis estadístico variables cualitativas

- Gráfico de barras de la ganancia por año, tomando los valores de revenue más significativos los cuales están entre los años 1973 y 2017

- Gráfico de dispersión entre las variables Revenue, Budget, popularity y return

- Nube de palabras