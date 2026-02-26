# U1-APUNTES-DE-CLASE

**Temas de la Unidad 1**

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

- **Cine y Efectos Visuales (VFX):** Creación de personajes CGI, escenarios digitales y composición de video.

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

- **Uso:** Gráficos digitales, web, videojuegos.

- **Componentes:** Cada color se define por la intensidad de Rojo, Verde y Azul, usualmente en rangos de $0$  a  $255$.

### 🔵 Modelo CMY / CMYK (Cyan, Magenta, Yellow, Black)
Es un modelo sustractivo (la suma de colores produce negro). Es el estándar para medios físicos.

- **Uso:** Impresión offset y digital.

- **Dato:** En la práctica se añade la K (Black) porque la mezcla de cian, magenta y amarillo puros suele dar un café oscuro en lugar de un negro perfecto.

### 🌈 Modelos HSV y HSL (Perceptuales)
A diferencia de RGB, estos modelos se basan en cómo los humanos percibimos el color en lugar de cómo lo generan las máquinas.

- **HSV (Hue, Saturation, Value):** Matiz, Saturación y Valor.

- **HSL (Hue, Saturation, Lightness):** Matiz, Saturación y Luminosidad.

- **Uso:** Selectores de color en software de diseño (Photoshop, Figma) y retoque fotográfico.

---

<p align="center">
  <img src="https://github.com/user-attachments/assets/f7e7e5a3-3fe5-47af-b7ed-41b4eb6a5801" width="400" title="Evolución de la Graficación">
  <br>
  <em>Figura 6: Ejemplo.</em>
</p>

---


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

## 1.5.1 Formatos de imagen

**Representación y trazo de líneas y polígonos.**

**Explicación de Código en Blender**

**Código completo:**

<img width="366" height="547" alt="image" src="https://github.com/user-attachments/assets/eb3a3efc-8e21-41d5-ae8b-c30ff9803495" />


**1. Importación de Librerías**

<img width="95" height="30" alt="image" src="https://github.com/user-attachments/assets/272544f7-4093-4ab1-bf37-ee091f93c4e7" />

* **bpy:** Es la librería principal de Blender. Permite controlar la interfaz, crear objetos, materiales y mallas.
* **math:** Proporciona funciones matemáticas esenciales.

**2. Definición de la Función Principal**

<img width="312" height="18" alt="image" src="https://github.com/user-attachments/assets/bf525021-a739-493e-b5df-6299cf466732" />

Esta función es el "molde". Recibe tres datos:
* **nombre:** El nombre que tendrá el objeto en tu escena.
* **lados:** Cuántos lados tendrá el polígono (ej. 3 para un triángulo, 6 para un hexágono).
* **radio:** Qué tan grande será la figura desde el centro hasta sus puntas.

**3. Creación de la Estructura de Datos**

<img width="326" height="87" alt="image" src="https://github.com/user-attachments/assets/9e717571-28a9-435d-b358-54b0fa883293" />

* **Malla (Mesh):** Es el contenedor de los datos "invisibles" (puntos y líneas).
* **Objeto:** Es la representación del ítem en la escena 3D.
* **Link:** Esta línea es crucial; sin ella, el objeto existe en la memoria pero no aparece en tu pantalla.

**4. El Motor Matemático (Cálculo de Vértices)**

<img width="344" height="97" alt="image" src="https://github.com/user-attachments/assets/5ea78d90-6848-4375-8a91-1ca67c8d6ab2" />

El código divide un círculo completo ($2\pi$ radianes) entre el número de lados.

* Usa Coseno para calcular la posición en el eje X.
* Usa Seno para la posición en el eje Y.
* El eje Z se deja en 0 para que la figura sea perfectamente plana.

**5. Definición de Aristas (Conexiones)**

<img width="293" height="52" alt="image" src="https://github.com/user-attachments/assets/92f70768-676d-4d74-9e37-784844364494" />

Este bucle le dice a Blender qué puntos debe unir con una línea. El símbolo % (módulo) asegura que el último punto se conecte de vuelta con el primero, cerrando la figura.

**6. Limpieza y Ejecución**
* **malla.from_pydata(...):** Toma todas las coordenadas y conexiones calculadas y las "inyecta" en el objeto de Blender.

* **bpy.ops.object.delete():** ¡Cuidado aquí! Este bloque borra todo lo que haya en tu escena de Blender antes de crear el polígono para que la vista esté limpia.

* Llamada a la función: Es donde eliges qué quieres crear. En tu imagen, está configurado para un Hexágono **(lados=6)** de tamaño 5 **(radio=5)**.

**Al ejecutar el Scrips tendremos como resultado el Polígono:**

<img width="296" height="191" alt="image" src="https://github.com/user-attachments/assets/282a0b30-017e-4f35-8eaa-1f6cde9c38a1" />

------------------------------







**Práctica 1 - Flor de vida**
--------------------------
 **Código:**
 
**1.Importación de Librerías**

<img width="87" height="31" alt="image" src="https://github.com/user-attachments/assets/e15cadd6-11c5-4944-9a41-bd668f4591d4" />

* **import bpy:** Es la librería principal de Blender (Blender Python). Sin ella, no podrías crear objetos, mover la cámara o cambiar materiales mediante código.
* **import math:** Contiene funciones matemáticas. La usamos aquí principalmente para calcular el seno (sin) y coseno (cos), necesarios para posicionar objetos en un círculo.


**2. Limpieza de la Escena**

<img width="299" height="29" alt="image" src="https://github.com/user-attachments/assets/fc71b876-0d3e-4545-9e68-889ff636b284" />

