# Laboratorio SAT · Separating Axis Theorem (2D & 3D)

Visualizador interactivo en tiempo real para explorar el **Teorema del Eje Separador (Separating Axis Theorem - SAT)** en dos y tres dimensiones con representación vectorial de ejes locales, productos cruzados y proyecciones ortogonales escalares por producto punto.

🌐 **Demo en línea**: [https://wosdan.github.io/visualizador-sat/](https://wosdan.github.io/visualizador-sat/)

---

## 🚀 Características y Novedades

- **Vectores de Ejes en las Figuras:**
  - **En 3D:** Cada caja orientada (OBB) despliega sus tres ejes principales locales ($X, Y, Z$) con flechas vectoriales codificadas por color, destacando en amarillo dorado el eje que interviene en la prueba activa.
  - **En 2D:** Muestra los ejes de orientación locales en el centroide y las normales exteriores en cada arista del polígono.

- **Visualización Geométrica del Producto Cruz ($\vec{u} \times \vec{v}$):**
  - Identifica y resalta el vector director de arista $\vec{u}$ en la Figura A y $\vec{v}$ en la Figura B.
  - Construye en el centro del espacio el paralelogramo que generan $\vec{u}$ y $\vec{v}$.
  - Dibuja el **vector resultante del producto cruz** $\vec{C} = \vec{u} \times \vec{v}$ (y su normalizado $\vec{n} = \frac{\vec{C}}{\|\vec{C}\|}$) con flecha verde esmeralda y marca de ángulo recto ($\perp$).

- **Proyección mediante Producto Punto ($\vec{v}_k \cdot \vec{n}$):**
  - Muestra en el espacio 3D las líneas de proyección ortogonales desde los 8 vértices de cada caja hacia la recta del eje.
  - Genera los intervalos continuos $[\min_A, \max_A]$ y $[\min_B, \max_B]$ directamente en 3D y en la gráfica inferior.

- **Consola Matemática Detallada:**
  - Desglose componente a componente del producto cruz y del producto punto con verificación de condición de solapamiento estricto.

---

## 🎮 Controles

| Acción | Control |
|---|---|
| **Mover figuras** | Clic y arrastrar sobre la figura deseada |
| **Rotar figura B** | Deslizador "Rotar B" en la barra de herramientas |
| **Inspeccionar eje** | Clic en cualquier botón del listado derecho |
| **Siguiente eje** | Botón "Siguiente eje →" |
| **Alternar vectores de ejes** | Botón "Ejes en figuras: ON/OFF" |
| **Alternar proyecciones 3D** | Botón "Proyecciones 3D: ON/OFF" |
| **Orbitar cámara (3D)** | Clic derecho o arrastrar fondo |
| **Zoom cámara (3D)** | Rueda del ratón |
| **Restablecer escena** | Botón "Restablecer" |

---

## 🛠️ Tecnologías

- **HTML5 Canvas 2D** acelerado por hardware con escalado HiDPI (`devicePixelRatio`).
- **JavaScript Moderno (ES6+)** con álgebra vectorial pura sin librerías externas.
- **CSS3 Dark Theme** responsivo.
