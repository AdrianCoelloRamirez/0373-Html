Fase 1: Introducción a CSS Grid Layout

Este repositorio contiene la solución correspondiente a la Fase 1 del proyecto de maquetación con CSS Grid. En esta etapa se establecen la estructura base del diseño, el comportamiento responsivo básico de las cuadrículas y las reglas globales de estilo.

🛠️ Conceptos y Estilos Implementados

En esta fase se trabajaron los siguientes aspectos técnicos en main.css:

Reinicio de Caja Global:

Implementación del modelo de caja universal con box-sizing: border-box; para un control preciso de bordes y márgenes internos.

Tipografía y Elementos Base:

Configuración de estilos para los encabezados principales (h1) asignando tamaño (1.5em) y peso tipográfico destacado (bold).

Contenedores Principales en Grid:

.grid-container: Definición de una rejilla de tres columnas mediante grid-template-columns: 1fr 2fr 1fr; con un espaciado intermedio (gap) de 5px.

.grid-container-2: Configuración de una rejilla flexible de 5 columnas idénticas usando la función repeat(5, minmax(0, 1fr)); y un espacio entre celdas de 1rem.

Posicionamiento y Extensión de Elementos (Grid Columns):

Extensión horizontal completa de elementos destacados (.item-1 y .item-5) a lo largo de las 3 columnas del primer contenedor utilizando grid-column: 1 / 4;.

Estilos Visuales:

Uso de colores de fondo temáticos (lightsalmon e rgb(253, 213, 197)) y rellenos proporcionales (padding) para distinguir áreas principales y subelementos (.grid-item y .sub-item).

Fase Avanzada: Reset Global, Alineaciones y Rejilla Compleja

Este repositorio contiene la documentación de la Fase Avanzada del proyecto de maquetación con CSS Grid. En esta iteración se implementa un reset global de márgenes, alineaciones individuales dentro de la rejilla principal y la reestructuración de la rejilla secundaria a 5 columnas.

🛠️ Cambios e Implementaciones en la Fase Avanzada

En esta fase final se aplican las siguientes mejoras y refinamientos en main.css:

Reset Global de Estilos (*):

Se añade margin: 0; y padding: 0; junto con box-sizing: border-box; para eliminar márgenes predeterminados del navegador y asegurar una maquetación consistente.

Alineación Individual (.item-4):

Se añade align-self: flex-end; al cuarto elemento de la rejilla principal para alinear la celda hacia el borde inferior de su contenedor grid.

Ajuste Fino de Sub-ítems (.sub-item):

Se reduce el espacio interno a padding: 0.8rem; y se compensa el margen con margin-top: -0.3rem;.

Rejilla Secundaria Expandida (.grid-container-2):

Se establece la rejilla a 5 columnas de ancho equivalente: grid-template-columns: repeat(5, minmax(0, 1fr));.

Se ajusta la separación entre celdas a un valor de gap: 17px;.

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
  grid-template-columns: repeat(5, minmax(0, 1fr));
  gap: 20px;
  margin-top: -0.2rem;
}


🚀 Instrucciones de Uso

Clonar el repositorio localmente o cambiar a la rama feat/fase-1.

Abrir el archivo index.html en el navegador o mediante la extensión Live Server de Visual Studio Code para visualizar la estructura en rejilla.

Cambiar a la rama avanzada mediante git checkout feat/advanced (o hazaña/avanzado).

Abrir index.html en el navegador para comprobar el comportamiento del maquetado Grid final.

Posicionarse en la rama feat/fase-2 mediante git checkout feat/fase-2.

Visualizar los cambios en el navegador con Live Server o abriendo directamente index.html.

