# Combate

El modo **Combate** de DnDino está pensado para ser el tracker operativo principal del enfrentamiento. Esta página describe el modo de combate estándar de DnDino.

El combate nace siempre en el contexto de un **lugar** y arrastra consigo a los personajes, las presencias locales y los posibles monstruos o PNJ vinculados a esa escena.

Esta página explica todo el flujo:

- preparación del precombate
- gestión de participantes
- inicio del enfrentamiento
- uso del panel del turno actual
- aplicación de daño, curación, condiciones y tiradas de salvación
- integración con la **Ventana de Jugadores**
- cierre del enfrentamiento y resumen final

## Uso con una o dos pantallas

El combate de DnDino funciona muy bien también con **una sola pantalla**: toda la parte operativa permanece en el panel principal y puedes gestionar participantes, turnos, daño, condiciones y el resumen final sin necesidad de un segundo monitor.

Dicho esto, si tienes una configuración con dos pantallas, puedes usar:

- una pantalla principal para el panel de control del DM
- una segunda pantalla o monitor para la **Ventana de Jugadores**

En esta configuración el flujo resulta todavía más cómodo:

- en la pantalla del DM permanecen visibles la lista de participantes, los controles del asalto, el turno actual, los textos de ataque, las notas DM y las ediciones rápidas
- en la pantalla de los jugadores se muestra una presentación limpia del participante activo, con imagen y overlay contextual

En la práctica:

- con una sola pantalla controlas todo el combate desde la pantalla principal
- con dos pantallas separas el panel técnico del DM de la presentación para los jugadores

!!! tip
    La segunda pantalla no es obligatoria. Es simplemente una mejora muy útil cuando quieres mostrar a los jugadores imágenes e información del turno actual sin exponer el panel técnico del DM.

## Cómo funciona la Ventana de Jugadores durante el combate

Cuando el combate se inicia, DnDino puede abrir o actualizar automáticamente la **Ventana de Jugadores**.

Si la presentación para jugadores está activa:

- al principio del combate puede aparecer una breve **intro** con los participantes
- durante el combate la ventana se actualiza al **participante del turno actual**
- al final del enfrentamiento puede aparecer un **resumen final**

Durante el combate, la Ventana de Jugadores no muestra el panel técnico del DM, sino una presentación visual con:

- imagen del participante activo
- nombre mostrado a los jugadores
- información de overlay, si está activada

El overlay puede incluir:

- asalto actual
- PG actuales, máximos y temporales
- condiciones
- siguiente turno

La información sobre enemigos puede gestionarse por separado respecto a la de los héroes.

## Ajustes de la Ventana de Jugadores y de la segunda pantalla

Las opciones más importantes se encuentran en **Ajustes**, dentro del área dedicada a la presentación del combate y de la ventana de jugadores.

### Apertura y comportamiento general

Los ajustes principales son:

- `Abrir ventana de jugadores incluso con un solo monitor`
- `Mostrar controles de la ventana de jugadores en la barra superior`
- `Mostrar intro de combate a los jugadores`
- `Mostrar resumen final a los jugadores`

#### Abrir ventana de jugadores incluso con un solo monitor

Si esta opción está activa, DnDino puede abrir automáticamente la Ventana de Jugadores incluso cuando trabajas con un solo monitor.

Si está desactivada:

- con un solo monitor la ventana no se abre automáticamente
- si ya está abierta, seguirá actualizándose igualmente

#### Mostrar controles de la ventana de jugadores en la barra superior

Si activas esta opción, en la barra superior aparecen botones para:

- abrir manualmente la ventana de jugadores
- cerrarla manualmente

#### Mostrar intro de combate a los jugadores

Cuando pulsas `Iniciar enfrentamiento`, la Ventana de Jugadores puede mostrar una breve introducción con:

- título del enfrentamiento
- participantes implicados
- número de participantes

Si desactivas esta opción, el combate pasa directamente a la presentación del primer participante activo.

#### Mostrar resumen final a los jugadores

Cuando el combate termina, la Ventana de Jugadores puede mostrar un resumen final.

El resumen para jugadores solo muestra datos útiles para ellos, como:

- daño infligido por los héroes
- daño sufrido por los héroes
- imagen del enemigo más peligroso

El resumen final para jugadores permanece visible hasta que cambies el contenido de la ventana o la cierres.

### Información mostrada durante el turno

Los ajustes que controlan el overlay del participante activo son:

