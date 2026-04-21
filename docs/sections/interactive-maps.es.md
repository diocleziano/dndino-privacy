# Mapas interactivos

Los **mapas interactivos** sirven para navegar visualmente por los lugares de la aventura sobre un mapa gráfico real, usando marcadores clicables vinculados a los registros de lugares.

Están pensados para los casos en los que la simple estructura en árbol ya no basta y quieres moverte por el espacio de la campaña de una forma más natural, por ejemplo sobre:

- una ciudad
- un castillo
- un barrio
- una mazmorra
- una región

## Para qué sirven

Los mapas interactivos son útiles cuando quieres:

- usar un mapa como superficie principal de navegación
- abrir lugares haciendo clic en marcadores visuales
- dar una estructura espacial más clara a la campaña
- pasar de un mapa de detalle a uno más amplio

No sustituyen a los **Lugares** ni sustituyen a los **Mapas conceptuales**:

- los **Lugares** siguen siendo los registros reales de la campaña
- los **Mapas conceptuales** sirven para mostrar relaciones lógicas y narrativas
- los **Mapas interactivos** sirven en cambio para navegar lugares reales sobre una imagen de mapa

## De dónde nacen

Los mapas interactivos no son un tipo de registro separado creado en un módulo aparte. Nacen a partir de las **imágenes de mapa** vinculadas a los lugares.

En la práctica:

1. vinculas una o más imágenes de tipo `Mapa` a un lugar
2. eliges cuál de ellas debe usarse como mapa interactivo por defecto
3. sobre ese mapa añades marcadores vinculados a los lugares

## Dónde se usan

Los mapas interactivos viven en la sección **Lugares y Misiones**.

Pueden usarse de dos formas:

- como **modo interactivo integrado** dentro del panel de lugares
- como **panel de mapa grande** abierto desde `Medios`

## Diferencia entre modo integrado y panel grande

### Modo interactivo integrado

Cuando la aventura tiene mapas disponibles, dentro del panel de lugares puedes pasar de la vista normal a la vista `Interactiva`.

En este modo:

- la parte izquierda de la pantalla muestra el mapa en lugar del árbol clásico de lugares
- el panel derecho sigue mostrando el detalle del lugar seleccionado
- al hacer clic en los marcadores navegas directamente entre los lugares

### Panel de mapa grande

Desde el panel `Medios` de un lugar también puedes abrir un mapa interactivo en un panel dedicado más grande.

Este modo resulta especialmente útil cuando quieres:

- modificar marcadores
- ajustar vínculos
- trabajar con más precisión sobre el mapa

## Cómo se prepara un mapa interactivo

El flujo correcto es el siguiente:

1. abre el lugar que debe poseer el mapa
2. ve a la sección `Medios`
3. añade una o más imágenes de tipo `Mapa`
4. elige cuál de ellas debe convertirse en el mapa interactivo por defecto
5. abre el mapa interactivo
6. crea los marcadores y vincúlalos a los lugares

## Cómo se elige el mapa por defecto

Un lugar puede tener varios mapas vinculados. Entre ellos, uno puede marcarse como mapa interactivo de referencia.

Cuando DnDino necesita decidir qué mapa mostrar para un lugar, usa esta lógica:

- si el lugar tiene un mapa seleccionado explícitamente como mapa interactivo, usa ese
- en caso contrario usa el primer mapa disponible del lugar
- si el lugar no tiene mapas propios, puede usar el mapa de un lugar padre

## Relación entre lugar y mapa

Cada mapa interactivo pertenece a un lugar.

El lugar propietario del mapa no tiene por qué ser el único lugar que se puede abrir desde él: los marcadores pueden vincular cualquier lugar de la estructura de la aventura.

## Cómo se entra en el modo interactivo

En el panel `Lugares`, cuando existen mapas disponibles, puedes pasar a la vista `Interactiva`.

En ese modo encontrarás:

- cabecera del mapa interactivo
- selector `Mapa`
- posible botón `Atrás`
- posible botón `Nivel superior`
- toggle `Mostrar nombres de marcadores`
- controles de zoom
- canvas del mapa

## Selector de mapa

El menú `Mapa` permite elegir qué mapa mostrar entre los disponibles en la aventura.

## Navegación entre mapas

El modo interactivo admite dos tipos de navegación entre mapas.

### Atrás

El botón `Atrás` devuelve al mapa mostrado anteriormente.

### Nivel superior

Si el lugar actual tiene un lugar padre que posee un mapa interactivo, puede aparecer el botón `Nivel superior`.

Esto te permite subir a un mapa más amplio.

## El canvas del mapa

El canvas es la superficie central donde se muestra el mapa propiamente dicho.

Aquí puedes:

- ver el mapa
- ver los marcadores
- hacer clic o doble clic sobre los marcadores
- usar zoom y pan

## Zoom y desplazamiento

Los mapas interactivos admiten:

- zoom hacia delante y hacia atrás
- restablecimiento del zoom
- desplazamiento horizontal y vertical
- pan arrastrando el mapa
- gesto de pinza
- zoom con la rueda del ratón cuando el cursor está sobre el mapa

