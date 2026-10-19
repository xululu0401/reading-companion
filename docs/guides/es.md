# Guía de Compañero de lectura

Para la versión 0.3.x. Lee archivos o páginas web, toma notas y crea tarjetas para compartir. Las funciones básicas no requieren cuenta ni clave de IA. Esta guía funciona sin conexión.

## 1. Primeros pasos

1. Abre un archivo EPUB, PDF o TXT desde la aplicación de escritorio, o cambia a lectura web e introduce una URL.
2. Selecciona un libro y crea una nota a la derecha con título y contenido.
3. Espera la confirmación de guardado local. No significa que exista una copia en la nube.
4. Crea tarjetas, edita el texto y los colores, exporta imágenes y copia el texto para publicar.
5. Exporta una copia JSON y conserva los libros originales por separado.

Descarga el instalador desde la página oficial de versiones. La navegación integrada y la configuración de IA requieren la aplicación de escritorio.

## 2. Interfaz y lista de notas

- La biblioteca permite elegir libros, editar sus datos y buscar títulos o contenido de notas. No busca en el texto completo de los libros.
- Arrastra el separador entre lectura y notas para cambiar el ancho. Haz doble clic para restablecerlo; con el foco en el separador puedes usar las flechas.
- Abre la flecha junto al título de la nota actual para ver todas las notas de ese libro. El número 4 incluye notas, extractos y resúmenes; el número no es el botón de la lista.
- Cambiar entre lectura y estudio de publicación conserva la página cargada. Cambiar de libro o actualizar manualmente puede navegar a otra página.
- Sal de la lectura a pantalla completa con su botón o Esc. El modo de escritura concentrada tiene un botón para volver al diseño normal.
- El botón de interrogación de la barra superior abre esta guía sin abandonar la lectura.

Eliminar libros: pulsa la papelera junto al libro en la biblioteca de la izquierda o elige «Eliminar de la biblioteca» al editar sus datos. La confirmación muestra el número de notas asociadas y permite crear una copia de seguridad. Al confirmar se eliminan también las notas, extractos, resúmenes y borradores para compartir de ese libro; no se puede deshacer. Los archivos originales y los libros de tus cuentas web no se modifican; la caché de archivos importados permanece en la aplicación. También puedes eliminar el último libro y añadir una URL o abrir un archivo desde la biblioteca vacía.

## 3. Leer EPUB, PDF y TXT

Abre archivos sin DRM de hasta 50 MB; TXT admite hasta 10 MB. Los libros importados permanecen en el dispositivo.

- EPUB: índice, capítulos anterior/siguiente, tamaño de letra, temas, marcadores por capítulo y posición de lectura. Se usa un diseño propio, sin reproducir todos los estilos, fuentes o diseños fijos del editor.
- PDF: salto de página, zoom, marcadores y selección si existe una capa de texto. Las páginas escaneadas no permiten extraer texto directamente. No hay OCR, anotaciones manuscritas ni formularios interactivos.
- TXT: UTF-8 o UTF-16 con BOM, división en secciones, tamaño, temas y marcadores. Si aparecen caracteres incorrectos, convierte el archivo a UTF-8 antes de importarlo.

Si falta el original, abre exactamente el mismo archivo para asociar notas y progreso mediante su huella. Un archivo modificado puede identificarse como otro libro. Conserva siempre copias de los originales.

## 4. Lectura web y extractos

Introduce directamente una URL como `https://weread.qq.com` y pulsa Enter, o usa un acceso directo. Las palabras normales se envían a la búsqueda de Baidu; algunos nombres de servicios reconocidos abren su web. Inicia sesión mediante el sitio. Usa atrás, adelante y actualizar/detener, y guarda la página actual en la biblioteca.

Los enlaces ordinarios de nueva ventana se abren en el panel de lectura. Los procesos de inicio de sesión, pago o ventanas solicitadas explícitamente pueden abrirse aparte. La opción de permitir ventanas independientes modifica el comportamiento de los enlaces ordinarios.

Selecciona texto normal y utiliza el menú contextual para guardarlo como extracto. Confirma texto, fuente y libro de destino.

Algunos sitios, como WeRead, dibujan su propia selección. Utiliza primero la función Copiar del sitio y después pega como extracto desde el menú contextual de la aplicación. El portapapeles solo se lee al elegir esa acción. Comprueba lo pegado; también puedes abrir Extracto a la derecha y pegar texto y fuente manualmente.

