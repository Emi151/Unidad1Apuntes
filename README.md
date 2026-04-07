# Unidad1Apuntes
Apuntes de la unidad 1 de graficacioón 

# 1.1 Historia y evolución de la graficación por computadora
<p> La graficación por computadora es una disciplina que combina informática, matemáticas y percepción visual para generar, 
manipular y representar imágenes mediante sistemas computacionales.</p>
<p></p>Su evolución está profundamente ligada al desarrollo del hardware y de los algoritmos matemáticos.</p>
<p>📌 Orígenes (1950 – 1960)</p>
Durante esta etapa, los gráficos eran extremadamente básicos debido a las limitaciones del hardware.
Características:
✔ Gráficos vectoriales
✔ Pantallas monocromáticas
✔ Aplicaciones militares y científicas
Uno de los hitos más importantes fue:
Sketchpad (1963)
Considerado el precursor del diseño asistido por computadora (CAD). Introdujo:
* Manipulación interactiva
* Uso del mouse
* Representación geométrica

📌 Consolidación (1970 – 1980)
Aquí se desarrollan los algoritmos fundamentales que aún se estudian hoy.
Avances clave:
✔ Algoritmos de rasterización
✔ Representación de polígonos
✔ Relleno de áreas

Ejemplos importantes:
* Algoritmo de Bresenham → trazado eficiente de líneas
* Algoritmo DDA → aproximación incremental
También surge el concepto de:
✔ Mapas de bits (gráficos raster)

📌 Revolución 3D (1980 – 1990)
Con el aumento de potencia computacional:
✔ Aparición de gráficos tridimensionales
✔ Renderizado básico
✔ Simulación de iluminación
Industria impactada:
✔ Videojuegos
✔ Cine digital
✔ CAD avanzado

📌 Era moderna (1990 – actualidad)
Avances determinantes:
✔ GPUs dedicadas
✔ Ray tracing
✔ Shaders programables
✔ Realidad virtual / aumentada

Aplicaciones actuales:
✔ Simulación física
✔ Visualización científica
<p>✔ Motores graficos en tiempo real</p>

# 1.2 Áreas de aplicación
La graficación por computadora es transversal a numerosas disciplinas.
🎮 Videojuegos
✔ Renderizado en tiempo real
✔ Simulación de físicas
✔ Animación interactiva
🎬 Cine y animación
✔ Efectos visuales (VFX)
✔ Modelado 3D
✔ Iluminación realista
🏗 Arquitectura e ingeniería
✔ Visualización de estructuras
✔ Simulación de materiales
✔ Diseño CAD

🧬Medicina
✔ Reconstrucciones 3D
✔ Imágenes médicas (MRI, CT)
✔ Simulación quirúrgica

📊 Visualización de datos
✔ Gráficos estadísticos
✔ Simulación científica
✔ Interfaces interactivas

# 1.3 Aspectos matemáticos de la graficación
Las matemáticas son la base conceptual y operativa de toda representación gráfica.

📌 Álgebra Lineal
Esencial para gráficos 2D y 3D.
Conceptos clave:
✔ Vectores
✔ Matrices
✔ Transformaciones lineales

