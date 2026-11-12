# Laboratorio SAT · Separating Axis Theorem (2D & 3D)

Visualizador interactivo en tiempo real para explorar y calcular matemáticamente el **Teorema del Eje Separador (Separating Axis Theorem - SAT)** sobre un plano cartesiano graduado con coordenadas explícitas, productos cruzados y proyecciones por producto punto.

🌐 **Demo en línea**: [https://wosdan.github.io/visualizador-sat/](https://wosdan.github.io/visualizador-sat/)

---

## 🚀 Características Matemáticas

- **Plano Cartesiano Graduado (2D y 3D):**
  - **En 2D:** Ejes principales horizontal ($X$) y vertical ($Y$) con marcas graduadas cada 50 unidades, origen $(0, 0)$ y flechas de orientación.
  - **En 3D:** Espacio cartesiano tridimensional con plano de tierra graduado en $Y = 0$, ejes globales $+X$ (rojo), $+Y$ (verde) y $+Z$ (azul) con valores numéricos visibles en los tres ejes y origen $(0, 0, 0)$.

- **Valores Numéricos Visibles para Cálculo Manual:**
  - **Centros de figuras:** Coordenadas cartesianas en vivo $(X, Y)$ en 2D y $[X, Y, Z]$ en 3D.
  - **Vértices:** Cada vértice de las Figuras A y B muestra su etiqueta y coordenadas exactas (ej: $P_1(-88, -54)$ o $v_1[-1.60, 0.86, -0.35]$).
  - **Vectores de Ejes y Aristas:** Muestran sus componentes $(\Delta x, \Delta y)$ y vector unitario $\vec{n} = (n_x, n_y)$.
  - **Producto Cruz:** Componentes explícitos de $\vec{u}$, $\vec{v}$, $\vec{C} = \vec{u} \times \vec{v}$, magnitud $\|\vec{C}\|$ y normalizado $\vec{n}$.
  - **Proyecciones Escalares:** Cada punto proyectado sobre el eje muestra su valor escalar $p = \vec{v} \cdot \vec{n}$, así como los límites del intervalo $[\min_A, \max_A]$ y $[\min_B, \max_B]$.

- **Consola Matemática Paso a Paso:**
  - Desglose aritmético explícito: multiplica cada componente del vértice por el vector del eje y suma los términos para verificar manualmente con lápiz y papel o calculadora.

---

## 🎮 Controles

| Botón / Control | Descripción |
|---|---|
| **Plano cartesiano: ON/OFF** | Alterna los ejes coordenados y marcas graduadas de la grilla |
| **Valores numéricos: ON/OFF** | Alterna las coordenadas $(x, y, z)$ en vértices, centros y proyecciones |
| **Ejes figuras: ON/OFF** | Muestra los ejes de rotación local en el centro de las figuras |
| **Proyecciones 3D: ON/OFF** | Muestra los rayos ortogonales e intervalos de sombra en 3D |
| **Arrastrar figura** | Clic izquierdo y arrastrar para mover libremente por el plano |
| **Rotar B** | Deslizador angular de $-180^\circ$ a $180^\circ$ |
| **Orbitar cámara (3D)** | Clic derecho o arrastrar fondo |
| **Zoom cámara (3D)** | Rueda del ratón |
| **Siguiente eje →** | Recorre los ejes potenciales de colisión |

---

## 🛠️ Tecnologías

- **HTML5 Canvas 2D** acelerado por hardware con escalado HiDPI (`devicePixelRatio`).
- **JavaScript ES6+** con álgebra lineal y cálculo analítico sin librerías externas.
- **CSS3 Dark Theme** responsivo.
