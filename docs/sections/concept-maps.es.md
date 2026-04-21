# Mapas conceptuales

La sección **Mapas conceptuales** sirve para construir una representación visual de las relaciones entre lugares, personajes, otros mapas conceptuales y notas libres.

No es un mapa geográfico ni una pizarra genérica: es una herramienta pensada para conectar los nodos de la campaña de forma rápida, legible y navegable.

Puedes usarla para:

- organizar la estructura narrativa de la aventura
- conectar lugares y personajes
- trazar relaciones entre elementos importantes
- añadir recuadros temáticos
- anotar ideas directamente sobre nodos, recuadros y vínculos

## Dónde se encuentra

Los mapas conceptuales se abren desde dos puntos principales:

- desde el **panel de aventura**, en el bloque `Mapas conceptuales`
- desde el panel de un **lugar**, cuando quieres crear o abrir un mapa conceptual vinculado a ese lugar

Esto significa que un mapa conceptual puede ser:

- **global de la aventura**
- **vinculado a un lugar específico**

## Cómo es la pantalla

La pantalla de mapas conceptuales se divide en tres columnas principales:

- **barra lateral izquierda** con paleta y lista de mapas
- **canvas central** donde construyes el mapa
- **inspector a la derecha** con los detalles del elemento seleccionado

## Sidebar: paleta y fuentes

La barra lateral izquierda reúne todo lo que puedes insertar en el mapa.

Las categorías principales son:

- `Lugares`
- `Personajes`
- `Mapas`

Además puedes trabajar con:

- filtros
- búsqueda de texto
- creación de recuadros
- creación de nodos libres

## Filtros de la paleta

La paleta admite un filtro dedicado con estos modos:

- `Todo`
- `Lugares`
- `Personajes`
- `Mapas`

## Búsqueda en la paleta

La barra de búsqueda de la paleta sirve para encontrar rápidamente:

- un lugar
- un personaje
- un mapa conceptual ya existente

## Qué puedes arrastrar al canvas

En el canvas puedes arrastrar:

- lugares de la aventura
- personajes disponibles para la aventura
- otros mapas conceptuales
- nodos libres

Los personajes disponibles en la paleta no son todos los personajes de la base de datos de forma indiscriminada: el sistema usa los personajes vinculados a la aventura.

## Lugares en la paleta

Los lugares de la paleta se muestran teniendo en cuenta la jerarquía de los lugares de la aventura.

## Personajes en la paleta

Los personajes mostrados en la paleta tienen un subtítulo informativo que puede incluir:

- tipo
- raza
- clase

## Mapas en la paleta

La sección `Mapas` de la paleta muestra los otros mapas conceptuales de la aventura.

Esto es especialmente útil porque un mapa conceptual puede contener un nodo que apunta a otro mapa conceptual, creando una red de mapas conectados entre sí.

## Crear un nuevo mapa conceptual

Puedes crear un nuevo mapa conceptual:

- desde el panel de aventura
- desde el panel de un lugar
- directamente desde la pantalla de mapas conceptuales, si ya estás gestionando uno

Cuando se crea, DnDino le asigna automáticamente un nombre progresivo como:

- `Mapa conceptual`
- `Mapa conceptual 2`
- `Mapa conceptual 3`

## Renombrar un mapa

El título del mapa activo se puede editar directamente en la pantalla.

Cuando sales del campo o confirmas el cambio, DnDino guarda el nuevo nombre.

## Eliminar un mapa

Seleccionando un mapa activo puedes eliminarlo con el botón `Eliminar`.

## El canvas central

El **canvas** es la zona principal donde construyes el mapa.

Aquí puedes:

- arrastrar nodos desde la paleta
- mover nodos
- crear recuadros
- conectar nodos y recuadros con flechas
- leer la estructura general de la campaña de un vistazo

## Tipos de elementos en el canvas

En el canvas existen tres familias principales de elementos:

- **nodos**
- **recuadros**
- **conexiones**

### Nodos

Los nodos representan:

- un lugar
- un personaje
- un mapa conceptual
- un nodo libre

### Recuadros

Los recuadros sirven para agrupar visualmente varios nodos dentro de una zona común.

### Conexiones

Las conexiones son flechas que unen nodos y recuadros.

## Nodos normales y nodos libres

### Nodos vinculados a registros reales

Cuando arrastras al canvas un lugar, un personaje o un mapa conceptual, creas un nodo vinculado a un registro real de la aplicación.

Esto significa que el nodo:

- muestra el título real del elemento
- puede mostrar el subtítulo contextual
- puede abrir el registro vinculado desde el inspector

### Nodo libre

El `Nodo libre` es un nodo especial para ideas y apuntes no vinculados a un registro real.

Es útil para:

- anotaciones narrativas
- conceptos abstractos
- eventos
- grupos de ideas
- recordatorios de diseño

## Recuadros de grupo

El botón `Recuadro` crea un contenedor visual dentro del canvas.

Un recuadro:

- tiene un título
- tiene una nota dedicada
- se puede mover
- se puede redimensionar
- se puede colapsar
- puede contener automáticamente los nodos que quedan dentro de él

## Cómo se mueven los nodos

Los nodos pueden arrastrarse libremente dentro del canvas.

Su posición se guarda en el mapa, por lo que la organización permanece.

## Cómo se mueven los recuadros

