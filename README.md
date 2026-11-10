# Laboratorio SAT · Separating Axis Theorem (2D & 3D)

Visualizador interactivo en tiempo real para explorar el **Teorema del Eje Separador (Separating Axis Theorem - SAT)** en dos y tres dimensiones.

🌐 **Demo en línea**: [https://wosdan.github.io/visualizador-sat/](https://wosdan.github.io/visualizador-sat/)

---

## 🚀 Características

- **Modo 2D:**
  - Polígonos convexos arbitrarios con traslación y rotación en tiempo real.
  - Generación dinámica de normales a partir de las aristas de ambas figuras.
  - Proyección ortogonal de los vértices sobre el eje seleccionado con visualización de intervalos mínimos/máximos.
  - Indicador visual inmediato de separación (verde) o solapamiento (rojo).

- **Modo 3D Isométrico:**
  - Cajas orientadas en el espacio (OBB - Oriented Bounding Boxes).
  - Evaluación de hasta 15 ejes potenciales:
    - 3 normales de caras para la figura A.
    - 3 normales de caras para la figura B.
    - Hasta 9 ejes generados por el producto cruzado de los pares de aristas ($A_i \times B_j$).
  - Cámara orbital libre con ratón/touch (paneo, rotación y zoom mediante scroll).
  - Gráfica inferior de proyecciones escalares por producto punto ($v \cdot n$).

- **Consola Matemática en Vivo:**
  - Muestra el vector unitario $n$, los cálculos de proyecciones escalares individuales, intervalos $[\min_A, \max_A]$ y $[\min_B, \max_B]$, y el criterio de separación estricto con tolerancia epsilon ($10^{-8}$).

---

## 🎮 Controles

| Acción | Control |
|---|---|
| **Mover figuras** | Clic y arrastrar sobre la figura deseada |
| **Rotar figura B** | Deslizador "Rotar B" en la barra de herramientas |
| **Inspeccionar eje** | Clic en cualquier botón del listado derecho |
| **Siguiente eje** | Botón "Siguiente eje →" |
| **Orbitar cámara (3D)** | Clic derecho y arrastrar o arrastrar el fondo |
| **Zoom cámara (3D)** | Rueda del ratón |
| **Restablecer escena** | Botón "Restablecer" |

---

## 🛠️ Tecnologías

- **HTML5 Canvas 2D** acelerado por hardware con escalado HiDPI (`devicePixelRatio`).
- **JavaScript Moderno (ES6+)** sin dependencias externas ni frameworks pesados.
- **CSS3 Dark Theme** responsivo con variables personalizadas y tipografía nativa del sistema.
