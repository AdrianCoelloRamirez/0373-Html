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

📁 Estructura del Archivo CSS (main.css)

* {
  box-sizing: border-box;
}

h1 {
  font-size: 1.5em;
  font-weight: bold;
}

.grid-item {
  background-color: lightsalmon;
  padding: 3rem;
}

.sub-item {
  background-color: rgb(253, 213, 197);
  padding: 1rem;
  padding-right: 2rem;
  padding: 0.5rem;
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
  gap: 1rem;
  margin-top: -0.2em;
}


🚀 Instrucciones de Uso

Clonar el repositorio localmente o cambiar a la rama feat/fase-1.

Abrir el archivo index.html en el navegador o mediante la extensión Live Server de Visual Studio Code para visualizar la estructura en rejilla.