# Data Engineer Challenge

Se pide resolver los siguientes problemas implementando funciones, usando 2 enfoques por cada problema: Uno en el que se optimice el tiempo de
ejecución, y otro en que se optimice la memoria en uso

## Problemas:
1. Las top 10 fechas donde hay más tweets. Mencionar el usuario (username) que más publicaciones tiene
por cada uno de esos días. Debe incluir las siguientes funciones:
  - def q1_time(file_path: str) -> List[Tuple[datetime.date, str]]:
  - def q1_memory(file_path: str) -> List[Tuple[datetime.date, str]]:

2. Los top 10 emojis más usados con su respectivo conteo. Debe incluir las siguientes funciones:
- def q2_time(file_path: str) -> List[Tuple[str, int]]:
- def q2_memory(file_path: str) -> List[Tuple[str, int]]:

3. El top 10 histórico de usuarios (username) más influyentes en función del conteo de las menciones (@)
que registra cada uno de ellos. Debe incluir las siguientes funciones:
  - def q3_time(file_path: str) -> List[Tuple[str, int]]:
  - def q3_memory(file_path: str) -> List[Tuple[str, int]]:

## Cómo ejecutar el código

Se utilza docker para crear un contenedor donde se pueda correr spark y pyspark en una Jupiter notebook. Para esto se debe descargar docker desde la página oficial del proyecto `https://hub.docker.com/`

Dentro del repositorio se debe correr el siguiente comando `docker run --name pyspark -p 8888:8888 -v ./.:/home/jovyan/work jupyter/pyspark-notebook`
Se creartá una carpeta que se comparte con los contenedores, en la carpeta del repositorio se debe guardar el archivo json con el nombre `farmers-protest-tweets-2021-2-4.json` que se desea procesar

Se podrá acceder al notebook en la siguiente url `http://127.0.0.1:8888/`, dentro de la carpeta work se encontrará la notebook y el archivo json
