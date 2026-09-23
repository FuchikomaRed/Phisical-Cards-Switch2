Base maestra de lanzamientos físicos de Nintendo Switch 2
Base de datos pública para catalogar los lanzamientos físicos de Nintendo Switch 2 y distinguir entre cartuchos que contienen el juego y ediciones que requieren una descarga mediante Game-Key Card.

Qué clasifica
Cada registro distingue entre:

Cartucho Completo: el cartucho contiene los datos principales del juego.

Game-Key Card: el cartucho contiene la clave necesaria para descargar el juego y debe conservarse insertado para jugar.

También se diferencia entre:

Nintendo Switch 2 Edition: edición específica para Nintendo Switch 2.

Switch 1 compatible: edición física que también puede utilizarse en una Nintendo Switch original.

Campos del CSV
Los datos se almacenan en switch2_fisicos.csv.

Campo	Descripción
titulo	Nombre del juego.
editor	Editorial o distribuidora.
region	Región de la edición: NA, JP, EU o varias separadas por |.
formato	Cartucho Completo o Game-Key Card.
edicion_plataforma	Nintendo Switch 2 Edition o Switch 1 compatible.
compatible_switch1	Indica si la edición puede utilizarse en Nintendo Switch original.
descarga_gb	Tamaño aproximado de la descarga necesaria.
excepcion_regional	Diferencias de formato entre regiones.
codigo_producto	Código de producto o referencia comercial, cuando está disponible.
notas	Observaciones sobre la edición, compatibilidad o preservación.
fecha_lanzamiento	Fecha en formato AAAA-MM-DD.
estado	Confirmado o Próximo.
Cómo añadir un juego
Abre switch2_fisicos.csv.

Añade una línea nueva respetando el orden de las columnas.

Mantén la codificación UTF-8.

Utiliza comillas dobles si un campo contiene comas.

Guarda los cambios y haz commit en GitHub.

Espera unos instantes a que GitHub Pages actualice la web.

Ejemplo:

text
Nuevo juego,Editorial,NA|EU,Game-Key Card,Nintendo Switch 2 Edition,No,32,No confirmada,ABC-123,Descarga obligatoria,2026-10-30,Próximo
Estructura del proyecto
text
.
├── index.html
├── switch2_fisicos.csv
└── README.md
index.html: interfaz web con búsqueda, filtros y estadísticas.

switch2_fisicos.csv: fuente de datos editable.

README.md: documentación del proyecto.

Filtros disponibles
La interfaz permite filtrar por:

Texto libre.

Editor.

Región.

Formato físico.

Tipo de edición o compatibilidad.

También muestra contadores de resultados, cartuchos completos, Game-Key Cards, Nintendo Switch 2 Editions y ediciones compatibles con Switch 1.

Alertas de próximos lanzamientos
La página incluye una sección independiente para señalar próximos lanzamientos confirmados como Game-Key Card. Estas alertas deben revisarse periódicamente porque el formato físico, la región o la fecha pueden cambiar antes de la publicación.

Criterios de catalogación
Se considera Cartucho Completo cuando la tarjeta contiene los datos principales del juego y no depende de una descarga completa para iniciar la experiencia.

Se considera Game-Key Card cuando la tarjeta no contiene el juego completo y requiere descargar los datos desde Internet.

Las actualizaciones, parches, contenido adicional y requisitos online se anotan aparte y no cambian automáticamente la categoría principal.

Las diferencias entre regiones se registran en filas independientes cuando el formato físico cambia entre NA, JP y EU.

Los tamaños marcados como Por confirmar no deben sustituirse por estimaciones sin una fuente verificable.

Estado de los datos
La base se encuentra en desarrollo y puede contener registros pendientes de confirmación. Antes de publicar una edición como definitiva, conviene comprobar:

La carátula regional.

La ficha de la editorial o distribuidora.

La tienda oficial de la región correspondiente.

El tamaño de descarga indicado por Nintendo o por el editor.

La compatibilidad con Nintendo Switch original.

Licencia y contribuciones
Este repositorio contiene datos de catalogación y una interfaz de consulta. Las marcas, nombres de juegos, logotipos y materiales pertenecen a sus respectivos propietarios.

Para proponer una corrección o añadir un lanzamiento, abre una incidencia en GitHub o realiza un pull request con la fuente de verificación correspondiente.
