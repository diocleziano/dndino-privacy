# Ajustes

La sección **Ajustes** reúne las preferencias globales de DnDino. Aquí no se trabaja sobre una aventura o un personaje concreto, sino que se define **cómo debe comportarse la aplicación en su conjunto**.

Los ajustes influyen sobre todo en:

- el aspecto general de la interfaz
- el comportamiento de la barra superior
- el flujo de `Lugares`
- el comportamiento del `Combate`
- la gestión de imágenes, copias y snapshots
- el soporte y la parte diagnóstica de la base de datos

## Cómo está organizada la pantalla

La página se divide en dos áreas:

- una **barra lateral izquierda** con las categorías
- un **panel principal** a la derecha con las opciones de la sección seleccionada

Las categorías disponibles son:

- `General`
- `Barra superior`
- `Lugares`
- `Combate`
- `Medios`
- `Tema`
- `Base de datos`
- `Diagnóstico`
- `Soporte`
- `Licencias`

Esta estructura separa bien las preferencias de uso diario de las más técnicas, como las copias de seguridad y el diagnóstico.

## General

La sección `General` reúne las preferencias base de la aplicación.

### Perfil DM

Aquí puedes personalizar tu perfil con:

- `Nombre de usuario`
- `Género`

El nombre se reutiliza también en otras partes de la app, por ejemplo en el mensaje de bienvenida de la `Home`.

### Idioma de la interfaz

Puedes decidir si:

- seguir el idioma del sistema
- forzar un idioma concreto de la aplicación

### Confirmaciones globales

La opción `Pedir confirmación antes de eliminar` añade una confirmación antes de acciones destructivas, como eliminaciones o retiradas.

### Metadatos

Dentro de `General` también encontrarás:

- `Mostrar metadatos en la aplicación`

Esta opción decide si los paneles de metadatos deben mostrarse en las pantallas que los soportan.

### Disposición de paneles en el dashboard de aventura

Esta parte es importante si usas con frecuencia el `Dashboard de aventura`.

Puedes:

- arrastrar paneles
- reordenarlos dentro de la columna izquierda o derecha
- moverlos de una columna a otra

### Tema activo

Dentro de `General` también se muestra el **tema actualmente seleccionado** como resumen rápido. El cambio real de tema se hace en la sección `Tema`.

### Guías introductorias

Desde aquí puedes restaurar el comportamiento de primer uso de la aplicación.

El botón `Restablecer primer uso` hace que DnDino vuelva a considerar como no vistas las guías contextuales y los recorridos introductorios.

## Barra superior

La sección `Barra superior` define el comportamiento de las herramientas rápidas presentes en la parte superior de la aplicación.

### Aspecto de la barra superior

Puedes elegir si la barra superior se muestra:

- solo con iconos
- o con iconos y nombre debajo

### Dado predeterminado

DnDino incluye un lanzadados rápido en la barra superior. Aquí puedes elegir el **tipo de dado predeterminado** que se propone al abrirlo.

### Apertura rápida de personajes

Este ajuste controla el comportamiento de la apertura rápida de personajes desde la barra superior.

Puedes decidir si el acceso rápido debe llevar:

- a una vista más orientada a la lectura
- o a un modo más cercano a la edición

### Apertura rápida de reglas

La barra superior también permite abrir rápidamente las `Reglas`.

Desde aquí puedes decidir si ese acceso debe abrir:

- el editor completo
- o una ventana más compacta y orientada a la consulta

### Controles de la ventana de jugadores en la barra superior

La opción `Mostrar controles de la ventana de jugadores en la barra superior` añade controles en la barra para abrir o cerrar manualmente la `Ventana de Jugadores`.

## Lugares

La sección `Lugares` contiene las preferencias globales utilizadas como comportamiento predeterminado en el panel de lugares.

### Rol de presencia predeterminado

Cuando añades una presencia a un lugar, DnDino puede proponer un rol inicial por defecto.

### Mostrar mapas de los lugares padre por defecto

Si activas esta opción, en la pantalla `Lugares` los mapas heredados de los lugares padre se muestran ya visibles.

### Recordar el último lugar visitado

Si está activo, al volver a la pantalla `Lugares` la aplicación intenta restaurar el último lugar seleccionado para esa aventura.

### Cerrar automáticamente el lugar anterior

Este ajuste se aplica durante una **sesión en vivo activa**.

Cuando un lugar se marca como `En visita`, el lugar que antes estaba `En visita` se marca automáticamente como `Visitado`.

## Combate

La sección `Combate` reúne las preferencias globales del sistema de combate.

Aquí encontrarás tanto opciones de presentación como elecciones que influyen en el flujo práctico del enfrentamiento y de la `Ventana de Jugadores`.

## Orden de los paneles centrales

Puedes reordenar el orden de los paneles centrales del combate arrastrando elementos como:

- `Ataques`
- `Habilidades especiales`
- `Habilidades`
- `Conjuros`
- `Descripción`

## Presentación del combate

Esta subsección controla el comportamiento general del combate y de la presentación para los jugadores.

### Mostrar turno a los jugadores por defecto

Si está activo, los nuevos combates empiezan ya con la presentación automática del turno habilitada.

### Abrir la ventana de jugadores incluso con un solo monitor

