# FAQ

Esta sección reúne respuestas rápidas a las preguntas más habituales sobre DnDino.

Si necesitas una explicación completa de una pantalla concreta, lo mejor es abrir después la página específica de la guía. La FAQ está pensada sobre todo para los casos prácticos más frecuentes.

## ¿Cómo retomo enseguida mi última campaña?

Abre `Inicio` y usa la tarjeta de la **última aventura**.

Desde ahí puedes:

- abrir directamente el panel de la aventura
- ir al último lugar visitado, si está disponible

Es la forma más rápida de volver al trabajo sin pasar cada vez por la lista completa de aventuras.

## ¿Cuál es la diferencia entre ficha base, personaje de aventura, presencia de lugar y participante de combate?

La **ficha base** es el registro general del personaje o de la criatura.

A partir de esa ficha, DnDino puede crear registros contextuales separados:

- el **personaje de aventura**, usado dentro de una campaña
- la **presencia de lugar**, usada en los lugares
- el **participante de combate**, usado durante el encuentro

Este sistema sirve para mantener separados:

- nombres contextuales
- iniciativa
- PG actuales
- notas del DM
- estado local del combate o del lugar

En otras palabras, la ficha base sigue siendo la referencia general, mientras que los registros contextuales permiten trabajar de forma práctica durante la partida.

## ¿Cómo añado un héroe a la aventura?

Abre el `Panel de Aventura` y entra en la sección `Personajes`.

Desde ahí puedes:

- añadir un personaje existente
- crear un personaje nuevo con `Crear personaje`

Si creas un personaje nuevo desde el selector, al guardar vuelves al panel de selección y la lista se actualiza inmediatamente.

## ¿Cómo añado una presencia a un lugar?

Abre el lugar y ve a la sección `Presencias`.

Desde ahí puedes añadir:

- un héroe ya vinculado a la aventura
- un `PNJ`
- un `Monstruo`

Recuerda esta diferencia importante:

- un `PNJ` sigue siendo único dentro de ese lugar
- un `Monstruo` se puede añadir varias veces

Esto permite tener varias instancias del mismo monstruo en un mismo lugar, evitando a la vez duplicados no deseados de PNJ.

## ¿Puedo cambiar el nombre de un monstruo sin modificar su ficha base?

Sí.

Esa es precisamente una de las razones por las que DnDino usa registros contextuales.

Puedes renombrar un monstruo:

- en el precombate
- en las presencias de los lugares
- en otros contextos locales donde el nombre operativo necesite ser más cómodo de leer

Esto no cambia el nombre de la ficha base original.

## ¿Cómo enlazo rápidamente un personaje o un lugar dentro de una descripción?

En los campos de texto compatibles con enlaces internos, usa el comando `Link`.

Desde ahí puedes crear enlaces a:

- personajes
- lugares
- conjuros
- reglas
- dotes

Esto resulta muy útil:

- en `Lugares`, para enlazar otros lugares o personajes citados en la descripción
- en `Personajes`, sobre todo en `Ataques`, para enlazar tiradas o referencias útiles

## ¿Para qué sirven los enlaces en los Ataques de los monstruos?

Sirven para convertir un texto descriptivo en una herramienta operativa.

En los campos rich text de los ataques puedes insertar enlaces como:

- `Ataque completo`
- `Tirada libre`
- `Tirar dados`
- `Tirada de ataque`

Esto permite:

- lanzar dados rápidamente
- aplicar daño a los objetivos
- enlazar otras entradas de la aplicación

Es una de las formas más eficaces de hacer realmente útil la ficha de un monstruo durante el combate.

## ¿Estoy obligado a usar las tiradas automáticas del combate?

No.

DnDino ofrece muchas automatizaciones, pero no te obliga a utilizarlas.

Puedes seguir:

- tirando dados físicos en mesa
- leyendo los resultados de forma tradicional
- aplicando el daño manualmente

La aplicación te ayuda sobre todo a eliminar el trabajo repetitivo de actualizar PG y hacer cálculos mentales.

## ¿El combate funciona bien con un solo monitor?

Sí.

`Combate Flat` funciona bien incluso en una sola pantalla.

La doble pantalla con la `Ventana de Jugadores` es muy útil para la presentación, pero no es un requisito. En un solo monitor puedes usar el combate sin problemas y decidir desde los ajustes cómo debe comportarse la ventana de jugadores.

## ¿Puedo decidir cuánta información ven los jugadores durante el combate?

Sí.

En `Ajustes > Combate`, entre otras cosas, puedes decidir si los jugadores ven:

- la ronda
- los PG
- las condiciones
- el siguiente turno
- el nombre real de los enemigos
- detalles de PNJ y monstruos

Esto te permite elegir entre un combate más transparente o uno más propio de una pantalla de DM.

## ¿Cómo funciona el resumen final del combate?

Al final del combate, DnDino cierra el encuentro y sincroniza los datos contextuales con los registros enlazados.

Además:

- el DM ve el resumen final dentro del combate
- los jugadores pueden ver un resumen en la `Ventana de Jugadores`, si la opción está activa

El resumen público está centrado en los personajes y no en los enemigos.

## ¿Qué ocurre si un héroe baja de 0 PG?

Los héroes pueden bajar a valores negativos.

La regla que maneja la aplicación es esta:

- entre `0` y `-(PG máximos - 1)`, el héroe queda `Inconsciente`
- con `-PG máximos` o menos, el héroe muere de forma definitiva

Durante el combate, cuando un héroe está inconsciente, DnDino también muestra el panel de **tiradas de salvación contra la muerte**.

## ¿Cómo muestro una imagen a los jugadores?

DnDino utiliza una ventana dedicada para la presentación a los jugadores.

Puedes usarla:

- durante el combate
- con las imágenes de la aventura
- en otros flujos que admiten presentación

El comportamiento de esta ventana se ajusta en `Ajustes > Medios` y, en parte, en `Ajustes > Combate`.

## ¿Cómo hago una copia de seguridad de mis datos?

Ve a `Ajustes > Base de datos`.

Desde ahí puedes:

- ver dónde se guardan los datos de la app
- abrir la carpeta de datos
- abrir la carpeta de copias
- crear manualmente una instantánea
- restaurar una instantánea
- restaurar desde iCloud, si está configurado

En esa misma sección también puedes decidir:

- la frecuencia de las copias automáticas
- el número máximo de instantáneas que se conservan

## ¿Dónde encuentro información técnica de la base de datos si algo no cuadra?

Ve a `Ajustes > Diagnóstico`.

Ahí puedes comprobar:

- la ruta de la base de datos
- si el archivo existe
- su tamaño
- la fecha de la última modificación
- la versión de SQLite
- las tablas encontradas y el número de registros

Es la sección adecuada si quieres saber si un problema es solo visual o afecta realmente a los datos guardados.

## ¿Cómo contacto con soporte?

Abre `Ajustes > Soporte`.

Desde ahí puedes:

- enviar una solicitud de soporte
- enviar una sugerencia
- copiar el correo de contacto

Usa `Soporte` cuando algo no funcione o no quede claro. Usa `Sugerencia` cuando quieras proponer una mejora o una función nueva.

!!! tip
    Si una respuesta aquí te parece demasiado breve, usa la FAQ como punto de partida y luego abre la página específica de la guía, por ejemplo `Personajes`, `Lugares`, `Combate` o `Ajustes`.