- `Mostrar asalto en la ventana de jugadores`
- `Mostrar PG en la ventana de jugadores`
- `Mostrar condiciones en la ventana de jugadores`
- `Mostrar siguiente turno en la ventana de jugadores`

### Información sobre enemigos, monstruos y PNJ

Para participantes que no son héroes existen controles dedicados:

- `Mostrar detalles de PNJ y monstruos a los jugadores`
- `Mostrar condiciones de los enemigos a los jugadores`
- `Mostrar nombres de los enemigos a los jugadores`

Esto permite decidir si la Ventana de Jugadores debe:

- mostrar la criatura de una forma más evocadora
- o mostrar también datos más técnicos

## Dónde se abre el combate

El combate se crea desde el contexto de un **lugar**. Una vez abierto, DnDino muestra una pantalla dividida en dos columnas principales:

- a la izquierda, el tracker operativo del combate
- en el centro, el panel principal de la escena o del turno actual

Antes de empezar el combate, el panel central muestra el **Resumen previo al combate**.

Cuando el enfrentamiento está activo, ese mismo panel se convierte en el área del **Turno actual**.

Cuando el combate ha terminado, el panel central muestra el **Resumen final del enfrentamiento** para el DM.

## Estructura general de la pantalla

### Columna izquierda

La columna izquierda contiene:

- `Control de combate`
- encabezado de la lista de participantes
- lista ordenada de participantes

La lista queda enmarcada por dos líneas decorativas y funcionales:

- `Inicio del asalto`
- `Fin del asalto`

### Panel central

El panel central cambia según el estado del combate:

- **antes de empezar** muestra el resumen previo al combate
- **durante el enfrentamiento** muestra al participante del turno actual
- **al final del combate** muestra el resumen final del DM

## Precombate

El precombate sirve para preparar el enfrentamiento antes de lanzar el primer turno.

Es la fase en la que más conviene ajustar tres cosas:

- el nombre de los monstruos, cuando quieres distinguirlos mejor en mesa
- la iniciativa de los héroes, introduciéndola manualmente
- la iniciativa de PNJ y monstruos, tirándola automáticamente o escribiéndola a mano

## Resumen previo al combate

La tarjeta inicial muestra una panorámica rápida con métricas como:

- participantes
- héroes
- aliados
- enemigos
- PG totales de los enemigos
- participantes ya en condiciones críticas

## Iniciativa de personajes

La sección `Iniciativa de personajes` reúne a los héroes principales y permite modificar rápidamente la iniciativa antes de ordenar el enfrentamiento.

En cada fila encontrarás:

- nombre del participante
- subtítulo contextual
- campo de iniciativa
- botón `Eliminar`

## PNJ y monstruos

La sección `PNJ y monstruos` está dedicada a los participantes no héroes.

Aquí puedes:

- modificar rápidamente la iniciativa
- renombrar al vuelo monstruos y PNJ para distinguirlos mejor
- usar `Init PNJ/Monstruos` para tirar automáticamente la iniciativa
- introducir manualmente el valor si prefieres usar una tirada hecha fuera de la aplicación
- eliminar rápidamente a un participante con `Eliminar`

## Acciones principales del precombate

En el resumen previo al combate las acciones principales son:

- `Añadir`
- `Ordenar`
- `Iniciar enfrentamiento`

Si al menos un participante sigue con iniciativa `0`, DnDino pide confirmación antes de empezar.

## De dónde pueden salir los participantes

El panel de añadir participantes puede recurrir a tres orígenes:

- `Héroes`
- `Presencias del lugar`
- `Globales`

### Héroes

Aquí aparecen los personajes de aventura ya vinculados a la campaña. Cada héroe solo puede entrar una vez en el combate.

### Presencias del lugar

Aquí aparecen los personajes que ya están presentes en el lugar desde el que nace el combate. Su estado local puede reutilizarse como base para el enfrentamiento.

### Globales

Aquí aparecen fichas base no vinculadas ya como héroes de la aventura.

En el caso de los globales:

- los `Monstruos` pueden añadirse varias veces
- los `Héroes` y `PNJ` globales no pueden duplicarse como fichas globales puras

## Control de combate

Una vez iniciado el enfrentamiento, el panel `Control de combate` permanece fijo encima de la lista y contiene las acciones principales del asalto.

Las filas de botones son:

1. `Añadir` y `Ordenar`
2. `Iniciar/Pausar` o `Reanudar` y `Finalizar`
3. `Ant.` y `Sig.`

Además, si existe un último ataque reversible, aparece también:

- `Deshacer último ataque`

## Lista de participantes

La lista de la izquierda es el corazón del seguimiento táctico.

Cada fila cerrada muestra:

- posición en el orden del turno, por ejemplo `1/8`
- nombre del participante
- hasta tres iconos de condiciones
- distintivo `Turno` si es el participante activo
- CA
- PG
- PG temporales
- iniciativa

El participante en turno actual se destaca mucho más que los demás:

- franja lateral de color
- borde reforzado
- fondo más cálido
- desplazamiento automático para mantenerlo visible

La fila también usa efectos de impacto cuando el participante:

- recibe daño
- muere
- es restaurado mediante un undo

## Menú contextual en una fila

Con **clic derecho** sobre la tarjeta del participante puedes abrir el menú contextual.

Actualmente la acción disponible es:

- `Eliminar`

## Expansión de la fila del participante

Al hacer clic en la fila, el participante se expande y muestra sus controles rápidos.

En la parte expandida encontrarás:

- nombre editable
- campos numéricos rápidos:
  - iniciativa
  - PG
  - PG temporales
  - CA
- botones de acción
- bloque de condiciones
- acceso a habilidades, especiales y conjuros, si existen

## Botones rápidos de la fila

Las acciones rápidas pueden incluir:

- `Atacar`
- `Daño`
- `Curar`
- `Salvación`
- `Notas DM`
- `Editar`
- `Condiciones`

Algunos botones solo aparecen cuando tienen sentido para ese participante.

## Atacar

`Atacar` abre un popover donde puedes seleccionar:

- uno o varios objetivos
- el daño a aplicar

El selector de objetivos usa una lista compacta con:

- nombre
- CA
- PG
- condiciones

El orden de los objetivos no es aleatorio. DnDino intenta proponerte primero los participantes más lógicos según quién esté atacando.

En general:

- si ataca un **Héroe**, primero se proponen los **enemigos**, luego aliados, luego neutrales y por último monstruos de menor prioridad
- si ataca un participante no héroe, primero se proponen los **héroes**, luego aliados, luego neutrales y por último enemigos menos adecuados

Dentro de cada grupo, los nombres se ordenan alfabéticamente.

El popover no preselecciona nunca un objetivo de forma automática: la elección debe ser manual.

Cuando aplicas un ataque a varios objetivos:

- el daño se aplica a todos los seleccionados
- el banner superior muestra varias líneas, una por cada objetivo golpeado
- el undo del último ataque conserva todo el grupo

## Daño y Curación

`Daño` aplica daño directo al participante.

`Curar` aplica curación directa.

## Salvación

`Salvación` abre el popover de **tirada de salvación** basado en las características del participante.

## Condiciones

El botón `Condiciones` abre el popover dedicado a gestionar estados activos.

Desde aquí puedes:

- añadir condiciones
- elegir duración y reglas de expiración
- vincular el final de una condición al turno de otro participante

## Notas DM

El botón `Notas DM` siempre está visible.

Abre un popover editable donde puedes escribir notas contextuales sobre el participante. El contenido se guarda al cerrar el popover.

## Editar

`Editar` abre el panel de edición del participante.

Sirve cuando necesitas intervenir de forma más profunda sobre:

- iniciativa
- CA
- PG máximos, actuales y temporales
- rol en combate
- datos contextuales vinculados

## Turno actual

Cuando el combate está activo, el panel central se centra por completo en el participante cuyo turno está en curso.

La tarjeta superior muestra:

- imagen del participante
- nombre
- subtítulo
- CA
- PG
- PG temporales
- iniciativa
- velocidad
- inspiración, si el participante es un héroe de aventura
- condiciones activas
- características principales

## Paneles centrales durante el turno

Debajo del resumen del turno solo aparecen los paneles que tienen contenido real.

Las secciones posibles son:

- `Ataques`
- `Habilidades especiales`
- `Habilidades`
- `Descripción`
- `Conjuros`

Todos estos paneles son plegables.

Además, usan un ligero acento visual:

- `Ataques` rojo
- `Habilidades` amarillo
- `Habilidades especiales` verde
- `Conjuros` celeste
- `Descripción` gris

## Ataques y enlaces internos

La sección `Ataques` es uno de los puntos más fuertes del combate flat.

