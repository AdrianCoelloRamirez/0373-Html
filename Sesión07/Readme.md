🎮 Formulario de Inscripción - Twitch Rivals 2026

Proyecto web desarrollado con HTML5 y CSS3 puros (Vanilla) que implementa un formulario de registro responsivo y accesible para una competición de esports inspirada en Twitch Rivals.

📋 Características y Requisitos Cumplidos

1. Estructura y Validación HTML5

Semántica estructurada: Uso correcto de <form>, <fieldset>, <legend> y <label> vinculados mediante atributos for, id y name.

Campos incluidos:

Datos personales: Nombre completo, Correo electrónico (validación nativa type="email"), Nickname (entre 3 y 15 caracteres), Contraseña (8 a 20 caracteres), Edad (mínimo 16 años) y Fecha de nacimiento.

Detalles de competición: Selector de videojuego (<select>), Plataforma de selección única (radio), Disponibilidad horaria de selección múltiple (checkbox) y Comentarios adicionales (<textarea>).

Legal: Casilla obligatoria de aceptación de normas vinculada a la página externa normas.html (configurada para abrirse en una pestaña nueva sin perder los datos introducidos).

Controles nativos: Botones funcionales de envío (type="submit") y limpieza de formulario (type="reset").

2. Diseño y Estilos CSS3

Diseño Responsivo (Responsive): Contenedor principal centrado con Flexbox y anchura adaptable (width: 100% y max-width: 600px) junto con opciones flexibles (flex-wrap: wrap).

Estética Dark & Lilac: Fondo de pantalla completo con imagen temática fija (background-size: cover) y tarjeta principal con bordes redondeados y paleta de colores oscura con acentos lila/lavanda (#a78bfa).

Interactividad y Estados:

Efecto :focus luminoso en los campos de entrada para destacar el elemento activo.

Efectos :hover personalizados en botones principales y opciones de selección.

Selectores estructurales (:first-child y :nth-child(2)) para mantener el código HTML limpio de clases innecesarias.

📁 Estructura del Proyecto

├── index.html          # Página principal con el formulario de inscripción
├── normas.html         # Página secundaria con los Términos y Condiciones (ToS)
├── Css/
│   └── style.css       # Hoja de estilos principal (Vanilla CSS)
└── README.md           # Documentación del proyecto


🚀 Cómo ejecutar el proyecto

Descarga o clona los archivos manteniendo la estructura de carpetas.

Abre el archivo index.html en cualquier navegador web moderno (Chrome, Firefox, Edge, Safari).

No requiere instalación de dependencias, servidores ni frameworks externos.