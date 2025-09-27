### Documentación
Paloma Riquelme
### Proceso de limpieza de datos
Quiero aclarar que siguiendo sus correcciones hemos decidido hacer un cambio en las fuentes base. 
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

