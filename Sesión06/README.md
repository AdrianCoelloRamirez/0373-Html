Fase 2: Ajustes de Layout y Rejilla Flexible

Este repositorio contiene la documentación de la Fase 2 del proyecto de maquetación con CSS Grid. En esta etapa se refina la maquetación general agregando márgenes de encuadre en el cuerpo (body), ajustando los espacios entre celdas (gap) y reestructurando la segunda rejilla para 3 columnas responsivas.

🛠️ Cambios e Implementaciones en la Fase 2

A diferencia de la Fase 1, en esta etapa se introducen los siguientes cambios clave en main.css:

Encuadre General del Documento (body):

Se añade un espaciado interno amplio al body mediante padding: 0 10rem 35rem 10rem; para centrar visualmente el contenido y otorgarle margen inferior de desplazamiento.

Ajuste de la Rejilla Secundaria (.grid-container-2):

Se modifica el número de columnas de 5 a 3 columnas flexibles: grid-template-columns: repeat(3, minmax(0, 1fr));.

Se amplía la separación entre elementos dentro de esta segunda rejilla aumentando el gap a 20px.

Simplificación de Rellenos Internos (.sub-item):

Se unifica el padding de los subelementos a un valor limpio de 1rem, eliminando las reglas duplicadas previas.

📁 Estructura del Archivo CSS (main.css)

* {
  box-sizing: border-box;
}

h1 {
  font-size: 1.5em;
  font-weight: bold;
}

body {
  padding: 0 10rem 35rem 10rem;
}

.grid-item {
  background-color: lightsalmon;
  padding: 3rem;
}

.sub-item {
  background-color: rgb(253, 213, 197);
  padding: 1rem;
}

.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  gap: 5px;
}

.item-1 {
  grid-column: 1 / 4;
}

.item-5 {
  grid-column: 1 / 4;
}

.grid-container-2 {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 20px;
  margin-top: -0.2rem;
}


🚀 Instrucciones de Uso

Posicionarse en la rama feat/fase-2 mediante git checkout feat/fase-2.

Visualizar los cambios en el navegador con Live Server o abriendo directamente index.html.