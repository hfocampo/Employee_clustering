#              SEGMENTACIÓN DE EMPLEADOS USANDO CLUSTERING


<p align="center">
  <img src="images/kmeansclustering.PNG" width="600" alt="Texto alternativo si la imagen no carga">
</p>


En el proyecto sobre rotación de empleados 'Empoyee_rotation' que pueden ver en el repositorio de GitHub [Portafolio](https://github.com/hfocampo/Employee_turnover.git) usamos los algoritmos de aprendizaje supervisado Logistic Regression y KNeighbors o de vecinos más cercanos, para  predecir qué empleados tendrían probabilidad de retirarse e la empresa, basados en información relevante de talento humano de la misma.

Ahora bien, sabiendo qué empleados son proclives a retirarse, el reto es entender qué los podría estar motivando a dejar la empresa; y en este sentido necesitamos encontrar elementos diferenciadores que nos permitan tener algún nivel de certeza o por lo menos que nos permita auscultar en profundidad los motivadores del abandono; podemos hacer entonces una segmentación de empleados que de forma manual es tediosa y seguramenta no tendríamos los mejores resultados esperados, toda vez que contamos con al rededor de 28 variables a analizar y correlacionar y una base de datos de empleados, por lo general, inmensa. 

Machine Learning nos ofrece para estos análisis herramientas que se denominan Algoritmos de Aprendizaje no Supervisado; y son No Supervisados porque trabajan con conjuntos de datos que no tienen etiquetas o respuestas conocidas asociadas a las observaciones. En otras palabras, no hay un "supervisor" que guíe el proceso de aprendizaje proporcionando las respuestas correctas a cada entrada. Además, en el aprendizaje no supervisado, el objetivo principal es encontrar patrones, estructuras o relaciones intrínsecas en los datos sin tener en cuenta ninguna variable objetivo. Los algoritmos de aprendizaje no supervisado exploran la estructura subyacente del conjunto de datos para descubrir información útil sin ninguna guía externa sobre lo que deberían ser los resultados.


## K-MEANS

El objetivo principal de K-means es agrupar un conjunto de datos en K grupos o clústeres basados en la similitud de las características de las observaciones, en vista de que la elección del número K de clústeres es un hiperparámetro crítico en el algoritmo K-means y puede afectar significativamente la calidad de los resultados, es muy importante conocer este valor; para esto se usa la métrica Elbow (codo) que se utiliza en el análisis de clustering para determinar el número óptimo de clústeres (K) en un conjunto de datos. 



<p align="center">
  <img src="images/cluster_result.PNG" width="1000" alt="Texto alternativo si la imagen no carga">
</p>


Para el proyecto que estamos trabajando, aplicamos el algoritmo K-means y la métrica Elbow obteniendo los siguientes resultados:

- K óptimo para clustering = 5
- De los 5 cluster, el cluster 4 tiene 23 empleados
- El cluster 4 tiene el 100% de los empleados que resultaron con alguna probabilidad de abandonar la compañía



#                  ANÁLISIS DE CLUSTERS PARA ENTENDER LA POSIBLE ROTACION DE EMPLEADOS


<p align="center">
  <img src="images/salary_environment_satisfaction.PNG" width="1000" alt="Texto alternativo si la imagen no carga">
</p>



En la primera gráfica vemos que los empleados del cluster 4 fueron los que recibieron menos aumento aumento de salario promedio 'Percent Salary Hike' y la gráfica2 muestra también un volumen alto de trabajadores con Envieronment Satisfaction baja.



<p align="center">
  <img src="images/training_age.PNG" width="1000" alt="Texto alternativo si la imagen no carga">
</p>



Por otro lado podemos observar que el grupo del cluster 4 son los que han recibido menos entrenamiento el último año 'Training Times Last Year' y también los del cluster 4 son los empleados promedio con grupo de edad entre 32 y 42 años, que seguramente les importa el desarrollo profesional y desean buscar otras alternativas laboralas con mejores condiciones o mayores retos.



<p align="center">
  <img src="images/education.PNG" width="1000" alt="Texto alternativo si la imagen no carga">
</p>



Y a nivel educativo, el 87% de los empleados del cluster 4 con probabilidad de abandonar la empresa, son del nivel educativo 3 y 4, con estudios de 'Bachelor' y 'Master'.




# CONCLUSIONES

- Pueden resultar muchos más análisis productos de la segmentación realizada, el análisis estadístico de los datos y las correlaciones de variables, pero lo más importante es el análisis de sensibilidad de la información dura y matemática con el conocimiento y aportes de los encargados de recursos humanos en la empresa.

- Se recomienda tambien incluir otras variables al modelo  que permitan manejar otros escenarios de análisis.


## Contacto
- Héctor Ocampo Gaviria
- [Portafolio](https://github.com/hfocampo/PI2_Siniestros_Viales.git)
- [hector.ocampog@gmail.com]
