# Unidad1Apuntes
<p>puntes de la unidad 1 de graficación</p>
# 1.1 Historia y evolución de la graficación por computadora
La graficación por computadora es una disciplina que combina informática, matemáticas y percepción visual para generar, 
manipular y representar imágenes mediante sistemas computacionales.
Su evolución está profundamente ligada al desarrollo del hardware y de los algoritmos matemáticos.
📌 Orígenes (1950 – 1960)
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
✔ Motores gráficos en tiempo real

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
