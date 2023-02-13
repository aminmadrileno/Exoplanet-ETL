# Exoplanet-ETL

1. extraiendo datos:

en primer lugar he usado el selenium libreria de python para escrapar una tabla de NASA Exoplanet archive.
Esa tabla contenia mas de 5,000 planetas capturadas de NASA. Por eso proyecto solo he concentrado a los 20 mas cercanas de la tierra. 

Despues de eso, he cargado un archivo CSV de kaggle que muestra todas las planetas un nuestra sistema solar y sus atributos que podemos compara con las Exoplanetas descubrido.


Al final, por comparar las estrellas de las Exoplanetas, necesitamos tambien los atributos y datos de nuestra estrella, el sol. Por eso he escrapeado el wikipedia pagina del sol para obtener datos lo que podemos usar para compararlos con las otras estrellas. 


2. Limpizando los datos:
Para limpizar los datos, he cambiado los tipos de datos de las columnas, borrado valores nulos y unificado los tipos de valores en la tabla de las 20 planetas extrañas.

Los proximos Pasos:
- Voy a limpizar los datos de las planetas de nuestra sistema solar y unificarlos, asi que son similar con los atributos de las exoplanetas para hacerlo mas facil por comparar entre ellos.
- Lo mismo hago con la tabla del sol por compararlo con las estrellas de las exoplanetas. 

Cargando datos:
- Los archivos CSV que son convertido desde los DataFrames van a ser convertido otra vez hacia SQL. 
- Ahí, los archivos obtienen primary y secondary keys. 
- Al final los bases de datos van a ser unidado en una base de datos con el metodo de join. 
- El gol es, que la base de datos en fin tiene las exoplanetas, nuestra planetas y nuestra estrella. Tambien columnas que tienen valores de tasas que muestran el comparison entre esos.
