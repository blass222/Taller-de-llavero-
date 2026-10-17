# 🔑 Taller de Llaveros 3D

Generador web interactivo que convierte cualquier imagen (PNG, JPG o WebP) en un modelo 3D multicolor listo para imprimir (`.3mf`) o en una vista previa en alta resolución (`.png`). Todo el procesamiento ocurre directamente en el navegador, sin subir archivos a ningún servidor.

## ✨ Características principales

* **Cuantización automática de color:** Reduce la imagen de 2 a 8 colores mediante clustering (K-means) y permite editar, ocultar o ajustar cada color de forma individual.
* **Alturas independientes por color:** Toca cualquier color en el lienzo 2D para asignarle una altura de capa personalizada (ideal para sistemas multimaterial como AMS o cambios de filamento por altura de capa).
* **Eliminación automática de fondo:** Detecta y recorta el fondo de la imagen con un clic.
* **Múltiples formatos y accesorios:**
  * **Hook:** Pestaña superior con argolla.
  * **Hole:** Orificio integrado directamente en la silueta.
  * **Bookmark:** Clip marcapáginas integrado en la base inferior.
  * **Cake Toppers (1 o 2 palitos):** Pinches configurables de 30 a 120 mm para decoración de tortas.
* **Formas de base personalizables:** Contorno adaptable a la figura, círculo, cuadrado redondeado o corazón.
* **Vista previa 2D y 3D interactiva:** Renderizado en tiempo real con sombras en 2D y visualización tridimensional interactiva mediante Three.js.
* **Exportación directa a `.3mf`:** Genera mallas optimizadas por rectángulos con objetos separados por color, listas para abrir en **Bambu Studio**, **OrcaSlicer**, **PrusaSlicer** o **Creality Print**.

## 🚀 Cómo usarlo

1. Abre la aplicación en tu navegador (o simplemente abre el archivo `index.html`).
2. **Sube o arrastra** tu imagen en el panel izquierdo.
3. Ajusta la **cantidad de colores**, el **borde**, el **tipo de colgador** y las **dimensiones en milímetros**.
4. *(Opcional)* Haz clic sobre las zonas de color en la vista 2D para modificar su grosor individualmente, o cambia a la vista **3D** para inspeccionar el relieve.
5. Presiona **Descargar 3D (.3mf)** e impórtalo directamente en tu laminador favorito.

## 🛠️ Tecnologías utilizadas

* HTML5 Canvas API (procesamiento de píxeles y cuantización K-means).
* Generador nativo de archivos comprimidos ZIP / `.3mf` en JavaScript puro (sin dependencias externas para exportar).
* [Three.js](https://threejs.org/) (r128) para la previsualización 3D interactiva.
* 
