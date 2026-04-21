# Página de inicio

La **página de inicio** es la pantalla de entrada de DnDino. No es un panel operativo pensado para gestionar directamente todos los módulos de la aplicación, sino un **punto de acceso rápido** diseñado para:

- retomar de inmediato la última aventura usada
- volver rápidamente a las herramientas principales
- orientarte al abrir la aplicación

La página de inicio tiene por tanto dos funciones principales:

- **reanudación rápida**, si ya tienes una campaña activa
- **inicio guiado**, si estás empezando desde cero

## Estructura de la pantalla

La Home está compuesta por tres áreas principales:

1. un encabezado de bienvenida
2. un panel principal dedicado a la última aventura o al arranque inicial
3. una cuadrícula con las herramientas principales de la aplicación

## Encabezado de bienvenida

En la parte superior de la pantalla aparece un saludo inicial.

Si en los ajustes se ha introducido el nombre del Dungeon Master, la Home muestra un mensaje personalizado, por ejemplo:

- `¡Hola, Marcos!`

En caso contrario aparece una versión genérica:

- `¡Hola, DM!`

Debajo del saludo hay una breve frase que explica el propósito de esta pantalla: retomar el trabajo donde lo dejaste o abrir de inmediato una de las herramientas principales.

## Panel principal

El panel principal cambia según el estado de la aplicación.

### Si ya existe una aventura reciente

Cuando la aplicación encuentra una aventura usada recientemente, la Home muestra una tarjeta grande dedicada a la **última aventura**.

Esta tarjeta contiene:

- el título de la aventura
- una breve descripción, si existe
- un botón `Abrir aventura`
- un posible botón para ir directamente al último lugar visitado
- algunas estadísticas de resumen
- una sección visual con los héroes vinculados a la aventura

Si la aventura tiene una imagen de portada, esa imagen se usa como fondo de la tarjeta. En caso contrario, DnDino muestra un fondo gráfico predeterminado.

#### Botón Abrir aventura

El botón principal de la tarjeta abre directamente el **panel principal de la aventura**, que es el centro operativo de la campaña.

Es la forma más rápida de retomar el trabajo.

#### Botón Ir al último lugar visitado

Si la aplicación conoce el último lugar abierto dentro de la aventura, en la tarjeta aparece también un segundo botón que te lleva directamente allí.

Esto resulta muy útil cuando quieres retomar la exploración o continuar el trabajo sobre una zona narrativa concreta de la campaña.

## Estadísticas de la aventura

En el panel principal se muestran también algunas métricas de resumen de la última aventura.

Las estadísticas visibles son:

- `Misiones`
- `Lugares`
- `Sesiones`
- `Combates`

Estos valores sirven como un vistazo rápido para entender cuánto material se ha construido ya en la campaña.

## Héroes de la aventura

Si la aventura tiene héroes vinculados, en la parte derecha de la tarjeta aparece una sección dedicada a ellos.

Esta área puede mostrar:

- el número total de héroes
- retratos, si están disponibles
- un mensaje invitando a añadir una imagen de portada si aún no la tienen

Cuando solo hay un héroe, el retrato se muestra en mayor tamaño. Cuando hay varios, los retratos se disponen en un conjunto más compacto.

Esta sección tiene una función sobre todo visual: ayuda a reconocer la campaña de un vistazo.

## Cuando todavía no existe ninguna aventura

Si el usuario aún no tiene aventuras disponibles, la Home muestra un panel alternativo pensado para acompañar el primer uso.

En este caso la pantalla presenta:

- el título `Listo para empezar`
- una breve descripción introductoria
- el botón `Ir a aventuras`
- tres pasos sugeridos para empezar a usar DnDino

Los tres pasos mostrados son:

1. crear una aventura
2. añadir personajes
3. construir lugares y misiones

En esta situación, la Home cumple una función de onboarding y acompaña la creación de la primera campaña.

## Herramientas principales

Debajo del panel principal hay una cuadrícula de tarjetas que representan las herramientas principales de la aplicación.

Las secciones accesibles desde la Home son:

- `Aventuras`
- `Héroes, PNJ y Monstruos`
- `Equipo`
- `Reglas`
- `Generador de nombres`
- `Ajustes`

Cada tarjeta contiene:

- un título
- un breve subtítulo descriptivo
- un icono
- un fondo ilustrado dedicado

### Aventuras

Abre la lista de campañas y te permite:

- crear una nueva aventura
- abrir una campaña existente
- retomar el trabajo de preparación

### Héroes, PNJ y Monstruos

Abre la sección que reúne las fichas de criaturas. Desde aquí puedes trabajar con:

- héroes
- PNJ
- monstruos
- datos base vinculados a las fichas

!!! tip
    Con el tiempo verás que muchos personajes también pueden abrirse y modificarse directamente desde dentro de una aventura, sin romper tu flujo de preparación.

### Equipo

Abre la sección dedicada a:

- armas
- armaduras
- herramientas
- equipo

### Reglas

Abre el área de consulta rápida de reglas y referencias. Resulta útil para:

- consultar material de apoyo
- buscar reglas
- abrir contenidos relacionados con el juego

### Generador de nombres

Abre la herramienta para generar rápidamente nombres útiles durante la preparación o la improvisación, por ejemplo para:

- PNJ
- monstruos
- encuentros inesperados

!!! tip
    Durante la sesión, el mini generador de nombres de la barra superior suele ser todavía más cómodo, porque te permite crear nombres sin salir de la pantalla en la que estás trabajando.

### Ajustes

Abre el panel de preferencias globales de la aplicación y de gestión local de la base de datos.

## Cuándo usar la Home

La Home es especialmente útil cuando quieres:

- retomar rápidamente la última campaña
- abrir el panel principal de la aventura más reciente
- volver al último lugar visitado
- acceder rápidamente a las herramientas principales de la aplicación
- empezar una nueva campaña si la base de datos todavía está vacía

!!! tip
    Si trabajas casi siempre en la misma campaña, la tarjeta de la última aventura es la forma más rápida de volver al punto correcto sin tener que pasar cada vez por la lista completa de aventuras.