Esto es una buena práctica. Antes de crear figuras nuevas, el código selecciona todo lo que hay en la pantalla y lo borra. Así te aseguras de que tu escena esté vacía cada vez que ejecutas el script.






**3. Definición de Variables (Parámetros)**

<img width="130" height="48" alt="image" src="https://github.com/user-attachments/assets/f1d05360-c13e-454d-8489-abdb06fc1efd" />


* **radio:** Es la distancia desde el centro (0,0,0) hasta donde se colocarán los otros círculos. También es el tamaño de los círculos mismos.
* **angulo_actual:** Es el punto de partida (0 grados).
* **paso_angular:** Indica cuánto vamos a girar para poner el siguiente círculo. Como un círculo completo tiene 360°, si saltamos de 60 en 60, pondremos exactamente 6 círculos ($360 / 60 = 6$).



**4. Creación del Círculo Central**

<img width="568" height="20" alt="image" src="https://github.com/user-attachments/assets/816c39e5-9401-4837-af5c-b10dd3799bf7" />


* Esta función crea un círculo justo en el centro del mundo (0, 0, 0).

* vertices=64 hace que el círculo se vea suave y no como un polígono de pocos lados.



**5. El Cálculo Geométrico (Círculos 1 y 2)**
Aquí es donde ocurre la "magia" de las coordenadas polares:

<img width="360" height="32" alt="image" src="https://github.com/user-attachments/assets/ecaa50e4-c160-40bd-af90-912f45df96d0" />


* **math.radians(angulo_actual):** Blender/Python necesitan que los ángulos estén en radianes, no en grados. Esta función hace la conversión.

* **Coseno (cos):** Nos da la posición en el eje X.

* **Seno (sin):** Nos da la posición en el eje Y.

* Al multiplicar el resultado por el radio, obtenemos el punto exacto donde debe ir el centro del nuevo círculo para que toque perfectamente al círculo central.



**6. Actualización del Ángulo**

<img width="214" height="15" alt="image" src="https://github.com/user-attachments/assets/2bf59004-b55b-4042-8a68-3a141b3337ea" />


* Para el segundo círculo, el código suma 60 a angulo_actual. Ahora angulo_actual vale 60.

* Al repetir el cálculo de x e y con 60 grados, el nuevo círculo aparece desplazado, comenzando a formar el patrón de "flor".

**Resultado**

<img width="190" height="182" alt="image" src="https://github.com/user-attachments/assets/26198881-46d8-4774-88a9-3017b04b0330" />

---

 **Código con inicion del ciclo while:**

<img width="709" height="457" alt="image" src="https://github.com/user-attachments/assets/90d6e124-45f6-4a2e-b4a0-b588c12a04ab" />

---

**1. El "Interruptor" del Ciclo (while)**

La línea ```while angulo_actual < 360:``` es el corazón del código. Funciona como una pregunta constante:

- **Pregunta:** "¿El ángulo actual es menor a 360?"

- **Si la respuesta es SÍ:** Ejecuta todo el bloque de código que está indentado (hacia la derecha).

- **Si la respuesta es NO:** Detente y termina el programa.

**2. El Cálculo Matemático (Posicionamiento)**

Dentro del ciclo, el código calcula dónde poner el siguiente círculo usando coordenadas polares:

- ```math.radians(angulo_actual)```: Convierte tus grados (0°, 60°, 120°...) a una unidad que la computadora entiende para calcular curvas.

- ```radio * math.cos(...)```: Calcula la distancia en el eje **X**.

- ```radio * math.sin(...)```: Calcula la distancia en el eje **Y**.

Esto asegura que cada círculo nuevo se coloque exactamente sobre el borde del círculo central, girando alrededor de él.

**3. La Ejecución en Blender**

```bpy.ops.mesh.primitive_circle_add(...)```:

Esta es la orden de construcción. Usa los resultados de **X** e **Y** que calculamos arriba para colocar el círculo en la escena 3D. Como está dentro del ciclo, Blender recibirá esta orden 6 veces seguidas en milisegundos.

**4. El "Paso" hacia adelante (Actualización)**

La línea ```angulo_actual += paso_angular``` es la más importante para el control:

- **Primera vuelta:** El ángulo es 0°. Al terminar, le suma 60. Ahora es 60°.

- **Segunda vuelta:** El ángulo es 60°. Al terminar, suma 60. Ahora es 120°.

- ... así sucesivamente hasta llegar a 360°.

---

**Resultado**


<img width="268" height="239" alt="image" src="https://github.com/user-attachments/assets/77b23db2-9ae4-4aef-bf2e-4c9931a2bc47" />

---

## 1.6 Procesamiento de mapas de bits
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

---

## Bibliografías APA

- Sutori. (s. f.). Sutori. https://www.sutori.com/es/historia/historia-y-evolucion-de-la-graficacion-por-computadora--HWxiLPJRpHqkjwYoadxpmheZ

- Client challenge. (s. f.). https://es.slideshare.net/slideshow/1-2-areas-de-aplicacion-de-la-graficacion-por-computadora-pdf/282295469

- Client challenge. (s. f.-b). https://es.slideshare.net/slideshow/1-3-aspectos-matematicos-de-la-graficacion-pdf/282295700

- Modelos de color RGB, CMY, HSV y HSL. (s. f.). https://graficaciontmmjc.blogspot.com/2019/03/modelos-de-color-rgb-cmy-hsv-y-hsl.html

- Client challenge. (s. f.-c). https://es.slideshare.net/slideshow/1-6-procesamiento-de-mapas-de-bits-en-graficacion/282295902