Este ajuste controla el comportamiento automático de la `Ventana de Jugadores` en configuraciones de una sola pantalla.

### Mostrar automáticamente el detalle del jugador en turno

Cuando cambia el turno, la aplicación puede:

- seleccionar automáticamente al participante activo
- abrir también su detalle

### Ordenar automáticamente por iniciativa al empezar

Cuando pulsas `Iniciar combate`, DnDino puede reordenar automáticamente a los participantes por iniciativa antes de comenzar el asalto.

### Pedir confirmación antes de terminar el combate

Esta opción es importante porque terminar un combate no es solo un cierre visual:

- sincroniza PG y estado en los registros vinculados
- cierra el flujo del enfrentamiento

### Mostrar intro del combate a los jugadores

Si está activa, cuando el combate empieza la `Ventana de Jugadores` muestra una breve introducción con los participantes del enfrentamiento.

### Mostrar resumen final a los jugadores

Si está activa, al final del enfrentamiento la `Ventana de Jugadores` muestra un resumen final con los datos principales de los personajes.

## Información del participante activo

Esta subsección decide qué información del turno actual se muestra a los jugadores.

Puedes elegir si hacer visibles:

- `Asalto`
- `PG`
- `Condiciones`
- `Siguiente turno`

## Información de enemigos y PNJ

Esta parte gestiona por separado lo que ven los jugadores cuando el participante activo es:

- un enemigo
- un monstruo
- un PNJ

Puedes controlar de forma independiente:

- la visibilidad de PG y PG temporales
- la visibilidad de las condiciones
- la visibilidad del nombre real del enemigo

## Medios

La sección `Medios` reúne las preferencias para la gestión de imágenes y de la ventana de presentación.

### Imágenes para jugadores a pantalla completa

Si está activa, las imágenes mostradas a los jugadores se abren en modo pantalla completa.

### Imágenes del DM en el monitor principal

Esta opción hace que la ventana del DM se abra por defecto en la primera pantalla disponible.

### Recordar tamaño de la ventana del DM

Si está activo, al volver a abrir una nueva imagen para el DM la ventana mantiene:

- el último tamaño
- la última posición

## Mantenimiento de medios

La sección `Mantenimiento de medios` cubre el lado más técnico de la gestión de imágenes.

Desde aquí puedes lanzar `Limpiar medios no utilizados`, que comprueba los archivos de imagen guardados por la aplicación y elimina aquellos que ya no están vinculados a ninguna entidad.

## Tema

La sección `Tema` permite elegir la **paleta global** de la aplicación.

Cada tema muestra una pequeña vista previa visual con sus colores principales, para que puedas entender enseguida cómo cambiará la interfaz.

## Base de datos

La sección `Base de datos` es una de las más importantes para la seguridad de los datos.

Aquí encontrarás:

- la ruta de la carpeta de datos
- la ruta de la base SQLite
- la ruta de la carpeta de copias
- información sobre los snapshots más recientes

### Copia de seguridad automática

Puedes elegir:

- la frecuencia de la copia automática
- el número máximo de snapshots automáticos que se conservarán

### Snapshots en la nube

DnDino también gestiona el comportamiento de los snapshots en la nube.

Desde aquí puedes decidir cómo deben comportarse los guardados en la nube y ver el estado actual a través del texto de resumen mostrado en pantalla.

### Acciones principales

En el panel `Base de datos` encontrarás los principales botones de mantenimiento:

- `Abrir carpeta de datos`
- `Abrir carpeta de copias`
- `Crear snapshot...`
- `Restaurar snapshot...`
- `Restaurar desde iCloud`

### Reinicio de la aplicación

La función `Restablecer datos de la aplicación` elimina:

- la base de datos de la aplicación
- los medios de la aplicación

pero conserva las copias ya creadas.

### Últimos snapshots

En la parte inferior de la sección `Base de datos`, DnDino muestra también la lista de los últimos snapshots encontrados.

Para cada uno se muestran:

- nombre del archivo
- fecha
- tamaño

## Diagnóstico

La sección `Diagnóstico` sirve para controlar el estado técnico de la base de datos SQLite utilizada por la aplicación.

Aquí puedes:

- actualizar los datos de diagnóstico
- ver la ruta de la base de datos
- comprobar si el archivo existe
- verificar su tamaño y fecha de modificación
- ver la versión de SQLite

### Tablas

El diagnóstico también muestra la lista de tablas encontradas en la base de datos junto con el número de registros presentes en cada una.

## Soporte

La sección `Soporte` reúne los canales rápidos para contactar con quien desarrolla la aplicación.

Aquí encontrarás:

- el correo de soporte
- el botón `Solicitar soporte`
- el botón `Enviar una sugerencia`
- el botón `Copiar correo`

## Licencias

La sección `Licencias` reúne las referencias legales y de atribución utilizadas por la aplicación.

Actualmente incluye en particular la parte relativa al **System Reference Document 5.2** de Dungeons & Dragons, con referencias:

- al documento SRD
- a la licencia `CC-BY-4.0`

!!! tip
    Si estás configurando DnDino por primera vez, las secciones más útiles para revisar de inmediato son `General`, `Barra superior`, `Combate` y `Base de datos`. Suelen ser las que más influyen en el uso diario y en la seguridad de los datos.
