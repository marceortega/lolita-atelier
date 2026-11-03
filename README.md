# Lolita Atelier

Prototipo visual de una boutique ficticia de delantales vintage. Todo el contenido está en español. No incluye compras, carrito, formularios ni páginas de detalle.

## Cómo abrir la página

Abre `index.html` con doble clic o desde el menú «Abrir archivo» de tu navegador. No necesitas instalar paquetes ni iniciar un servidor. Todos los recursos están guardados localmente y funcionan sin conexión.

## Tecnologías y estructura

- `index.html`: HTML5 semántico, secciones y catálogo de seis productos.
- `css/styles.css`: CSS3, variables de color, cuadrículas y adaptación a computador, tablet y celular.
- `images/delantal.svg`: ilustración vectorial local de referencia, creada para este prototipo. No es una fotografía de un producto real.

No se utiliza JavaScript, frameworks, bibliotecas, fuentes externas ni backend. El SVG es un recurso gráfico estático.

## Modificar colores

Edita las variables del bloque `:root` al principio de `css/styles.css`: `--rose`, `--cream`, `--white`, `--sage` y `--brown`. `--ink` y `--muted` definen colores oscuros para mantener legibles los textos. Comprueba el contraste al cambiarlos.

## Agregar productos

Duplica un bloque `<article class="product">` dentro de `.product-grid`. Cambia el nombre, la descripción, el precio, la etiqueta y el atributo `alt` de la imagen. La cuadrícula distribuye automáticamente las nuevas tarjetas. «Ver detalles» es una etiqueta visual con `aria-disabled="true"`, sin enlace ni comportamiento. El aviso debajo del catálogo explica esta limitación.

## Sustituir imágenes

Las seis tarjetas comparten una ilustración y emplean variantes cromáticas CSS. Son marcadores visuales, no fotografías ni muestras exactas de los modelos. La imagen principal también está identificada como referencia.

1. Guarda fotografías propias o con permiso de uso en `images/`, por ejemplo `rosa-de-abril.jpg`.
2. Cambia el `src` correspondiente a `images/rosa-de-abril.jpg`.
3. Escribe un texto `alt` que describa la fotografía real y actualiza los atributos `width` y `height` a sus dimensiones.
4. Elimina de esa imagen las clases de color (`green`, `gold`, `terracotta`, `violet` o `lace`), si existen.
5. Para fotografías que llenen el marco, cambia `object-fit:contain` por `object-fit:cover` y reduce o elimina el `padding` en `.product-image img` o `.image-frame img`.
6. Retira los avisos de ilustración únicamente cuando hayas reemplazado todas las referencias pertinentes.

No se han descargado imágenes ni utilizado URLs externas.

## Accesibilidad y revisión

Incluye idioma español, enlace para saltar al contenido, navegación por anclas, foco visible, textos alternativos y respeto por la preferencia de movimiento reducido. El menú permanece visible en móviles sin JavaScript. El correo `.example` y la ubicación son ficticios; no hay envío de mensajes.

Para revisar visualmente, abre el archivo y prueba anchos de 1440, 768 y 390 píxeles, navegación con Tab y zoom al 200 %. La comprobación estática de rutas y anclas no reemplaza una prueba visual en navegador.
