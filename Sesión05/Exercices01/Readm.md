Ejercicio: Menú Responsive con HTML y CSS

Descripción del proyecto

Este proyecto consiste en crear un menú de navegación responsive utilizando HTML y CSS.

El menú contiene el logo de Instagram y tres iconos: Home, Settings y Logout.

El objetivo es que el menú se adapte al tamaño de la pantalla:

En pantallas grandes, los elementos aparecen en horizontal.

Cuando se reduce el ancho de la ventana, los iconos van pasando progresivamente a nuevas filas.

El fondo marrón se mantiene en todas las filas.

Los iconos conservan su tamaño.

Al pasar el ratón por encima de los elementos, se aplica un efecto hover.

Tecnologías utilizadas

HTML5: estructura del menú de navegación.

CSS3: diseño, colores, tamaños y distribución de los elementos.

Flexbox: organización y adaptación de los elementos.

Imágenes: logo de Instagram e iconos de navegación.

Propiedades CSS utilizadas

Algunas de las propiedades principales utilizadas son:

display: flex: activa el sistema Flexbox.

flex-wrap: wrap: permite que los elementos pasen a otra fila cuando no hay suficiente espacio.

flex-direction: column: organiza los elementos verticalmente.

justify-content: controla la distribución horizontal de los elementos.

align-items: controla su alineación.

margin y padding: controlan los espacios exteriores e interiores.

width y height: establecen las dimensiones.

background-color: establece los colores de fondo.

:hover: aplica cambios visuales al pasar el ratón por encima.

Diseño y colores

Se utilizan cuatro variables CSS para definir los colores del proyecto:

--primary-color: color principal.

--second-color: fondo rosa claro.

--third-color: marrón del menú.

--fourth-color: marrón oscuro utilizado para el efecto hover.

Comportamiento responsive

El menú utiliza Flexbox y la propiedad flex-wrap: wrap para adaptarse al ancho disponible.

De esta manera, los elementos no desaparecen al reducir la pantalla, sino que se reorganizan en diferentes filas.

Autor

Ejercicio práctico de HTML y CSS.