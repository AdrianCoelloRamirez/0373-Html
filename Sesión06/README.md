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

📁 Estructura del Archivo CSS (main.css)

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
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
  padding: 0.8rem;
  margin-top: -0.3rem;
}

.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  gap: 5px;
}

.item-1 {
  grid-column: 1 / 4;
}

.item-4 {
  align-self: flex-end;
}

.item-5 {
  grid-column: 1 / 4;
}

.grid-container-2 {
  display: grid;
  grid-template-columns: repeat(5, minmax(0, 1fr));
  gap: 17px;
}


🚀 Instrucciones de Uso

Cambiar a la rama avanzada mediante git checkout feat/advanced (o hazaña/avanzado).

Abrir index.html en el navegador para comprobar el comportamiento del maquetado Grid final.