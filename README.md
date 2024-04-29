# **Siniestros viales: Introducción** 

Los siniestros viales son eventos que ocurren en las vías públicas e involucran vehículos, pudiendo resultar en daños materiales, lesiones o incluso pérdidas de vidas. En Buenos Aires, una ciudad con un alto volumen de tráfico y una densa población, estos incidentes representan una preocupación significativa para la seguridad pública y la calidad de vida de sus habitantes.

Este repositorio proporciona datos y análisis sobre los siniestros viales en Buenos Aires, con el objetivo de comprender mejor este fenómeno y explorar medidas efectivas para reducir su incidencia y mitigar sus consecuencias.


### Datos

Para este proyecto se utilizaron datos de [Buenos Aires Data](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales), que abarcan información desde 2016 hasta 2021, información sobre las víctimas, los hechos, entre otros:

 * **HECHOS**: contiene filas del hecho ocurrido con identificador único y las variables temporales, espaciales y participantes asociadas al mismo.

 * **VICTIMAS**: contiene filsa por cada víctima y las variables edad, sexo y modo de desplazamiento asociadas a cada víctima. Se vincula a los HECHOS mediante el id del hecho.
 * [**Diccionario de datos**](https://docs.google.com/spreadsheets/d/1Op98U-Hh2a3Q7uuznAzdl4Bf8r8qPr4m/edit#gid=1771770012)

## Análisis Exploratorio de Datos (EDA)

El primer paso que se realizó fue la de extraer los datos del archivo:
1. **HECHOS**: Tabla de datos de los homicidios por siniestros viales en la Ciudad Autónoma de Buenos Aires.
2. **VICTIMAS**: Tabla de datos de las víctimas involucradas en los homicidios por siniestros viales.

Una vez hecho ésto, se analizó la información general de los datos, tanto como cantidad de registros, valores faltantes, cantidad de variables y duplicados.

### Análisis de los datos
Se ha notado una disminución constante desde 2018, con un mínimo notable en 2020 debido a la cuarentena estricta por la pandemia de COVID-19. A pesar de ello, se ha detectado un aumento notable de siniestros a partir de diciembre, atribuido a una flexibilización de las restricciones por las festividades.

Posteriormente, se ha analizado la distribución de víctimas según los días de la semana, identificando que los lunes y los fines de semana registran los números más altos. Esto se explica por el inicio de la semana laboral los lunes, que aumenta el tráfico, y los fines de semana, cuando las personas tienden a salir y reunirse, aumentando así la movilidad y el tráfico.

Se ha examinado la distribución horaria de los accidentes, notándose un aumento marcado alrededor de las 6 de la mañana. Durante los fines de semana, este aumento se relaciona con la salida a boliches y fiestas, aumentando las posibilidades de accidentes debido a conductores ebrios.

Se ha observado que la mayoría de las víctimas son hombres, principalmente entre los 20 y 40 años, siendo las motocicletas y los peatones los más afectados. Las motocicletas son vulnerables en la carretera, y los peatones pueden ser afectados por el comportamiento imprudente de algunos conductores.

Esta concentración de accidentes en el grupo de edad de 20 a 40 años puede ser ocasionada por encontrarse entre las personas que van a trabajar o aquellas que salen a reuniones o fiestas con mayor frecuencia en el caso de los más jovenes. Este análisis destaca la necesidad de medidas preventivas y una mayor conciencia pública para mejorar la seguridad vial.

## **Visualización**
Se utliza la herramienta Power BI para desarrollar una dashboard interactivo para analizar los datos de manera más dinámica.

## **KPIs**

Para este análisis se propuso crear 3 KPIs (Indicadores Claves de Rendimiento):

1. ***Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior***.

    > *Definimos a la tasa de homicidios en siniestros viales como el número de víctimas fatales en accidentes de tránsito por cada 100.000 habitantes en un área geográfica durante un período de tiempo específico. Su fórmula es:* <center>
$\frac{\text{Número de homicidios en siniestros viales}}{\text{Población total}} * 100000$<br><br>
</center >

2. ***Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior***.

    > *Definimos a la cantidad de accidentes mortales de motociclistas en siniestros viales como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal. Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es:*<center>
$\frac{\text{Víctimas en moto del año anterior - Víctimas en moto del año actual}}{\text{Víctimas en moto del año anterior}}*100$<br>
<br></center>
