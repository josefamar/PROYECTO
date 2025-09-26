## Ficha técnica Paloma Riquelme

### Fuente de los datos
•	Informe de Siniestros Ferroviarios 2024, elaborado por la Comisión Nacional de Seguridad de Tránsito (CONASET) a partir de registros de Carabineros de Chile y el Observatorio de Datos del Ministerio de Transportes y Telecomunicaciones.
### Metodología de la construcción de la base
1. **Extracción:**  Se seleccionaron las tablas contenidas en el informe en PDF, específicamente las referidas a siniestros según horario, día, mes, causa, tipo de siniestro y usuarios involucrados.
2.	**Conversión:** Los cuadros fueron exportados a un formato tabular (Excel/CSV) para permitir análisis exploratorio.
3.	**Selección de variables:** Para esta entrega, se priorizó la tabla de siniestros según horario (2024), ya que permite observar los momentos del día donde existe mayor concentración de accidentes y fallecidos.
4.	**Estandarización:** Se unificaron los tramos horarios en intervalos de 3 horas, manteniendo la misma codificación del informe (00:00–02:59; 03:00–05:59; etc.).
5.	**Codificación** Cada fila representa un tramo horario con variables numéricas asociadas (n° de siniestros, fallecidos, lesionados).
### Alcance de los datos
• **Cobertura temporal:** Año 2024.
• **Cobertura geográfica:** Nacional (Chile).
•	**Unidad de análisis:** tramo horario de ocurrencia del siniestro.
•	**Nivel de desagregación:** datos agregados, no individualizados por comuna o región.
### Características de los datos
•	Datos oficiales y validados, con acceso público.
•	**Naturaleza cuantitativa:** número de siniestros, fallecidos y lesionados.
•	**Nivel de análisis:** exploratorio/descriptivo.
•	**Limitación:** no permite georreferenciar accidentes, pero sí caracterizar patrones temporales.
### Variables incorporadas
* Horario:	Tramo horario en el que ocurrió el siniestro (ej. 18:00–20:59)	Categórica
* Siniestros:	Número de siniestros ferroviarios registrados en ese tramo	
* Fallecidos:	Número de fallecidos en ese tramo horario	
Total de lesionados en ese tramo horario
Sseveridad	
#### Otras observaciones
•	El horario 18:00–20:59 concentró el mayor número de siniestros (19) y fallecidos (7).
•	El segundo tramo más crítico fue 09:00–11:59 (18 siniestros, aunque menos fatal).
•	La madrugada (00:00–05:59) presentó un índice de severidad más alto que otros horarios, lo que sugiere mayor letalidad cuando ocurren accidentes a esas horas.

### 4. Documentación

Proceso de limpieza de datos
Paso 1: Extracción
•	Se identificó la tabla de siniestros ferroviarios según horario (2024) en el informe.
•	Se transcribieron los datos a un archivo Excel para estructurarlos en formato de filas y columnas.
Paso 2: Normalización
•	Se mantuvo la misma categorización de tramos horarios usada por CONASET (intervalos de 3 horas).
•	Se verificó consistencia entre totales (103 siniestros, 29 fallecidos, 58 lesionados) y los subtotales por horario.
Paso 3: Limpieza
•	No hubo duplicados ni datos inconsistentes, pero sí se ajustaron nombres de variables (ej. “Menos graves” → Semi graves).
•	Se codificaron todas las variables con nombres en minúsculas y sin espacios, para mejorar su manejo en Excel y software estadístico.
Paso 4: Validación
•	Los totales por fila fueron contrastados con el cuadro original del informe, confirmando correspondencia 1:1.

### Fuente utilizada
•	Informe de Siniestros Ferroviarios 2024 (CONASET).
Justificación:
Es una de las fuentes oficiales y pública que recopila, sistematiza y valida información sobre siniestros ferroviarios en Chile.

### Ejemplos de preguntas que se pueden responder con la base limpia
1.	¿En qué tramo horario se concentran más siniestros ferroviarios?

2.	¿Qué horarios presentan mayor mortalidad (fallecidos por siniestro)?

3.	¿Cómo varía la ocurrencia de siniestros entre las horas punta y las horas de menor circulación?