## Mostrar nombres de marcadores

Con el toggle `Mostrar nombres de marcadores` puedes decidir si quieres ver también las etiquetas de los marcadores directamente sobre el mapa.

Cuando está activo:

- cada marcador puede mostrar su propio nombre o, si el título está vacío, el nombre del lugar vinculado

Cuando está desactivado:

- solo permanecen visibles los iconos de los marcadores

## Cómo funcionan los marcadores

Un marcador contiene:

- posición normalizada sobre el mapa
- título opcional
- vínculo opcional a un lugar

El marcador se guarda respecto a las coordenadas del mapa, por lo que sigue permaneciendo en el punto correcto incluso si cambias el zoom.

## Comportamiento de los marcadores en lectura

Cuando no estás en modo edición:

- un **clic simple** selecciona un marcador
- un **doble clic** abre el lugar vinculado

En el modo interactivo integrado, abrir un lugar significa actualizar enseguida el panel derecho.

En el panel de mapa grande, abrir un lugar cierra el panel del mapa y devuelve el foco al lugar seleccionado en el dashboard.

## Cómo se crea un marcador

Para crear un marcador en el panel de mapa grande:

1. abre el mapa interactivo desde `Medios`
2. pulsa `Editar`
3. pulsa `Nuevo marcador`
4. elige el lugar que vas a asociar
5. haz clic en un punto del mapa

## Modo edición

En el panel grande existe un verdadero estado de edición.

Cuando pulsas `Editar`:

- el mapa entra en modo edición
- puedes crear nuevos marcadores
- puedes seleccionar marcadores existentes para modificarlos
- puedes arrastrar los marcadores para recolocarlos

Cuando pulsas `Bloquear`, sales del modo edición.

## Nuevo marcador

Cuando activas `Nuevo marcador`:

- DnDino te pide primero elegir el lugar que quieres asociar
- después te invita a hacer clic sobre el mapa para colocarlo

## Elección del lugar vinculado

Cuando estás creando o editando un marcador, el inspector de la derecha muestra el selector de lugares.

Desde ahí puedes:

- buscar por nombre
- ver los lugares organizados en estructura jerárquica
- asignar el marcador al lugar correcto

## Modificar un marcador existente

Cuando un marcador está seleccionado en modo edición, en el inspector puedes modificar:

- `Título del marcador`
- `Lugar vinculado`

Si el título se deja vacío, DnDino usa como fallback el nombre del lugar vinculado o un título genérico.

## Mover un marcador

En modo edición puedes arrastrar un marcador a un nuevo punto del mapa.

Al final del arrastre, DnDino guarda:

- nueva posición X
- nueva posición Y

## Eliminar un marcador

También desde el inspector, cuando un marcador está seleccionado, puedes usar:

- `Eliminar marcador`

## El inspector del mapa

El panel lateral del mapa grande cambia según el estado actual.

### En lectura

Si no estás editando, el inspector muestra simplemente la lista de marcadores existentes.

### Durante la creación de un marcador

Si has activado `Nuevo marcador`, el inspector muestra:

- instrucciones
- campo de búsqueda
- lista de lugares seleccionables

### Durante la modificación de un marcador

Si has seleccionado un marcador existente, el inspector muestra:

- campo de título
- selector de lugar vinculado
- resumen del lugar actual
- botón para eliminar el marcador

## Lista de marcadores

La lista de marcadores dentro del inspector también puede usarse para navegar.

Cada fila muestra:

- título del marcador
- lugar vinculado, si existe

En lectura, al hacer clic en la fila puedes abrir el lugar vinculado.

## Cómo se comporta el mapa en el modo integrado

Cuando usas el modo `Interactiva` directamente dentro del panel de lugares:

- el mapa sigue al lugar seleccionado
- DnDino intenta mostrar el mapa más adecuado para ese lugar
- si el lugar no tiene un mapa propio, puede usar un mapa de un nivel superior

## Herencia del mapa desde el lugar padre

Una parte muy útil del sistema es que un lugar puede usar también un mapa de un nivel superior.

Esto permite escenarios como:

- el barrio usa el mapa de la ciudad
- la sala usa el mapa del castillo
- el punto de interés usa el mapa de la región

## Cómo abrir un mapa interactivo desde Medios

En el panel `Medios` de un lugar, los mapas de tipo `Mapa` pueden mostrar la acción:

- `Abrir mapa interactivo`

## Cuándo conviene usar el modo integrado

Conviene usar el modo interactivo integrado cuando quieres:

- navegar rápidamente entre los lugares
- trabajar con mapa y panel de lugar lado a lado
- usar el mapa como alternativa al árbol clásico

## Cuándo conviene usar el panel grande

Conviene usar el panel grande cuando quieres:

- crear marcadores
- mover marcadores
- cambiar vínculos
- trabajar con más precisión

## En la práctica

Los mapas interactivos son la herramienta adecuada cuando quieres dar a los lugares una verdadera dimensión espacial.

La idea clave es simple:

- el **lugar** sigue siendo el registro principal
- el **mapa** se convierte en la superficie visual
- el **marcador** es el vínculo operativo entre imagen y contenido
