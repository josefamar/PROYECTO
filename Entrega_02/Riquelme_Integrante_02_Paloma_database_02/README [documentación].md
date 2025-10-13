## Documentación
Paloma Riquelme
### Proceso de limpieza de datos
1. **Extracción manual:**  
   - Copia de cada tabla (día, edad y horario) directamente desde el PDF.
   - Pega inicial en Excel, conservando la estructura original.

2. **Normalización:**
* Se mantuvo la misma categorización de tramos horarios usada por CONASET (intervalos de 3 horas).
* Se verificó consistencia entre totales (103 siniestros, 29 fallecidos, 58 lesionados) y los subtotales por horario.

3. **Unificación:**  
   - Creación de una sola hoja en Excel con toda la información combinada.
   - Inclusión de una columna clave llamada `categoria` para identificar el origen de cada registro:  
     - `"DIA"`, `"EDAD"`, `"HORARIO"`.

4. **Validación:**  
   - Revisión de totales y cruces:
     - **Total siniestros:** 103.  
     - **Fallecidos:** 29.  
     - **Lesionados:** 58 (29 graves, 8 menos graves, 21 leves).

5. **Limpieza:**
* No hubo duplicados ni datos inconsistentes, pero sí se ajustaron nombres de variables (ej. “Menos graves” → Semi graves).
* Se codificaron todas las variables con nombres en minúsculas y sin espacios, para mejorar su manejo en Excel y software estadístico.
Paso 4: Validación
* Los totales por fila fueron contrastados con el cuadro original del informe, confirmando correspondencia 1:1.


### Fuente utilizada
* Informe de Siniestros Ferroviarios 2024 (CONASET).
**Justificación:**
Quiero aclarar que siguiendo sus correcciones hemos decidido hacer un cambio en las fuentes base, para hacer una mejor correlacion entre los datos y la encontramos importante porque es una de las fuentes oficiales y pública que recopila, sistematiza y valida información sobre siniestros ferroviarios en Chile.

### Ejemplos de preguntas que se pueden responder con la base limpia
1.	¿En qué tramo horario se concentran más siniestros ferroviarios?
2.	¿Qué horarios presentan mayor mortalidad (fallecidos por siniestro)?
3.	¿Cómo varía la ocurrencia de siniestros entre las horas punta y las horas de menor circulación?
4.	¿Qué grupo etario concentra más fallecidos en siniestros ferroviarios?
5.	¿En qué tramo horario ocurren más siniestros y en cuál se registran más muertes?
6.	¿Qué horario presenta mayor índice de severidad?
7.	¿Cómo se distribuyen los lesionados (graves, menos graves, leves) según la edad y el horario?
8.	¿Existen diferencias entre cantidad de siniestros y severidad de consecuencias?