Transformaciones comunes:
*Traslación
*Rotación
*Escalamiento
Ejemplo:
Una rotación en 2D:
[x' = x \cos(\theta) - y \sin(\theta)]
[y' = x \sin(\theta) + y \cos(\theta)]

📌 Geometría Analítica
Permite representar:
✔ Líneas
✔ Planos
✔ Curvas
Ejemplo de línea:
[y = mx + b]

📌 Trigonometría
✔ Rotaciones
✔ Proyecciones
✔ Cámaras virtuales

📌 Cálculo
✔ Curvas suaves
✔ Superficies
✔ Iluminación avanzada

Ejemplo:
Interpolación de curvas Bézier.

# 1.4 Modelos del color
Los modelos de color describen cómo se representan y combinan los colores.
🎨 RGB (Modelo Aditivo)
Basado en luz.
✔ Rojo
✔ Verde
✔ Azul
Características:
✔ Usado en pantallas
✔ Negro = ausencia de luz
✔ Blanco = suma total

🎨 CMY (Modelo Sustractivo)**
Basado en pigmentos.
✔ Cian
✔ Magenta
✔ Amarillo
Caracteristicas: 
✔ Usado en impresión

🎨 HSV
Representación más intuitiva:
✔ Hue → tono
✔ Saturation → intensidad
✔ Value → brillo
Muy usado en edición gráfica.

🎨 HSL
Similar a HSV, pero enfocado en luminosidad:
✔ Hue
✔ Saturation
✔ Lightness

Iluminación básica de un cubo
La iluminación es crucial para percepción de volumen y realismo.
1️⃣ Crear objeto
`Shift + A → Mesh → Cube`
2️⃣ Añadir fuente de luz
`Shift + A → Light`
Tipos comunes:
✔ Point → omnidireccional
✔ Sun → luz uniforme
✔ Area → iluminación suave
3️⃣ Parámetros importantes
✔ Energy → intensidad
✔ Color → tonalidad
4️⃣ Principio de iluminación
Modelo clásico:
✔ Key Light → luz principal
✔ Fill Light → reduce sombras
✔ Back Light → separa del fondo

# 1.5 Representación y trazo de líneas y polígonos
📏 Representación de líneas
Una línea se define mediante dos puntos:
[P_1(x_1, y_1), \quad P_2(x_2, y_2)]
Problema principal:
✔ Convertir ecuaciones continuas → píxeles discretos

📌 Algoritmo de Bresenham
Objetivo:
✔ Minimizar operaciones costosas
✔ Evitar números flotantes
Ventajas:
✔ Alta eficiencia
✔ Precisión en rasterización

🔷 Polígonos
Definidos por:
✔ Vértices
✔ Aristas

Operaciones fundamentales:
✔ Relleno
✔ Clipping
✔ Transformación

📌 Relleno de polígonos
Problema:
✔ Determinar qué píxeles pertenecen al interior.

Métodos:
✔ Scanline
✔ Flood Fill

# 1.6 Procesamiento de mapas de bits
Definición
Una imagen raster es una matriz de píxeles.
Cada píxel almacena:
✔ Información de color
✔ Intensidad

📌 Resolución
Mayor resolución:
✔ Más detalle
✔ Mayor costo computacional

📌 Operaciones comunes
✔ Escalamiento
✔ Rotación
✔ Recorte
✔ Filtros

📌 Problemas típicos**
Aliasing
✔ Bordes dentados

Solución:
✔ Antialiasing

Filtros de imagen**
✔ Suavizado (Blur)
✔ Nitidez (Sharpen)
✔ Detección de bordes

Aplicaciones:
✔ Mejora visual
✔ Procesamiento digital

📌 Transformaciones
✔ Interpolación
✔ Re-muestreo

Métodos:
✔ Vecino más cercano
✔ Bilineal
✔ Bicúbica

# Unidad2Apuntes

# **2.1 Transformación bidimensional**

<p>Son operaciones matemáticas que permiten **modificar la posición, tamaño o forma** de objetos en un plano 2D (ejes X y Y).
Se aplican mucho en animación, videojuegos, interfaces y diseño gráfico.</p>

## **2.1.1 Traslación**

<p>Es el **desplazamiento** de un objeto de un lugar a otro sin cambiar su forma ni tamaño.</p>

* Se mueve en X y en Y.
* Fórmula:
  [
  x' = x + t_x,\quad y' = y + t_y
  ]

📌 Ejemplo: mover un personaje 5 unidades a la derecha.

---

## **2.1.2 Escalamiento**

Consiste en **cambiar el tamaño** del objeto.

* Puede ser:

  * Uniforme (misma escala en X y Y)
  * No uniforme (distinta escala)

[
x' = x \cdot s_x,\quad y' = y \cdot s_y
]

📌 Ejemplo: agrandar una imagen al doble.

---

## **2.1.3 Rotación**

Es girar un objeto respecto a un punto (normalmente el origen).

[
x' = x\cos\theta - y\sin\theta
]
[
y' = x\sin\theta + y\cos\theta
]

📌 Ejemplo: rotar un sprite 90°.

---

## **2.1.4 Sesgado (Shear)**

Deforma el objeto inclinándolo.

* En X:
  [
  x' = x + sh_x \cdot y
  ]

* En Y:
  [
  y' = y + sh_y \cdot x
  ]

📌 Ejemplo: convertir un rectángulo en un paralelogramo.

---

# **2.2 Representación matricial de las transformaciones bidimensionales**

Todas las transformaciones anteriores se pueden representar con **matrices**, lo que facilita combinarlas.

Se usa mucho el sistema de **coordenadas homogéneas** (agregando un 1):

[
\begin{bmatrix}
x' \ y' \ 1
\end{bmatrix}
=============

\begin{bmatrix}
a & b & t_x \
c & d & t_y \
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
x \ y \ 1
\end{bmatrix}
]

📌 Ventajas:

* Puedes aplicar varias transformaciones con una sola multiplicación.
* Es más eficiente en gráficos por computadora.

---

# **2.3 Trazo de líneas curvas**

Permite dibujar curvas suaves en lugar de líneas rectas.

---

## **2.3.1 Bézier**

Son curvas definidas por **puntos de control**.

* Muy usadas en diseño gráfico y animación.
* Tipos:

  * Lineal (2 puntos)
  * Cuadrática (3 puntos)
  * Cúbica (4 puntos)

Fórmula general:
[
B(t) = \sum_{i=0}^{n} P_i \cdot B_{i,n}(t)
]

📌 Características:

* Suavidad
* Fácil control de forma
* Usadas en software como Illustrator

---

## **2.3.2 B-spline**

Son una generalización de las curvas Bézier.

📌 Características:

* Más flexibles
* Mejor control local (mover un punto no afecta toda la curva)
* Más suaves para modelado complejo

📌 Uso:

* Modelado 3D
* Animación
* CAD

---

# **2.4 Fractales**

Son figuras geométricas que se repiten a diferentes escalas (auto-similitud).

📌 Características:

* Infinitos detalles
* Generados por funciones matemáticas
* Muy usados en gráficos realistas

📌 Ejemplos:

* Conjunto de Mandelbrot
* Árboles fractales

📌 Aplicaciones:

* Videojuegos (paisajes)
* Animaciones
* Simulación de naturaleza

---

# **2.5 Uso y creación de fuentes de texto**

Se refiere a cómo se representan y diseñan letras en gráficos.

📌 Tipos:

* **Bitmap**: píxeles fijos
* **Vectoriales**: escalables sin perder calidad

📌 Tecnologías comunes:

* TrueType
* OpenType

📌 Uso en graficación:

* Interfaces gráficas
* Videojuegos
* Diseño UI/UX

📌 Creación:

* Se diseñan con curvas (generalmente Bézier)
* Se definen puntos, trazos y rellenos

---

# ✨ RESUMEN GENERAL

<p>* Transformaciones → modifican objetos (mover, girar, escalar)</p>
<p>* Matrices → permiten aplicar transformaciones fácilmente</p>
<p>* Curvas → generan formas suaves (Bézier y B-spline)</p>
* Fractales → crean estructuras complejas repetitivas
* Fuentes → representación gráfica de texto
