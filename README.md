# MineriaMSID
Repositorio para la asignatura de Minería de Datos 2022-2023. En este repositorio se incluye todos los archivos, cuadernos y modelos utilizados y generados para afrontar el reto de Cajamar de Carpooling.

## Reto Cajamar Carpooling
_Presente en España desde enero de 2010, BlaBlaCar es la mayor red social de viajes de larga distancia en coche compartido con más de 85 millones de usuarios en 22 países (5 millones en España). La red social pone en contacto a personas que quieren realizar un trayecto común y coinciden para hacerlo el mismo día._

Precisamente con datos de esta aplicación, con los desplazamientos indexados por día, origen y destino desde el 1 de Diciembre de 2017 hasta el 30 de Noviembre de 2019, pretendemos hacer un estudio y aprovechamiento de estos datos siguiendo el proceso KDD visto en la asignatura de Minería de Datos.

Nuestra propuesta plantea, por un lado, un enfoque similar al de [este estudio](https://www.dataestur.es/wp-content/uploads/Informe-flujos-turisticos-dic-2020.pdf) de Segittur, aplicando los datos de BlaBlaCar.

Otro punto a tratar en nuestro estudio sería realizar un análisis de las emisiones y el impacto de BlaBlaCar sobre estas. Ejemplos de estos análisis pueden ser este estudio de la [misma BlablaCar](https://blog.blablacar.es/blablalife/lp/el-uso-del-coche-compartido-reduce-1-6-millones-de-toneladas-de-co2-al-ano), o incluso [este otro](https://www.pagatelia.com/proyecto-zero-empty-seats) de Pagatelia.

## Datos utilizados
Para llevar a cabo el proyecto, hemos necesitado varios datos de fuentes externas. Estos conjuntos de datos los dejamos adjuntos tanto en la carpeta `data` como en la siguiente [carpeta de Drive](https://drive.google.com/drive/folders/1tJec4CXAwk6y1dFazWxox3RFGj4WL2El?usp=share_link). Algunos de ellos debido a su gran tamaño, solo están disponibles en la carpeta de Drive, estos son: `blablacar_dataset.csv`, `blablacar_ampliado_dataset.csv` y `habitantes_dt.csv`. Los dos primeros se encuentran en `data/Raw` y el último en `data/Processed`
Por otro lado, los modelos creados a partir de nuestros datos se encuentran tanto en la carpeta `models` como en la carpeta de Drive, por la misma razón que anteriormente. En este caso, el modelo de _Random Forest_ solo está disponible en dicha carpeta, en `models`.

## Líneas de Trabajo
Como propuestas de trabajo a realizar con los datos que se nos proporcionan (junto con otros de fuentes externa o generados por nosotros, en la carpeta `data`), hemos llevado a cabo las siguientes líneas:
1. Predicción de **volumen de movilidad de autobuses interurbanos** en base a los trayectos de BlablaCar.
2. Predicción de **emisiones por trayectos de BlaBlaCar** en los dos meses que prosiguen a los datos del dataset original.
3. Sistema de **recomendación de uso de BlaBlaCar** para una serie de fechas dadas como entrada.
4. Predicción de **viajes en poblaciones pequeñas** y cálculo de la probabilidad de dicho viaje (tanto en general como viaje frecuente).

## Metodología
Para el desarrollo de este proyecto, se han realizado diferentes iteraciones de acuerdo al progreso de las prácticas de la asignatura de Minería de Datos. Para ver los informes parciales que se han generado para cada iteración, vea la carpeta `reports`.

## Construido Con
Hemos utilizado para el desarrollo de este proyecto cuadernos de Google Colaboratory, principalmente en un Colab (en la carpeta `notebooks`) que incluye el desarrollo de todas las fases del proceso KDD así como las líneas de trabajo expuestas anteriormente (con las correspondientes explicaciones de cada apartado).

## Referencias
A lo largo del desarrollo de este proyecto, nos hemos apoyado en varias referencias para solventar algunas necesidades. Estas son:
- _Transport-co2_. (2020, May 20). PyPI. https://pypi.org/project/transport-co2/
- _Carbon intensity of crude oil in europe_. (2010). International Council on Clean Transportation and Energy-Redefined LLC. https://theicct.org/sites/default/files/ICCT_crudeoil_Eur_Dec2010_sum.pdf
-  J. A. Rodrigo, J. E. Ortiz_Skforecast. _Forecasting Series Temporales Con Python Y Scikitlearn_. (2021, February). https://www.cienciadedatos.net/documentos/py27-forecasting-series-temporales-python-scikitlearn.html
- Amidon, A. (2020, July 17). _How to Apply K-means Clustering to Time Series Data_. Medium. https://towardsdatascience.com/how-to-apply-k-means-clustering-to-time-series-data-28d04a8f7da3

## Autores
- María Garrido Arcos
- Sergio Jiménez Fernández
- Ismael Pérez Nieves
- David Pinto Camacho
