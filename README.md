# U1-APUNTES-DE-CLASE
Temas de la Unidad 1
# 🖥️ Graficación por Computadora

## 📖 Índice de Contenidos

---

### [Unidad I. Introducción a la graficación por computadora](#unidad-i-introducción-a-la-graficación-por-computadora)

* **1.1** [Historia y evolución de la graficación](#11-historia-y-evolución-de-la-graficación-por-computadora)
* **1.2** [Áreas de aplicación](#12-áreas-de-aplicación)
* **1.3** [Aspectos matemáticos de la graficación](#13-aspectos-matemáticos-de-la-graficación)
* **1.4** [Modelos del color: RGB, CMY, HSV y HSL](#14-modelos-del-color-rgb-cmy-hsv-y-hsl)
* **1.5** [Representación y trazo de líneas y polígonos](#15-representación-y-trazo-de-líneas-y-polígonos)
    * **1.5.1** [Formatos de imagen](#151-formatos-de-imagen)
* **1.6** [Procesamiento de mapas de bits](#16-procesamiento-de-mapas-de-bits)

---

## Unidad I. Introducción a la graficación por computadora

## 1.1 Historia y evolución de la graficación por computadora
La graficación por computadora ha pasado de ser una curiosidad de laboratorio a la base visual de nuestra era digital. Su evolución se puede dividir en hitos fundamentales:

### ⏳ Cronología de Hitos Clave

- **1950s - Los inicios:** Surge el SAGE (Semi-Automatic Ground Environment) de la Fuerza Aérea de EE. UU., que utilizaba pantallas vectoriales para mostrar trayectorias de radar. Es considerado uno de los primeros sistemas gráficos interactivos.

- **1963 - Sketchpad:** Ivan Sutherland crea Sketchpad en el MIT. Fue el primer programa que permitió la manipulación directa de objetos gráficos en una pantalla mediante un lápiz óptico, sentando las bases de la interfaz gráfica de usuario (GUI) y el CAD.

- **1970s - El nacimiento de los algoritmos:** Aparecen algoritmos fundamentales que usamos hoy en día, como el sombreado de Gouraud (1971) y el sombreado de Phong (1975), permitiendo superficies curvas más realistas.

- **1980s - La era de la computación personal:** Con el lanzamiento de la Macintosh (1984) y la Commodore Amiga, los gráficos de alta resolución y las interfaces de ventanas llegan al público general.

- **1990s - La revolución 3D:** Aparecen las primeras tarjetas aceleradoras de video (GPUs) y películas como Toy Story (1995), el primer largometraje generado totalmente por computadora.

- **2000s en adelante - Realismo Extremo:** Se estandarizan tecnologías como el Ray Tracing (Trazado de rayos) en tiempo real y los motores de videojuegos de alta fidelidad (Unreal Engine, Unity), borrando la línea entre lo real y lo digital.

### 🏆 Personajes Influyentes
- **Ivan Sutherland:** "Padre de la graficación por computadora".

- **Jim Blinn:** Pionero en el mapeo de texturas y reflexión.

- **Edwin Catmull:** Cofundador de Pixar y creador del algoritmo de Z-buffer.

<p align="center">
  <img src="https://github.com/user-attachments/assets/3e11e161-d8cd-414c-832d-68a71bbe28b0" width="600" title="Evolución de la Graficación">
  <br>
  <em>Figura 1: Evolución de la graficación por computadora.</em>
</p>

----

## 1.2 Áreas de aplicación
La graficación por computadora es el pilar de diversas industrias modernas. Sus aplicaciones se dividen en los siguientes sectores estratégicos:

### 🎮 Entretenimiento y Medios Digitales
- **Videojuegos:** Renderizado en tiempo real (motores como Unreal Engine o Unity).

- **Cine y Efectos** Visuales (VFX): Creación de personajes CGI, escenarios digitales y composición de video.

- **Publicidad:** Modelado de productos y animaciones comerciales de alta fidelidad.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d5cd0388-0ec3-455c-9298-bfb6422e904f" width="500" title="Evolución de la Graficación">
  <br>
  <em>Figura 2: Entretenimiento y Medios Digitales.</em>
</p>

### 🏥 Ciencia y Medicina
- **Visualización Científica:** Representación de datos complejos (clima, fluidos, física de partículas).

- **Imagenología Médica:** Reconstrucción 3D de tomografías (TAC) y resonancias magnéticas para planeación quirúrgica.

<p align="center">
  <img src="https://github.com/user-attachments/assets/bfd826a5-d00f-4a5b-a1e4-72c3476b4c97" width="200" title="Evolución de la Graficación">
  <br>
  <em>Figura 3: Ciencia y Medicina.</em>
</p>

### 🏗️ Diseño y Manufactura (CAD/CAM)
- **Arquitectura:** Recorridos virtuales (VR) y renderizado de planos.

- **Ingeniería:** Diseño Asistido por Computadora (CAD) para prototipado de piezas industriales y automotrices.

<p align="center">
  <img src="https://github.com/user-attachments/assets/57304eae-b88a-4419-ad96-bc045902ec40" width="400" title="Evolución de la Graficación">
  <br>
  <em>Figura 4: Diseño y Manufactura (CAD/CAM).</em>
</p>

### 🎓 Educación y Entrenamiento
- **Simuladores:** Entrenamiento de pilotos, conductores y cirujanos en entornos virtuales seguros.

- **E-Learning:** Gráficos interactivos para explicar conceptos abstractos de matemáticas o biología.

<p align="center">
  <img src="https://github.com/user-attachments/assets/21858bfc-57c1-4d44-9e44-68fc15cd37f1" width="400" title="Evolución de la Graficación">
  <br>
  <em>Figura 5: Educación y Entrenamiento.</em>
</p>

----

## 1.3 Aspectos matemáticos de la graficación
La graficación por computadora no es más que la manipulación de datos numéricos para representar formas en un espacio bidimensional o tridimensional.

**1. Geometría y Espacios de Coordenadas**
Para situar un objeto, necesitamos definir su posición en un sistema de referencia.

- **Coordenadas Cartesianas:** El estándar en 2D $(x, y)$ y 3D $(x, y, z)$.

- **Coordenadas Homogéneas:** Utilizadas para facilitar las transformaciones, añadiendo una cuarta componente $w$. Un punto en 3D se representa como $(x, y, z, w)$.

**2. Álgebra Lineal: Transformaciones**
Las transformaciones son el corazón de la computación gráfica. Se realizan mediante la multiplicación de Matrices de Transformación:

- **Traslación:** Mueve un objeto a una nueva posición.

- **Escalamiento:** Cambia el tamaño del objeto.

- **Rotación:** Gira el objeto alrededor de un eje.

**3. Proyecciones**
Es el proceso de convertir coordenadas 3D a una pantalla 2D:

- Proyección Perspectiva: Los objetos se ven más pequeños a medida que se alejan (simula el ojo humano).

- Proyección Ortográfica: Mantiene las dimensiones reales (ideal para planos técnicos y CAD).

**4. Álgebra de Vectores**
Esencial para el cálculo de iluminación y sombreado:

- Producto Punto ($\cdot$): Determina el ángulo entre dos vectores (clave para saber cuánta luz recibe una superficie).

- Producto Cruz ($\times$): Permite calcular el vector normal a una superficie, necesario para definir hacia dónde "mira" un polígono.

----

## 1.4 Modelos del color: RGB, CMY, HSV y HSL
Los modelos de color son sistemas matemáticos que nos permiten representar los colores mediante valores numéricos. En graficación, elegir el modelo correcto depende de si el destino es una pantalla, una impresora o una interfaz de usuario.

### 🔴 Modelo RGB (Red, Green, Blue)
Es un modelo aditivo (la suma de colores produce blanco). Es el estándar para todo lo que tenga una pantalla (monitores, móviles, proyectores).

- Uso: Gráficos digitales, web, videojuegos.

- Componentes: Cada color se define por la intensidad de Rojo, Verde y Azul, usualmente en rangos de $0$  a  $255$.

### 🔵 Modelo CMY / CMYK (Cyan, Magenta, Yellow, Black)
Es un modelo sustractivo (la suma de colores produce negro). Es el estándar para medios físicos.

- **Uso:** Impresión offset y digital.

- **Dato:** En la práctica se añade la K (Black) porque la mezcla de cian, magenta y amarillo puros suele dar un café oscuro en lugar de un negro perfecto.

### 🌈 Modelos HSV y HSL (Perceptuales)
A diferencia de RGB, estos modelos se basan en cómo los humanos percibimos el color en lugar de cómo lo generan las máquinas.

- **HSV (Hue, Saturation, Value):** Matiz, Saturación y Valor.

- **HSL (Hue, Saturation, Lightness):** Matiz, Saturación y Luminosidad.

- **Uso:** Selectores de color en software de diseño (Photoshop, Figma) y retoque fotográfico.




| Modelo | Descripción |
| :--- | :--- |
| **RGB** | Rojo, Verde, Azul (Aditivo) |
| **CMY** | Cian, Magenta, Amarillo (Sustractivo) |
| **HSV** | Matiz, Saturación, Valor |
| **HSL** | Matiz, Saturación, Luminosidad |

## 1.5 Representación y trazo de líneas y polígonos
En graficación, este proceso se conoce como Rasterización. Dado que una pantalla es una rejilla de píxeles (discreta), no podemos dibujar una línea perfecta; debemos aproximarla activando los píxeles que mejor representen la trayectoria.

**1. Algoritmo DDA (Digital Differential Analyzer)**

Es el algoritmo más sencillo. Se basa en calcular la pendiente $m$ y aumentar las coordenadas paso a paso.

- **Ventaja:** Fácil de entender e implementar.

- **Desventaja:** Requiere operaciones de punto flotante (decimales), lo que lo hace lento para procesadores antiguos.

**2. Algoritmo de Bresenham**

Es el estándar de la industria para el trazo de líneas. Utiliza únicamente aritmética de enteros (sumas y restas), lo que lo hace extremadamente rápido.

- **Concepto:** Utiliza un "parámetro de decisión" para determinar qué píxel está más cerca de la línea real.

**3. Trazo de Polígonos**

Para representar polígonos, se utilizan dos enfoques principales:

- **Modelo de Alambre (Wireframe):** Solo se dibujan las líneas que conectan los vértices.

- **Relleno de Polígonos (Scan-line Fill):** Se recorre la pantalla fila por fila y se activan los píxeles que están "dentro" de las fronteras del polígono.

### 1.5.1 Formatos de imagen
*(PNG, JPG, BMP, SVG)*

### 1.6 Procesamiento de mapas de bits
Un mapa de bits (o raster) es una estructura de datos que representa una rejilla rectangular de píxeles. El procesamiento consiste en aplicar funciones matemáticas a estos píxeles para alterar la imagen original.

**1. Estructura de un Píxel**

En memoria, un mapa de bits se almacena como una matriz donde cada elemento (píxel) contiene información de color, generalmente en formato RGBA:

- **R, G, B:** Canales de color.

- **A (Alpha):** Canal de transparencia.

**2. Operaciones de Punto (Brillo y Contraste)**

Son las transformaciones más simples donde el nuevo valor de un píxel depende solo de su valor original.

- **Brillo:** Se suma o resta una constante a cada canal: $P_{nuevo} = P_{actual} + constante$.

- **Contraste:** Se multiplica el valor por un factor de escala.

**3. Filtros de Convolución (Transformaciones de Vecindad)**

Para efectos más complejos, el nuevo valor de un píxel depende de sus vecinos. Se utiliza una pequeña matriz llamada Kernel.

- **Desenfoque (Blur):** Promedia los valores de los píxeles circundantes.

- **Detección de Bordes (Sobel/Prewitt):** Resalta los cambios bruscos de intensidad en la imagen.

**4. Transformaciones Geométricas**

Modifican la posición de los píxeles en el mapa:

- Rotación y Traslación.

- Escalamiento: Requiere técnicas de interpolación (bilineal o bicúbica) para rellenar los "huecos" que se crean al agrandar una imagen.