Si has preparado enlaces internos dentro de los ataques de la ficha base, puedes usarlos directamente durante el combate.

En particular, el enlace **Ataque completo** es muy útil porque:

- ejecuta tirada de ataque y daño en el mismo popover
- permite seleccionar uno o varios objetivos
- propone automáticamente `Daño a aplicar`
- te deja excluir líneas de daño individuales si has tirado varios componentes y solo quieres aplicar algunos
- cierra el popover en cuanto aplicas el daño

Esto hace que los ataques de monstruos se resuelvan mucho más rápido en mesa.

## Personajes con 0 PG o menos

En combate, los **Héroes** siguen una regla distinta de la de PNJ y monstruos.

### Héroes

Los héroes pueden bajar de `0` PG.

La regla es:

- entre `0` y `-(PG máximos - 1)`, el personaje está **Inconsciente**
- a `-PG máximos` o menos, el personaje muere de forma definitiva

Cuando un héroe está a `0` PG o menos pero no ha muerto definitivamente:

- permanece en el enfrentamiento
- en el panel central aparece la tarjeta `Tiradas de salvación contra la muerte`

Esta tarjeta registra:

- éxitos
- fallos

y permite marcar rápidamente:

- `Éxito`
- `Fallo`

Con 3 éxitos, el personaje vuelve a `1` PG. Con 3 fallos, muere.

### PNJ y Monstruos

Para los no héroes, el comportamiento es más simple:

- a `0` PG o menos, están muertos

## Turnos, asaltos y participantes fuera del ciclo

Dentro del ciclo de turnos:

- los héroes muertos definitivamente quedan excluidos
- PNJ y monstruos con `0` PG o menos quedan excluidos

Esto significa que un héroe **Inconsciente** todavía puede tener turno, precisamente porque aún debe gestionar sus tiradas de salvación contra la muerte.

## Banner de impacto y feedback visual

Cuando un ataque impacta, DnDino muestra un gran banner en la parte superior con un resumen inmediato.

Por ejemplo:

- quién golpeó
- quién fue golpeado
- cuánto daño se aplicó
- si el golpe mató al objetivo

Si hay varios objetivos, el banner muestra varias líneas dentro del mismo cuadro.

La **Ventana de Jugadores** también puede mostrar la animación del golpe, incluyendo a todos los objetivos implicados en el mismo ataque multiblanco.

## Deshacer último ataque

Cuando aplicas un ataque, aparece el panel:

- `Deshacer último ataque`

Debajo del botón aparece un breve resumen de lo que acaba de suceder.

Si el último ataque golpeó a varios objetivos, el panel muestra la lista completa de filas que serán restauradas.

Cuando confirmas el undo:

- los objetivos vuelven a su estado anterior
- aparece una notificación de restauración
- también se actualiza el feedback visual de las tarjetas

## Resumen final del enfrentamiento

Cuando termina el combate, el panel central pasa al **Resumen final del enfrentamiento** para el DM.

Esta pantalla muestra:

- asaltos totales
- duración
- enemigos abatidos
- daño infligido
- daño sufrido

## Qué se sincroniza al final

Cuando cierras el combate, DnDino guarda el resultado en los registros vinculados.

Para los héroes de aventura se sincronizan:

- PG actuales
- PG temporales
- condiciones manuales
- estado final

Para las presencias del lugar con estado local se sincronizan:

- PG actuales
- PG temporales
- condiciones manuales
- estado final

Además, el combate actualiza también los datos de la **sesión en vivo**, incluidos:

- daño infligido
- daño sufrido
- héroes caídos

## Cuándo brilla más el combate

El combate de DnDino da lo mejor de sí cuando lo usas así:

1. preparas bien el precombate
2. usas doble pantalla con la **Ventana de Jugadores**
3. aprovechas los enlaces en los `Ataques` de monstruos y PNJ
4. mantienes al DM en el tracker y a los jugadores en la presentación

!!! tip
    Aunque el combate ofrece muchas automatizaciones para tiradas, ataques completos y aplicación rápida del daño, DnDino sigue dejando espacio para un uso más clásico de los dados. Puedes seguir tirando físicamente o resolver la tirada fuera de la aplicación y usar el combate sobre todo para aplicar los valores de forma rápida y coherente, evitando la parte más incómoda: recalcular a mano los cambios y actualizaciones de puntos de golpe cada vez.