Los recuadros también pueden arrastrarse.

Cuando mueves un recuadro, DnDino puede mover con él los nodos que contiene, manteniendo el grupo legible.

## Redimensionar un recuadro

Los recuadros pueden redimensionarse desde las esquinas.

## Colapsar un recuadro

Un recuadro puede colapsarse.

Cuando está colapsado:

- ocupa menos espacio
- los nodos internos se ocultan del canvas
- las conexiones de los elementos ocultos no dificultan la lectura

## Crear una conexión

Las conexiones entre elementos se crean arrastrando desde el punto de anclaje de un nodo o de un recuadro hacia otro elemento compatible.

Puedes conectar:

- nodo → nodo
- nodo → recuadro
- recuadro → nodo
- recuadro → recuadro

DnDino evita:

- conexiones duplicadas idénticas
- conexiones de un elemento consigo mismo

## Para qué sirven las flechas

Las flechas sirven para representar relaciones, por ejemplo:

- un personaje que controla un lugar
- un lugar que conduce a otro
- un mapa que remite a un submapa
- un grupo temático vinculado a un nodo narrativo

El significado de las flechas es libre, así que conviene adoptar una convención coherente en tu campaña.

## Inspector: detalles del elemento seleccionado

La columna derecha cambia según lo que selecciones.

Puede mostrar los detalles de:

- un nodo
- un recuadro
- una conexión
- o del mapa en su conjunto, si no hay nada seleccionado

## Si seleccionas un nodo

Cuando seleccionas un nodo, el inspector muestra:

- título
- subtítulo
- posible botón `Abrir registro`
- descripción contextual, si está disponible
- notas del nodo
- botón para eliminar el nodo

### Abrir el registro vinculado

Si el nodo está vinculado a:

- un lugar
- un personaje

puedes abrir directamente el formulario correspondiente.

Si en cambio el nodo está vinculado a otro **mapa conceptual**, el botón abre ese mapa y además mantiene un pequeño historial de navegación entre mapas.

### Descripción contextual del nodo

Para algunos tipos de nodo, el inspector también muestra una descripción real que ya existe en la aplicación:

- para un **lugar**, muestra la `Descripción DM`
- para un **personaje**, muestra la descripción del personaje

### Notas del nodo

Cada nodo tiene también sus propias notas, separadas del registro de origen.

## Si seleccionas un recuadro

Cuando seleccionas un recuadro, el inspector muestra:

- título del recuadro
- número de elementos contenidos
- notas del recuadro
- botón para eliminar el recuadro

## Si seleccionas una conexión

Cuando seleccionas una flecha, el inspector muestra:

- resumen de la conexión
- nota de la flecha
- botón para eliminar la conexión

Las notas en las conexiones son muy útiles cuando quieres dar un significado más preciso a la relación, por ejemplo:

- alianza
- dependencia
- parentesco
- paso
- causa y efecto

## Si no seleccionas nada

Cuando no hay ningún elemento seleccionado, el inspector muestra un resumen del mapa:

- nombre del mapa
- número de nodos
- número de conexiones

## Zoom y navegación

La pantalla admite:

- zoom
- pan del canvas
- gestos de pinza
- uso rápido de atajos con ratón y trackpad

## Imágenes en los nodos

Los nodos vinculados a lugares o personajes también pueden usar la imagen de portada del registro vinculado como fondo visual.

## Mapas conceptuales conectados entre sí

Uno de los usos más potentes del sistema es la posibilidad de vincular un mapa conceptual con otro.

Esto permite construir:

- un mapa general de la aventura
- mapas secundarios para áreas específicas
- mapas especializados para personajes, facciones o subtramas

## Cuándo conviene usarlos

Los mapas conceptuales son especialmente útiles cuando quieres:

- planificar una campaña larga
- visualizar relaciones complejas
- organizar personajes y lugares en bloques
- preparar subtramas
- tener una vista estratégica que no dependa de textos largos

## Diferencia respecto a Lugares

La sección `Lugares` organiza la aventura en el plano espacial y de contenido.

Los **mapas conceptuales**, en cambio, organizan la campaña en el plano relacional.

En resumen:

- `Lugares` = estructura del mundo y contenido contextual
- `Mapas conceptuales` = estructura lógica, narrativa y relacional

## Diferencia respecto a los mapas interactivos

Los **mapas interactivos** sirven para navegar lugares reales con marcadores sobre un mapa gráfico.

Los **mapas conceptuales** sirven en cambio para conectar conceptos, personajes, lugares e ideas.

## Buenas prácticas

Para usar bien los mapas conceptuales conviene:

- mantener un mapa general de la aventura
- crear mapas más pequeños para áreas o capítulos
- usar recuadros para separar grupos de nodos
- usar nodos libres para ideas que aún no tienen una ficha real
- anotar nodos y flechas con notas breves pero útiles

## En resumen

Los mapas conceptuales de DnDino son una herramienta de organización avanzada.

Permiten construir una visión visual y navegable de la campaña conectando:

- lugares
- personajes
- otros mapas
- notas libres
- relaciones expresadas con flechas

!!! tip
    Si una campaña se vuelve compleja, prueba a usar un mapa conceptual general para la visión de conjunto y mapas más pequeños para ciudades, facciones o subtramas concretas. Es una de las formas más eficaces de no perder el hilo.
