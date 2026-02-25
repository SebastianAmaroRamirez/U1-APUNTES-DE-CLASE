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

## 🚀 1.2 Áreas de aplicación
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

## 📐 1.3 Aspectos matemáticos de la graficación
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

## 🎨 1.4 Modelos del color: RGB, CMY, HSV y HSL
Los modelos de color son sistemas matemáticos que nos permiten representar los colores mediante valores numéricos. En graficación, elegir el modelo correcto depende de si el destino es una pantalla, una impresora o una interfaz de usuario.

### 🔴 Modelo RGB (Red, Green, Blue)
Es un modelo aditivo (la suma de colores produce blanco). Es el estándar para todo lo que tenga una pantalla (monitores, móviles, proyectores).

- Uso: Gráficos digitales, web, videojuegos.

- Componentes: Cada color se define por la intensidad de Rojo, Verde y Azul, usualmente en rangos de $0$ a $255$.



| Modelo | Descripción |
| :--- | :--- |
| **RGB** | Rojo, Verde, Azul (Aditivo) |
| **CMY** | Cian, Magenta, Amarillo (Sustractivo) |
| **HSV** | Matiz, Saturación, Valor |
| **HSL** | Matiz, Saturación, Luminosidad |

### 1.5 Representación y trazo de líneas y polígonos
*(Explicación de algoritmos como Bresenham o DDA)*

#### 1.5.1 Formatos de imagen
*(PNG, JPG, BMP, SVG)*

### 1.6 Procesamiento de mapas de bits
*(Manipulación de píxeles y transformaciones de imágenes)*
