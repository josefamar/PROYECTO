# Análisis de diseño de la historia – Entrega 06

## 1. Estructura narrativa y recorrido del usuario

La historia web está organizada como un viaje en tren a través de distintas “estaciones” temáticas. Cada sección corresponde a un bloque narrativo y a una parte del argumento periodístico:

1. **Inicio**  
   Plantea el foco general: los atropellos ferroviarios del tramo Estación Central–Maule no se explican solo por imprudencia, sino por fallas estructurales del sistema. Se establece el tono editorial y se introducen el período de análisis (2014–2024) y el tramo geográfico.

2. **San Bernardo**  
   Usa la colisión de trenes de 2024 como escena de apertura. No se presenta como dato de la base de atropellos, sino como caso que revela las costuras del sistema ferroviario: convivencia entre vías, cruces y barrios residenciales. El mapa analítico refuerza visualmente el argumento.

3. **Señalización**  
   Explica cómo funcionan AUV y CTC, subrayando que fueron diseñados principalmente para ordenar trenes, no para proteger peatones. Se articulan visualizaciones que muestran la relación entre tramos, sistemas de control y número de siniestros.

4. **Territorio**  
   Introduce el índice de peligrosidad (IP) y muestra la concentración territorial del riesgo. Aquí la historia pasa de la descripción de casos a la medición estructural del problema, a través de la visualización de IP por comuna.

5. **Patrones humanos**  
   Profundiza en quiénes y cuándo cargan con el riesgo: grupos de edad, horarios y días de la semana. Las visualizaciones atómicas se combinan con una crónica que conecta los datos con rutinas cotidianas (trabajo, estudio, vida de barrio).

6. **Conclusión**  
   Integra los hallazgos y desplaza el foco desde la culpa individual a la responsabilidad estructural: empresas ferroviarias, autoridades, municipios y diseño urbano.

7. **Metodología**  
   Explica las fuentes de datos, criterios de filtrado, construcción del IP y uso de herramientas. Garantiza transparencia y replicabilidad del trabajo periodístico.

8. **Equipo**  
   Cierra reconociendo la autoría y los roles del equipo, reforzando la dimensión colaborativa del proyecto.

### Recorrido del usuario

La navegación principal se realiza a través de una barra superior que simula un **tren en movimiento**. Cada “estación” es un botón que desplaza al usuario a una sección específica. Al mismo tiempo, el tren se mueve en sincronía con el scroll, reforzando la metáfora de recorrido y brindando feedback visual de avance en la historia.

Esta decisión de diseño:

- Estructura la lectura en módulos claros.  
- Permite volver a secciones clave sin perderse.  
- Conecta el tema (ferrocarriles) con la forma de navegar.

---

## 2. Crónica, textos y estilo narrativo

La crónica mezcla:

- Descripciones situadas (San Bernardo, cruces, barrios).  
- Explicaciones técnicas (AUV, CTC, IP) traducidas a lenguaje comprensible.  
- Interpretación de patrones de datos (edades, horarios, territorio).  
- Momentos de reflexión editorial (conclusión).

### Estilo narrativo

Se optó por un estilo que:

- Equilibra **prosa periodística** con precisión técnica.  
- Evita jerga innecesaria, explicando siglas y conceptos (ej: IP, AUV, CTC).  
- Usa citas y formulaciones que invitan a la reflexión, en lugar de moralizar.

La amplificación se utiliza para:

- Convertir visualizaciones en historia: cada gráfico está acompañado de un párrafo que traduce “lo que se ve” en un mensaje periodístico.  
- Humanizar las cifras, reforzando que detrás de cada barra o punto en el mapa hay vidas y territorios concretos.

---

## 3. Diseño de información e interacción

### Diseño de información

Algunas decisiones clave:

- **Orden temático:** primero se instala la escena (San Bernardo), luego la infraestructura (Señalización), después el territorio (IP) y finalmente las personas (Patrones). Este orden permite ir desde lo visible y puntual hacia lo estructural.
- **Agrupación de visualizaciones:** las visualizaciones se ubican junto a los bloques de texto que las interpretan, evitando que el usuario deba desplazarse entre secciones para entenderlas.
- **Progresión de complejidad:** se parte de gráficos más panorámicos (por región/tramo) y se avanza hacia gráficos que requieren mayor interpretación (IP, patrones temporales).

### Diseño de interacción

- **Tren de navegación:** refuerza el concepto de recorrido y ayuda a que la usuaria/usuario ubique su posición en la historia.  
- **Scroll + click:** el sitio permite recorrer la historia de forma lineal (scroll) o saltar entre estaciones (click en el menú).  
- **Mapa interactivo Leaflet:** permite explorar el entorno del siniestro de San Bernardo más allá del texto, apoyando el argumento de convivencia estrecha entre vía y ciudad.

Estas decisiones buscan que la interacción no sea un adorno, sino una forma de comprender mejor la historia.

---

## 4. Decisiones visuales: logo, colores, tipografías, fotos

### Logo

El logo de **Punto Ciego** combina un elemento gráfico ferroviario con una composición tipográfica robusta. Representa:

- La idea de “señal” o advertencia.  
- La presencia de un sistema (vías, cruces) que no siempre ve a las personas.

### Paleta de colores

Se utiliza una paleta inspirada en:

- **Azules oscuros y aceros:** remiten al fierro, la infraestructura y la noche.  
- **Amarillo señalética:** asociado a advertencia, cruces y demarcación vial.  
- **Naranja óxido y tonos cálidos suaves:** evocan desgaste, tiempo y vulnerabilidad.

El uso de color cumple funciones de jerarquía:

- Secciones críticas (San Bernardo, Conclusión) utilizan fondos más contrastados.  
- Secciones analíticas (Territorio, Metodología) usan fondos claros con acentos de color para los bordes.

### Tipografías

- **Bebas Neue:** para títulos y encabezados, entregando un carácter fuerte y legible, con sensación de afiche ferroviario o señalética.  
- **Poppins:** para el cuerpo de texto, por su buena legibilidad en pantalla.

La combinación aporta una sensación de seriedad, contemporaneidad y claridad, sin perder el carácter editorial.

### Imágenes y recursos visuales

- **Portada con tren en movimiento (index):** la animación del fondo simula el desplazamiento del tren, reforzando la metáfora de viaje y preparando al usuario para la experiencia narrativa de la webstory.  
- **Foto/imagen del accidente de San Bernardo:** sitúa el caso en un lugar y tiempo concretos, conectando el dato con una escena real.  
- **Mapa analítico:** combina simbología simple (círculos, polígonos) con un layout limpio que evita saturar al usuario.

---

## 5. Coherencia entre diseño, hipótesis e historia

- La **hipótesis** plantea que el problema es estructural (sistema, territorio, cotidianidad).  
- El **diseño de información** sigue el mismo enfoque: estructura la webstory como un recorrido por piezas del sistema (señalización, territorio, patrones humanos).  
- El **diseño visual** remite constantemente al mundo ferroviario: tren, rieles, señalética, colores industriales.
- La **interacción** (tren que avanza, mapa, visualizaciones) no es solo ornamental, sino que organiza y hace visible la complejidad del fenómeno.

En conjunto, estas decisiones buscan que la persona que visita la web no solo lea un reportaje, sino que experimente un **viaje guiado** a través de los puntos ciegos del sistema ferroviario chileno.
