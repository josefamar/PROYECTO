# Análisis de las visualizaciones

Nuestro trabajo consiste en un reportaje gráfico alojado en una página web, cuya hipótesis plantea que, aunque la imprudencia de los peatones en las vías férreas es señalada como una de las principales causas de accidentes, también existen fallas estructurales y técnicas que contribuyen de manera significativa a que estos siniestros ocurran. A partir de esa premisa, analizamos nuestras visualizaciones, explicando qué dimensión de la problemática aborda cada una y qué mensaje buscamos comunicar con ellas dentro del relato general

---

## 1. Visualización 1 – Atropellos por región / tramo  
**Archivo código:** `codigo/andres_vis1.html`  
**Base de datos:** `base_datos/atropellos_tramo_ec_maule.csv`  
**Imagen referencial:** `imagenes/andres_vis1.png`

### Dimensiones y variables

- Eje X: Región / tramo (ej. Metropolitana, O’Higgins, Maule).  
- Eje Y: Número de atropellos ferroviarios (2014–2024).  
- Filtro implícito: tipo de siniestro = atropello; tramo = Estación Central–Maule.

### Mensaje periodístico

Esta visualización entrega una primera panorámica territorial: permite identificar que los atropellos no se distribuyen homogéneamente, sino que se concentran en ciertos tramos/regiones del recorrido. Esto sirve como puerta de entrada a la idea de **“territorios con riesgo acumulado”**, y refuerza el foco de que no se trata solo de eventos aislados.

### Rol en la historia

- Aparece asociada a la sección de **Señalización** como contexto macro.  
- Introduce la transición hacia el análisis más fino del índice de peligrosidad (IP).

---

## 2. Visualización 2 – Tipos de señalización / tramos  
**Archivo código:** `codigo/andres_vis2.html`  
**Base de datos:** `base_datos/atropellos_tramo_ec_maule.csv` (columnas asociadas a tipo de sistema AUV/CTC y cruces)  
**Imagen referencial:** `imagenes/andres_vis2.png`

### Dimensiones y variables

- Categorías: tramos con predominio de AUV, de CTC o mixtos.  
- Métrica: número de siniestros / presencia de cruces a nivel.  

### Mensaje periodístico

Esta visualización conecta directamente la dimensión técnica del sistema ferroviario (AUV/CTC) con el riesgo que enfrentan las personas. Muestra que los tramos con combinaciones de sistemas o con señalización deficiente tienden a concentrar más atropellos.

### Rol en la historia

- Refuerza el argumento de que **los sistemas de control se diseñaron para trenes, no para peatones**.  
- Ayuda a explicar por qué la “imprudencia” individual no basta como explicación.

---

## 3. Visualización 3 – Índice de peligrosidad (IP) por comuna  
**Archivo código:** `codigo/mariñanco_grafico2.html`  
**Base de datos:** `base_datos/indice_peligrosidad_comunas.csv`  
**Imagen referencial:** `imagenes/mariñanco_grafico2.png`

### Dimensiones y variables

- Unidades de análisis: comunas del tramo Estación Central–Maule.  
- Variables combinadas en el IP:
  - cantidad de atropellos,
  - presencia/tipo de cruces,
  - población expuesta,
  - características del entorno (residencial/industrial/mixto).

### Mensaje periodístico

El IP permite pasar de contar accidentes a medir **riesgo estructural**. Muestra comunas donde la vulnerabilidad no es un episodio, sino una condición permanente. Refuerza la tesis de que hay territorios donde el diseño urbano y ferroviario hace prácticamente inevitable cruzar la vía en condiciones peligrosas.

### Rol en la historia

- Eje central de la sección **Territorios en riesgo**.  
- Marca un antes y un después en la investigación, porque transforma la base de datos en una herramienta para priorizar intervención pública.

---

## 4. Visualización 4 – Edades de las víctimas  
**Archivo código:** `codigo/edades.html`  
**Base de datos:** `base_datos/edades_victimas.csv`  
**Imagen referencial:** `imagenes/edades.png`

### Dimensiones y variables

- Categorías de edad (ej. 0–17, 18–29, 30–44, 45–59, 60+).  
- Conteo de víctimas por grupo etario.

### Mensaje periodístico

Muestra que la exposición al riesgo no está concentrada en un solo grupo, pero se intensifica en **adultos en edad laboral** y también en **personas mayores**. Esto refuerza que el problema está ligado a rutinas cotidianas (trabajo, estudio, trámites), más que a conductas excepcionales.

### Rol en la historia

- Se inserta en la sección de **Patrones humanos**.  
- Ayuda a humanizar la estadística, recordando que detrás de cada barra hay proyectos de vida y responsabilidades familiares.

---

## 5. Visualización 5 – Horario de ocurrencia de los atropellos  
**Archivo código:** `codigo/zona_horaria.html`  
**Base de datos:** `base_datos/horarios_atropellos.csv`  
**Imagen referencial:** `imagenes/zona_horaria.png`

### Dimensiones y variables

- Eje X: franjas horarias (ej. madrugada, mañana, tarde, noche).  
- Eje Y: número de atropellos en cada franja.

### Mensaje periodístico

Revela que los siniestros se concentran en horarios donde coinciden **mayor flujo de personas y menor visibilidad** (tardes y noches). Esto cuestiona la idea de que los atropellos son “accidentes inesperados” y los sitúa dentro de contextos predecibles.

### Rol en la historia

- Profundiza en la idea de “vida cotidiana en riesgo”.  
- Conecta con la experiencia de quienes vuelven del trabajo, estudian o viajan en horarios complejos.

---

## 6. Visualización 6 – Día de la semana  
**Archivo código:** `codigo/dia_semana.html`  
**Base de datos:** `base_datos/dia_semana_atropellos.csv`  
**Imagen referencial:** `imagenes/dia_semana.png`

### Dimensiones y variables

- Categorías: lunes–domingo.  
- Conteo de atropellos por día.

### Mensaje periodístico

Permite distinguir entre rutinas laborales (lunes a viernes) y posibles patrones asociados a tiempo libre o viajes de fin de semana. Contribuye a perfilar cuándo el sistema exige “cruzar igual” a pesar del riesgo.

### Rol en la historia

- Completa el bloque de **Patrones humanos**.  
- Ayuda a conectar la narración con experiencias concretas (ir al colegio, viajar, salir el fin de semana).

---

## 7. Mapa analítico del siniestro de San Bernardo (Leaflet)

**Archivo código:** `mapasanbernardo.js` (en docs)  
**Imagen de contexto:** `imagenes/san_bernardo_contexto.png`  
**Base cartográfica:** OpenStreetMap  

### Dimensiones y variables

- Coordenadas geográficas de:
  - punto del accidente (colisión tren de pruebas / tren de carga),
  - cruces vehiculares y peatonales,
  - zona residencial,
  - estación próxima.
- Polígono de área de riesgo (interacción entre vía, maniobras y entorno habitado).

### Mensaje periodístico

Aunque el siniestro de San Bernardo no corresponde a un atropello, **funciona como escena emblemática**: evidencia cómo se combinan operaciones complejas, señalización vulnerable y proximidad con barrios residenciales. El mapa permite ver que la vía no es una línea abstracta, sino un dispositivo que atraviesa la vida diaria de una comuna densamente poblada.

### Rol en la historia

- Actúa como **caso de apertura** de la webstory.  
- Establece un puente visual y conceptual entre la colisión entre trenes y los atropellos a peatones, subrayando las fallas sistémicas compartidas.

---
