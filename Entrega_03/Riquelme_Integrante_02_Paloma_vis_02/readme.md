# README Paloma Riquelme 

## 1. Descripción general
Esta entrega individual presenta un conjunto de visualizaciones creadas con la librería **Altair (Python)**, que exploran los patrones de **accidentes ferroviarios en Chile** entre los años **2019 y 2024**, según edad, horario y día de la semana.

El propósito es apoyar una crónica periodística que investiga cómo ciertos grupos etarios y franjas horarias concentran la mayor cantidad de accidentes, y qué cambios se observan a lo largo del tiempo.  

La propuesta busca comunicar los resultados de forma **visual, clara y narrativa**, integrando la información en un dashboard diseñado para una **webstory periodística**.

## 2. Proceso de construcción

### a) Revisión y ampliación de bases
Siguiendo las observaciones recibidas en la evaluación anterior, se realizó una **búsqueda de bases de años adicionales** para ampliar el rango temporal del análisis y otorgar mayor validez a la comparación de tendencias.  
Se recopilaron los anuarios estadísticos de la **Empresa de Ferrocarriles del Estado (EFE)** entre **2019 y 2024**, consolidando tres dimensiones:
- Accidentes por **edad**
- Accidentes por **horario**
- Accidentes por **día de la semana**

Cada una de ellas se trató como base independiente, debido a que **no comparten una columna relacional directa**, lo que hace metodológicamente correcto mantenerlas separadas.


### b) Limpieza y procesamiento de datos
Se aplicaron procesos de limpieza con la librería `pandas`, que incluyeron:
- Estandarización de nombres de columnas (minúsculas, sin espacios ni caracteres especiales).  
- Conversión de formato ancho a largo mediante `pandas.melt()`.  
- Inclusión de los años faltantes, como **2021**, para mantener la continuidad temporal.  
- Reemplazo de valores vacíos o no informados por **cero**, asignando un nuevo campo descriptivo `estado` que indica:
  - `"Con registros"` → año con datos confirmados.
  - `"Sin accidentes reportados"` → año o categoría sin incidentes o sin registro.

Esta limpieza permitió crear un conjunto de datos coherente, replicable y con metadatos explícitos que documentan las ausencias de información.



### c) Visualización
Se elaboraron tres visualizaciones distintas en **Altair**, priorizando un diseño informativo y atractivo:
- **Gráfico 1:** Comparación por grupo etario y año, con colores diferenciados por tipo de accidente (fallecidos, graves, leves).
- **Gráfico 2:** Distribución horaria, con escala de intensidad y marcadores de ausencia de datos.
- **Gráfico 3:** Análisis por día de la semana, mostrando patrones de frecuencia y severidad.

Se usaron escalas de color **Tableau10** y **Viridis**, manteniendo la consistencia cromática y añadiendo el **gris** para indicar años sin registros oficiales.


### d) Exportación
Cada visualización fue exportada tanto en formato:
- `.html` → para la versión interactiva del dashboard.
- `.jpg` → para uso en publicaciones o versión impresa.

Finalmente, se integraron las tres visualizaciones en un **dashboard HTML unificado**, optimizado para visualización en web y compatible con narrativas multimedia.


## 3. Preguntas que responde la visualización
- ¿Qué grupos etarios concentran más accidentes ferroviarios y cómo ha cambiado esto en el tiempo?  
- ¿En qué horarios se producen más siniestros graves o mortales?  
- ¿Qué días de la semana presentan mayor recurrencia?  
- ¿Existen períodos sin registro (ausencia real o falta de información)?  


## 4. Herramientas utilizadas
- **Python 3.12**
- **Pandas** – procesamiento y limpieza de datos  
- **Altair** – visualización y diseño narrativo  
- **Google Colab / Jupyter Notebook** – scripting y documentación  
- **HTML / JPG** – exportación y presentación final  


## 5. Resultados esperados
El producto final busca ofrecer una mirada clara y comprensible sobre los accidentes ferroviarios en Chile, destacando su **dimensión temporal** y **patrón social**, además de transparentar los vacíos informativos existentes en los registros oficiales.
