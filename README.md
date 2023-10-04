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
