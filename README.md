# Modelo de Segmentación  de Clientes
## Contexto
Este repositorio presenta un proyecto como solución a un reto técnico para un vacante de Data Scientist con la siguiente consulta:
1. Análisis estadístico de las variables del Dataset, en donde se pueda evidenciar la distribución de las variables, los problemas de calidad, entre otros temas que consideres relevantes. Para este tema se sugiere entregar un reporte gráfico (idealmente en PowerBI) con el análisis realizado.
2. Desarrollar un proceso de Segmentación (haciendo uso de Python o alguna herramienta analítica) en donde el elemento a segmentar son cada uno de los clientes, en donde se evidencie:
    - Algoritmos probados
    - Método para determinar número óptimo de segmentos
    - Caracterización de los segmentos resultantes
    - Métricas de calidad de los segmentos resultantes

El [archivo adjunto](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/tablas/PruebaTecnica.xlsx) contiene 2 hojas:
  - Clientes: Contienen las variables relacionadas con los clientes objeto de segmentación
  - Transacciones: Contienen las variables transaccionales que deben ser integradas con la información de los clientes.

## Herramientas Utilizadas
- Visual Studio Code (IDE)
- Python (Lenguaje)
- Pandas, NumPy, missingno, warnings, Matplotlib, Seaborn, Scikit-learn (librerías)
- Jupyter (Notebook)
- Power BI (Dashboard)
- Git y Github (Repositorio)
- Trello (Tasks Managment)

## Desarrollo 

Para el desarrollo de este reto técnico se analizó la consulta y la conclusión es que se trata de un problema de aprendizaje no supervisado. Teniendo en cuenta esto, se ha realizado un [análisis exploratorio de datos](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/EDA.ipynb) (EDA) con el siguiente proceso:
  - Cargar el [archivo](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/tablas/PruebaTecnica.xlsx) con los datos que se analizarán utilizando Pandas
  - Verificar la calidad de los datos y evidenciar la distribución de las variables con el apoyo de gráficos intuitivos
  - Clasificar las variables que se analizarán en el feature engineering
  - Guardar las tablas resultantes del proceso las cuales será utilizadas en la implementación del modelo de ML
> En el archivo [EDA](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/EDA.ipynb) se puede evidenciar este proceso paso a paso y con mayor detalle

Luego, usando las tablas de [clientes](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/tablas/tabla_clientes_limpia.csv) y [transacciones](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/tablas/tabla_transacciones_limpia.csv) **limpias**, se redactó un [archivo](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/Modelo_ML.ipynb) en el que se han implementado 2 modelos de ML descritos a continuación:
- Algoritmo de análisis de componentes principales (PCA) + K-means
- Algoritmo de análisis de componentes principales (PCA) + Agglomerative Hierarchical Clustering

El proceso de dicha implementación fué el siguiente:
  - Cargar, validar y unir los datos
  - Implementar algoritmos y evaluar su distribución
  - Usar métricas para calcular la efectividad de los algoritmos
  - Decantar por el uso de (PCA) + K-means
  - Analizar y graficar la distribución de cada variable con respecto a los cluster resultantes
  - Definir un perfil con las características de los cluster resultantes
  - Crear una tabla con la descripción de cada cluster
  - Guardar las tablas resultantes
> En el archivo [Modelo_ML](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/Modelo_ML.ipynb) se puede evidenciar este proceso paso a paso y con mayor detalle

Por último, se ha elaborado un [dashboard interactivo](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/Dashboard_Clientes_Segmentados.pbix) en Power BI utilizando los datos de la [tabla resultante del modelo](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/tablas/tabala_modelo_ML.csv) y la [descripción de cada cluster](https://github.com/Arevalojj2020/Reto_Tecnico_Stradata/blob/main/tablas/tabla_descripcion_cluster.csv).

Este dashboard contiene la cantidad de registros analizados y clasifica a los clientes de la siguiente manera:
- Pefil de cluster
- Rango etario
- Estado
- Riesgo de ocupación

## Contribución 
Se agradece cualquier contribución al proyecto. Si desea colaborar, siga los siguientes pasos:
- Realice un fork del repositorio.
- Cree una rama para su nueva funcionalidad o corrección de errores.
- Realice los cambios necesarios y documente apropiadamente.
- Envíe una pull request para revisar los cambios propuestos.

## Contacto
- [LinkedIn](https://www.linkedin.com/in/juan-jos%C3%A9-ar%C3%A9valo-camargo/)
- Gmail: juanjoarevalo57@gmail.com
- [Portfolio](https://juanjoarevalo57.wixsite.com/juan-ar-valo)
- [Schedule a meeting🎯](https://calendly.com/juanjoarevalo57/entrevista-laboral?month=2023-06)
- Discord: .juanarevalo
- [Kaggle](https://www.kaggle.com/juanarvalo)