Las cuentas, suscripciones y resaltados pertenecen al sitio web. La aplicación no evita restricciones de membresía, copia o DRM ni garantiza que todos los sitios permitan incrustarse. Si falla una página, compruébala en un navegador normal.

## 5. Notas, extractos y guardado automático

Las notas guardan tus ideas; los extractos conservan texto original con capítulo, página o URL; los resúmenes de IA se guardan como notas separadas. Todos aparecen en la lista del libro y se pueden editar y compartir.

Selecciona texto solo dentro de la lectura local y utiliza el menú contextual o el botón de extracto. El diálogo admite hasta 20.000 caracteres. El editor ofrece encabezados, negrita, cursiva, listas, citas, imágenes, dibujos sencillos, deshacer y rehacer. Los dibujos son ilustraciones; no hay reconocimiento de escritura ni todas las funciones de Goodnotes. Las imágenes de las notas no se convierten automáticamente en portadas.

Notas y borradores se guardan automáticamente. Observa el estado de guardado; ante un fallo, exporta una copia y luego reintenta. No borres los datos. El botón de guardar ajustes de IA solo guarda la configuración del servicio.

El botón de descarga de la nota exporta Markdown para reutilizar texto, no una copia completa. Eliminar una nota elimina también su borrador de publicación. No hay papelera: haz una copia antes si lo necesitas.

## 6. Configurar servicios de IA

La IA es opcional. Aportas tu clave y pagas al proveedor. El servicio oficial gestionado, las suscripciones y las recargas no están implementados.

1. En ajustes elige DeepSeek, OpenAI, Claude, Gemini, Qwen, Kimi, GLM, Ollama o API personalizada y añade una configuración.
2. Introduce nombre, tipo de API, URL y clave.
3. Obtén la lista de modelos o escribe el ID que indique el proveedor. URL y clave no garantizan la detección automática.
4. La prueba de conexión envía una petición breve sin notas, pero puede tener coste. Obtener modelos también envía autenticación al destino configurado.
5. Guarda y activa la configuración y comprueba el servicio activo. Para cambiar, selecciona otra y guarda y activa. La primera configuración guardada se convierte en la predeterminada. Puedes guardar hasta 30.

Se admiten OpenAI Chat Completions, OpenAI Responses y Anthropic Messages. Gemini utiliza su API compatible con OpenAI. Incluye la ruta de versión requerida, como `https://api.example.com/v1`; `/v1` no se añade automáticamente. Los destinos remotos necesitan HTTPS; los locales pueden usar HTTP. No se admiten credenciales, parámetros de consulta ni fragmentos en la URL.

Instala e inicia Ollama por separado y prepara un modelo. Su dirección habitual es `http://localhost:11434/v1` y la clave puede quedar vacía. Obtén los modelos o introduce el nombre de uno instalado. Esta aplicación no descarga modelos.

El sistema operativo cifra las claves guardadas y no se vuelven a mostrar. Deja el campo vacío para conservar la clave. Si cambias dirección o protocolo debes introducirla otra vez o eliminarla explícitamente. Al borrar el servicio activo tendrás que activar otro.

## 7. Resumir y pulir con IA

Selecciona una nota, abre el organizador de IA y genera. Se admiten entre 10 y 50.000 caracteres. Solo se envían el texto de esa nota, su título y el título del libro, no el original, otras notas, cookies, imágenes o dibujos.

Se usa una captura del contenido al abrir el diálogo. Los cambios durante la generación no se añaden a esa petición. Para utilizar el contenido más reciente, termina la petición y vuelve a abrir el generador.

Revisa y edita el resultado antes de guardarlo como nueva nota de resumen; la original se conserva. La función de pulir en el estudio prepara título, cuerpo y etiquetas para aplicar al borrador. Regenerar envía otra petición que puede facturarse. Comprueba citas y afirmaciones atribuidas al autor.

## 8. Tarjetas y sincronización

1. Selecciona una nota y abre el estudio de publicación.
2. Edita título, cuerpo y colores; añade una portada JPG, PNG o WebP si quieres.
3. La vista previa tarda un momento en actualizarse. El texto largo se divide en páginas que puedes recorrer con flechas. Las imágenes son de 1080 × 1440 píxeles, proporción 3:4.
4. Exportar la tarjeta actual guarda una sola página PNG. Exporta las demás por separado; no hay exportación por lotes.
5. Copia el texto y publica tú las imágenes en Xiaohongshu u otra plataforma. La aplicación no publica automáticamente.

