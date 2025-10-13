# Documentación

**Integrante**: Andrés Hernández

## Realización del proceso de visualización:

## **Paso 1**

En primer lugar, consideré los datos que quería visualizar, en este caso, en qué regiones del país ocurrían más atropellos y qué tipo de señalética era la que se usaba en cada tramo.

De esta manera, se podían cruzar ambos datos, es decir, determinar qué regiones registraban la mayor cantidad de atropellos y el tipo de señalética que se empleaban en cada tramo.

## **Paso 2**

En segundo lugar, para decidir qué tipo de visualización representaba mejor la historia que quiero contar con esta base de datos, navegué por la página web: datavizproject. 

Esta web, que revisamos en clases, contiene una amplia y diversa cantidad de gráficos para hacer visualizaciones. Al seleccionar uno, se puede ver una breve descripción de este y los datos que utiliza para su elaboración. 

En base a esto, para la primera visualización decidí utilizar un Mapa de Pines o Pin Map y para la segunda visualización un Gráfico de Tabla o Table Chart. 

## **Paso 3**

En tercer lugar, para desarrollar correctamente los códigos que permitieran generar la visualización a través de Google Colab, realicé, con el apoyo de ChatGPT, un prompt que explicara en detalle el objetivo de la solicitud: desarrollar el tipo de gráfico (con una descripción de este, disponible en la web datavizproject) y los datos que necesitaba para la visualización. 

En el caso del Pin Map, necesitaba las coordenadas de cada región y la cantidad de accidentes que ocurrían en estas. Una vez generado el código con ChatGPT, me dediqué a hacer una revisión de este, agregar los datos uno por uno de la cantidad de accidentes y de las regiones en específico que necesitaba, sumado a cambios como el color y tamaño. 

En el caso del Gráfico de Tabla, necesitaba que quedaran las columnas de regiones y el tipo de señalética que había por región. Al igual que el anterior, una vez desarrollado el código con ChatGPT, edité uno por uno los datos de las regiones correspondientes a la cantidad de señaléticas que tenían, las que podrían ser: AUV, ERTMS N1, CTC y SSE / SB.

## **Paso 4**

Finalmente, tras revisar que todos los datos estuvieran correctos y con los detalles que esperaba, en cuanto a color, ubicación, tamaño, entre otros, ejecuté en Google Colab los códigos que permitieron visualizarlos. 

## Base de datos (CSV)

Para estas visualizaciones utilicé dos bases de datos. La primera, a partir de datos entregados por Carabineros de Chile, para generar el Pin Map, fue sobre la cantidad de atropellos que ocurrieron entre el 2017 a abril de 2025 en las regiones de Antofagasta, Atacama, Coquimbo, Valparaíso, O´Higgins, Maule, Ñuble, Bio-Bio, La Araucanía, Los Ríos y región Metropolitana. Sumé la cantidad de accidentes en cada región y con estos datos desarrollé el Pin Map.

De esta manera, se puede observar de una forma atractiva y dinámica cuáles son las regiones con mayor cantidad de atropellos o accidentes en el país. 

Para la segunda visualización, es decir, el Gráfico de Tabla, utilicé una base de datos generada a partir de datos publicados por EFE, donde se detalla el tipo de señalización;  AUV, ERTMS N1, CTC y SSE / SB que tiene cada tramo de las regiones de Valparaíso, Metropolitana, O´Higgins, Maule, Ñuble, Bio-Bio, La Araucanía y Los Ríos. En este caso, seleccioné los tipos de señaléticas por región.

Esto, con el fin de dar cuenta que los atropellos tienen directa relación con el tipo de señalización que se encuentran en las regiones.

-----------------------------------------------

La idea de utilizar las dos bases de datos y los tipos de gráficos, es dar cuenta de la relación que se observa entre atropellos y el tipo de señalización por región, lo que podría influir en la cantidad de fallecidos.


## Preguntas que pueden responder las visualizaciones

1. ¿Cuál es la región con más fallecidos por atropellos en las vías férreas desde 2017 a abril de 2025?

2. De las tres regiones con más fallecidos, ¿qué tipo de señalizaciones son los más utilizados?

3. De las tres regiones con menos fallecidos, ¿qué tipo de señalizaciones utilizan?










