# Lugares

La sección **Lugares** reúne todo lo relacionado con los espacios jugables de una aventura: ciudades, mazmorras, salas, zonas narrativas, misiones vinculadas, presencias, combates, imágenes, mapas y mapas interactivos.

Es una de las secciones más ricas de la aplicación, porque reúne:

- estructura narrativa
- estado de exploración
- contenido que mostrar a los jugadores
- presencias contextuales
- acceso rápido a los combates

## Para qué sirve la sección Lugares

El panel de lugares sirve para organizar la aventura tanto en el plano espacial como en el narrativo.

Aquí puedes:

- crear lugares y misiones
- construir jerarquías de lugares y sublugares
- enlazar imágenes y mapas
- gestionar las presencias en un lugar
- crear y reabrir combates vinculados a un lugar concreto
- mantener descripciones separadas para DM y jugadores
- usar un mapa interactivo para moverte entre lugares

## Cómo llegar

La sección se abre desde el **panel de aventura**, entrando en la tarjeta `Lugares y Misiones`.

Desde esa tarjeta puedes:

- abrir todo el panel de lugares
- usar accesos rápidos a un lugar reciente cuando existan
- usar accesos rápidos a un combate reciente vinculado a un lugar

## Estructura de la pantalla

El panel `Lugares` se organiza en torno a dos modos principales:

- `Normal`
- `Interactivo`

y en torno a dos áreas:

- una **columna izquierda** con árbol, búsqueda, filtros y acciones rápidas
- un **panel derecho** con el detalle del lugar seleccionado

## Modos Normal e Interactivo

### Modo Normal

![Modo Normal de Lugares](../images/avventura/it_LuoghiNormale.png){ .img-hero }

Es el modo clásico, pensado para trabajar directamente sobre:

- el árbol de lugares
- el detalle del lugar seleccionado
- presencias
- combates
- medios
- notas

Es el modo más adecuado para preparar y editar la aventura.

### Modo Interactivo

![Modo Interactivo de Lugares](../images/avventura/it_LuoghiInterattiva.png){ .img-hero }

El modo `Interactivo` se activa cuando la aventura dispone de mapas interactivos listos para usar.

En este modo, el foco pasa a la navegación mediante mapa:

- la parte izquierda de la pantalla muestra el mapa interactivo en lugar del árbol clásico
- los marcadores pueden seleccionarse
- con doble clic se puede abrir el lugar enlazado en el panel derecho
- los nombres de los marcadores pueden mostrarse u ocultarse
- están disponibles el zoom y el desplazamiento del mapa

Desde la pestaña `Medios` puedes seguir abriendo rápidamente el mapa interactivo asociado a uno de los mapas del lugar, pero en el modo `Interactivo` el mapa se convierte en el contenido principal de la parte izquierda del panel.

## La columna izquierda

La columna izquierda es el panel de navegación de esta sección.

Aquí encontrarás:

- búsqueda
- filtros
- un resumen compacto
- el árbol de lugares y misiones

### Menú contextual sobre lugares en el árbol

En el modo árbol puedes **hacer clic derecho sobre un lugar** para abrir un menú contextual con acciones rápidas directamente sobre ese nodo.

Las acciones disponibles son:

- `Añadir sublugar`
- `Añadir presencia`
- `Añadir enlace`
- `Eliminar enlace`
- `Crear mapa conceptual`
- `Crear combate`
- `Editar`
- `Eliminar lugar`

Este menú es una de las formas más rápidas de construir la estructura de la aventura mientras trabajas en el árbol.

En la práctica, te permite reorganizar el árbol rápidamente sin abrir cada vez el formulario completo del lugar.

### Reordenación rápida con arrastrar y soltar

El árbol de lugares también admite un flujo rápido mediante arrastrar y soltar.

Puedes:

- cambiar el orden de los lugares hermanos
- mover un lugar debajo de otro lugar
- devolver un lugar a la raíz si lo arrastras fuera de una rama padre

Esto hace mucho más rápido ajustar la estructura narrativa mientras preparas la aventura.

### Filtros y resumen

La barra lateral también muestra un resumen compacto con:

- total de lugares
- número de misiones
- número de lugares en visita

Según el modo y el contexto, los filtros pueden incluir:

- todos
- lugares
- misiones
- en visita
- activas

## Crear un lugar o una misión

Para crear un nuevo registro, utiliza el botón de creación en el panel de lugares.

El formulario se divide en tres grupos principales:

- `Información principal`
- `Descripciones`
- `Recursos del lugar`

## Información principal del lugar

En el formulario puedes completar:

- `Nombre`
- lugar padre o enlaces a lugares padre
- `Tipo`
- `Marcador`
- estado del lugar o estado de la misión

### Tipo: Lugar o Misión

El campo `Tipo` te permite elegir si el registro es un:

- `Lugar`
- `Misión`

Si el registro es un **Lugar**, usa el estado de visita:

- no visitado
- en visita
- visitado

Si el registro es una **Misión**, usa en cambio el estado de progreso:

- inactiva
- no disponible
- activa
- completada

## Lugares padre y jerarquía

El formulario de lugares admite una jerarquía avanzada.

Puedes seleccionar uno o varios lugares padre, y DnDino guarda esa relación como una estructura jerárquica real.

Esto significa que un lugar puede:

- estar en la raíz de la aventura
- existir como sublugar de otro lugar
- estar enlazado en más de un punto de la estructura cuando haga falta

Esto es útil, por ejemplo, cuando quieres:

- colocar un grupo entero de lugares bajo una misión
- mostrar el mismo lugar en más de una rama del árbol
- crear rutas narrativas distintas sin duplicar el registro

En estos casos, el lugar **no se duplica**: el árbol solo añade un enlace adicional al mismo lugar.

Cuando eliminas un enlace:

- el lugar no se borra
- si tiene varios padres, solo se elimina el enlace adicional
- si pierde su único padre, vuelve a la raíz del árbol

El formulario sigue evitando ciclos, excluyendo automáticamente el propio lugar y su subárbol de la lista de posibles padres.

## Marcadores del lugar

Cada lugar puede tener uno o más marcadores especiales, visibles también en el panel.

Entre los marcadores disponibles están:

- peligroso
- importante
- secreto
- bloqueado

Sirven como resaltados visuales rápidos para leer la aventura de un vistazo.

## Descripciones del lugar

La sección `Descripciones` del formulario se divide en varios campos de texto enriquecido:

- `Descripción DM`
- `Descripción jugadores`
- `Pistas`
- `Tesoros`
- `Notas`

Esta separación es muy útil porque te permite distinguir:

- lo que debe saber el DM
- lo que los jugadores pueden ver o descubrir
- información de apoyo como pistas y tesoros

## Enlaces internos en los textos del lugar

El sistema de **enlaces internos** también es muy útil en `Lugares`.

Aquí no se trata tanto de automatizar ataques como de hacer que el texto del lugar sea **navegable** y más rápido de usar en mesa.

Dentro de los campos de texto enriquecido de un lugar puedes insertar enlaces a:

- `Personaje`
- `Lugar`
- `Hechizo`
- `Dote`
- `Regla`
- y, cuando sea útil, también enlaces de tirada

### Por qué son útiles en los lugares

Las descripciones de lugar suelen contener muchas referencias:

- personajes presentes o mencionados
- lugares relacionados
- objetos o hechizos mencionados en el texto
- reglas especiales de escena

Convertir esas referencias en enlaces internos te permite:

- abrir al instante la ficha de un personaje citado
- saltar directamente a otro lugar de la aventura
- consultar un hechizo o una regla sin salir del contexto
- escribir descripciones más densas que sigan siendo fáciles de navegar

### Ejemplos prácticos

Puedes enlazar un personaje mencionado en el lugar, como `capitán Arven`, o un lugar citado en el texto, como `Cripta sumergida`.

De ese modo, la descripción deja de ser solo narrativa: también se convierte en un atajo de navegación.

### Dónde funcionan mejor

Las mejores partes de la ficha de lugar para usar enlaces internos son:

- `Descripción DM`
- `Descripción jugadores`
- `Pistas`
- `Notas`

### Búsqueda inicial del selector

Cuando pulsas `Enlace`, el selector intenta usar el texto seleccionado como filtro inicial.

Si encuentra una coincidencia real en el nombre de un registro:

- se abre ya filtrado

Si no encuentra resultados reales:

- limpia el filtro inicial
- y muestra la lista completa

## Recursos del lugar

Cada lugar puede tener sus propios recursos, divididos en:

- imágenes
- mapas

En el formulario puedes:

- añadir imágenes
- añadir mapas
- elegir la portada del lugar
- quitar la portada

Para cada recurso puedes configurar:

- nombre mostrado
- visibilidad para `Jugadores`
- visibilidad para `DM`
- texto de presentación

## Área hero del lugar

Cuando seleccionas un lugar, el panel derecho muestra un área hero con:

- la portada del lugar
- nombre
- tipo (`Lugar` o `Misión`)
- estado actual
- posibles marcadores
- la cadena jerárquica del lugar

También aparece un resumen rápido con:

- `Presencias`
- `Sublugares`
- `Imágenes`
- `Mapas`

## Pestañas de detalle

El panel derecho utiliza una barra de foco con cinco secciones principales:

- `Panorámica`
- `Presencias`
- `Combates`
- `Medios`
- `Notas`

### Panorámica

La pestaña `Panorámica` reúne:

- descripción DM
- descripción jugadores
- pistas
- tesoros
- mapas conceptuales vinculados al lugar

### Presencias

La pestaña `Presencias` reúne los personajes presentes en el lugar.

Desde aquí puedes:

- ver todas las presencias del lugar
- añadir una nueva presencia
- abrir el detalle contextual de esa presencia
- cambiar su rol en el lugar
- leer o editar las `Notas DM`
- eliminar la presencia

### Combates

La pestaña `Combates` muestra todos los enfrentamientos vinculados al lugar.

Desde aquí puedes:

- crear un nuevo combate para el lugar
- reabrir un combate existente
- ver si no ha empezado, está en pausa o ha concluido
- eliminar un combate

### Medios

La pestaña `Medios` reúne:

- imágenes del lugar
- mapas del lugar
- mapas heredados de lugares padre cuando están activados

Desde aquí puedes:

- explorar imágenes
- explorar mapas
- mostrarlos a los jugadores
- mostrarlos al DM
- abrir directamente un mapa interactivo

### Notas

La pestaña `Notas` está dedicada a las notas rápidas del DM para el lugar.

## Presencias del lugar

Las presencias del lugar se gestionan de forma contextual y separada de los personajes de aventura y de los participantes en combate.

Esto te permite conservar:

- nombres mostrados contextuales
- rol en el lugar
- notas DM locales
- estado local cuando sea necesario

## Dos posibles orígenes para una presencia

Cuando añades una presencia a un lugar, el formulario te pide el `Origen`.

Las fuentes posibles son:

- `Personaje de aventura`
- `Ficha base`

### Personaje de aventura

Este origen utiliza un personaje que ya está vinculado a la aventura.

En este caso, la presencia mantiene el estado contextual de campaña.

### Ficha base

Este origen clona un registro base del tipo:

- `PNJ`
- `Monstruo`

Los registros de tipo `Héroe` no pueden seleccionarse en este modo.

## Reglas de unicidad de las presencias

En el panel de lugares, DnDino aplica reglas muy concretas:

- un `Personaje de aventura` solo puede colocarse una vez en el mismo lugar
- un `PNJ` base solo puede añadirse una vez en el mismo lugar
- un `Monstruo` base puede añadirse varias veces en el mismo lugar

Cuando añades varias instancias del mismo monstruo, el nombre mostrado se numera automáticamente, por ejemplo:

- `Goblin`
- `Goblin 2`
- `Goblin 3`

## Datos de la presencia en el lugar

En el formulario de presencia puedes configurar:

- `Rol de encuentro`
- `Nombre mostrado`
- `Condiciones`
- `Notas DM`

Si la presencia proviene de una **ficha base** (`PNJ` o `Monstruo`), también dispones de un estado local del lugar como:

- PG temporales
- PG actuales
- estado

Si la presencia proviene de un **Personaje de aventura**, el lugar sigue referenciando ese estado contextual de campaña en lugar de duplicarlo localmente de la misma manera.

## Rol en el lugar

Cada presencia tiene un rol contextual:

- aliado
- neutral
- enemigo

Este rol es importante tanto para leer la escena como para flujos posteriores, como los combates.

## Combates vinculados al lugar

Los combates dentro de los lugares se crean directamente desde el lugar seleccionado.

Cuando creas un nuevo combate:

- el combate se guarda como encuentro de ese lugar
- aparece de inmediato en la pestaña `Combates`
- puede reabrirse más adelante

## Medios del lugar

La zona de medios del lugar distingue claramente entre:

- imágenes
- mapas

El panel también puede mostrar mapas heredados de lugares padre mediante el selector:

- `Mostrar mapas de lugares padre`

## Mapa interactivo

Cuando un mapa se selecciona como mapa interactivo del lugar, puedes abrirlo directamente desde el panel.

El mapa interactivo admite:

- zoom
- desplazamiento
- marcadores
- navegación entre lugares

### Marcadores del mapa interactivo

Cada marcador puede tener:

- una posición en el mapa
- un título
- un lugar de destino enlazado

Los marcadores pueden:

- crearse
- moverse
- renombrarse
- asociarse a un lugar
- eliminarse

Comportamiento básico:

- clic simple: seleccionar el marcador
- doble clic: abrir el lugar enlazado en el panel derecho

## Relación entre Lugares, Mapas y Mapas interactivos

Conviene pensar en estos tres elementos como capas distintas:

- el **lugar** es el contenedor narrativo y estructural
- el **mapa** es un recurso visual vinculado al lugar
- el **mapa interactivo** es un mapa elegido como soporte navegable, enriquecido con marcadores

## Misiones en la sección Lugares

Las misiones viven en la misma sección que los lugares, pero siguen su propio comportamiento.

Una misión:

- aparece en el árbol junto a los lugares
- usa un estado de progreso en lugar de un estado de visita
- aun así puede tener descripciones, notas, imágenes, mapas, presencias y enlaces contextuales

## Cuándo usar la sección Lugares

El panel `Lugares` es el lugar adecuado cuando quieres:

- construir la geografía de la campaña
- definir sublugares y enlaces
- preparar misiones y su estado
- situar presencias dentro del mundo