Título y cuerpo siguen inicialmente a la nota. Editar un campo en el estudio lo hace independiente y los cambios de la nota ya no lo sobrescriben. Restablece cada campo o ambos para seguir la nota otra vez. Esto reemplaza el texto independiente, así que conserva antes lo que necesites. Colores y portada se mantienen.

## 9. Copias, restauración y cambio de equipo

El guardado automático es local. Exporta JSON regularmente y conserva los libros aparte. JSON contiene datos para restaurar; no es una imagen para compartir ni requiere edición manual.

Incluye metadatos de libros, huellas, progreso, marcadores, notas, imágenes de notas y borradores. Excluye originales, cookies, claves de API y preferencia de idioma. La copia no tiene cifrado adicional.

Para cambiar de equipo: exporta el JSON más reciente → copia originales aparte → respalda primero las notas del equipo de destino → restaura y revisa las cantidades → abre los mismos archivos originales → inicia sesión en sitios y configura IA e idioma de nuevo.

Restaurar reemplaza la biblioteca y las notas actuales; no fusiona. El límite del archivo es 100 MB. Sin originales puedes leer las notas restauradas, pero no recuperar el texto del libro. El navegador y la aplicación usan almacenes distintos; JSON permite trasladar notas entre ellos.

## 10. Idiomas, privacidad y datos

Se admiten chino simplificado y tradicional, inglés, japonés y español, siguiendo el sistema o mediante selección manual. El cambio es inmediato y se guarda por separado de la IA. Otros idiomas del sistema usan inglés. Las notas existentes, los títulos y los sitios no se traducen. El selector de esta guía cambia solo su idioma. La IA recibe el idioma de la interfaz al solicitar la generación, aunque el resultado depende del modelo.

No hay sincronización automática en la nube, telemetría ni SDK publicitario. Las notas no son una caja fuerte cifrada. No borres los datos de la aplicación o del sitio sin una copia.

La ubicación habitual es `~/Library/Application Support/reading-companion` en macOS, `%APPDATA%/reading-companion` en Windows y `$XDG_CONFIG_HOME/reading-companion` o `~/.config/reading-companion` en Linux. Cierra y respalda antes de investigar archivos; no edites los datos en uso. Consulta los documentos públicos de privacidad y seguridad.

## 11. Problemas frecuentes

- No encuentro todas las notas: selecciona el libro y abre el menú junto al título de la nota actual.
- Extracto vacío: selecciona solo el texto de lectura. En sitios con selección propia, copia y pega; un PDF escaneado necesita OCR externo.
- La tarjeta no cambia: comprueba si el campo es independiente, restablece el seguimiento si procede y espera el renderizado. La portada se añade aparte.
- Idioma incorrecto: revisa la selección manual. Sitios y diálogos del sistema controlan su propio idioma.
- IA 401/403: clave y permisos; 404: URL, versión, protocolo e ID de modelo; 429: cuota o frecuencia; tiempo agotado: red y estado del proveedor.
- No hay lista de modelos: introduce un ID manual y prueba. Que no exista listado no implica que la generación falle.
- Almacenamiento seguro no disponible: revisa el llavero o servicio de credenciales del sistema. No se guardan claves en el backend de texto plano de Linux.
- Actualización lenta o pantalla de acceso: revisa red, sitio y sesión. Cambiar al estudio no debería actualizar la lectura; informa si puedes reproducirlo.
- Error al guardar o cargar: conserva los datos, exporta lo posible o restaura una copia conocida. No elimines el directorio para probar.

## 12. Límites y comentarios

No hay OCR, reconocimiento de escritura, anotaciones PDF, búsqueda completa en libros, sincronización en la nube, publicación automática ni IA oficial gestionada. No se ofrecen todas las capacidades de Goodnotes. No se han probado todas las interfaces de Windows/Linux, sitios y modelos. Las traducciones requieren revisión por hablantes nativos.

Incluye versión, sistema y arquitectura, idioma, escritorio o vista previa, pasos mínimos, resultado esperado y real, y capturas sin datos privados. Reproduce con un archivo pequeño propio; no adjuntes claves, cookies, libros con derechos ni toda tu biblioteca.

Informa de errores en https://github.com/xululu0401/reading-companion/issues . Para problemas de seguridad, sigue SECURITY.md del repositorio público y utiliza un canal privado sin revelar datos sensibles.
