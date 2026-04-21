# Héroes, PNJ y Monstruos

La sección **Héroes, PNJ y Monstruos** reúne todas las fichas base de los personajes de la aplicación. Es el lugar donde se crean, se modifican y se clonan los registros que luego podrán vincularse a aventuras, lugares y combates.

Esta página es importante porque en DnDino existen **varios niveles de personaje**, cada uno con un propósito distinto:

- la **ficha base**
- el **personaje de aventura**
- la **presencia en un lugar**
- el **participante en combate**

No son duplicados inútiles: sirven para mantener **datos contextuales separados**, como nombre visible, puntos de golpe, condiciones, iniciativa y notas del DJ, sin perder el vínculo con la ficha original.

## Ficha base

La **ficha base** es el registro principal guardado en la sección `Héroes, PNJ y Monstruos`.

Aquí defines todo lo que pertenece al personaje de forma general:

- nombre
- tipo: `Héroe`, `PNJ` o `Monstruo`
- raza, clase, tamaño, alineamiento
- características
- CA, PG máximos, velocidad, iniciativa
- descripción, habilidades, ataques
- imágenes vinculadas
- conjuros vinculados
- equipamiento y otros datos de referencia

La ficha base no representa automáticamente a un personaje “presente” en una aventura, un lugar o un combate. Es el modelo del que parten los niveles posteriores.

## Crear, modificar y clonar un personaje

Para crear una nueva ficha:

1. abre `Héroes, PNJ y Monstruos`
2. pulsa el botón de añadir
3. completa el formulario del personaje
4. guarda el registro

Puedes crear:

- héroes
- PNJ
- monstruos

El tipo elegido influye en campos y comportamientos posteriores. Por ejemplo:

- para los **héroes** tiene sentido hablar de presencia en la aventura, inspiración y estado contextual
- para los **monstruos** cobran más importancia el VD, los ataques y el uso múltiple en contextos operativos

Si abres una ficha existente, puedes modificar el registro base en todos sus apartados. Los cambios hechos aquí actualizan el registro de origen, pero no siempre sobrescriben automáticamente todos los registros contextuales ya creados en aventuras, lugares o combates. Esto es intencional.

La **clonación** crea una nueva ficha base a partir de una ya existente, copiando también elementos vinculados como:

- campos de la ficha
- conjuros vinculados
- ataques estructurados
- imágenes vinculadas

Es especialmente útil cuando quieres:

- crear variantes similares del mismo monstruo
- partir de un PNJ ya preparado
- construir rápidamente varias fichas con una estructura parecida

## Enlaces internos en los textos del personaje

Una de las funciones más útiles de la ficha base, sobre todo para **PNJ** y **Monstruos**, es el sistema de **enlaces internos** en los campos rich text.

Esta función es especialmente valiosa en la sección **Ataques**, porque transforma el texto descriptivo en herramientas operativas listas para usar durante la sesión y en combate.

En la práctica puedes insertar enlaces que abren directamente:

- una tirada de dados
- una tirada de ataque
- un ataque completo con daño
- un personaje
- un lugar
- un conjuro
- una dote
- una regla del glosario

## Dónde conviene usarlos

Los enlaces internos son especialmente útiles en campos rich text como:

- `Ataques`
- `Habilidades especiales`
- `Descripción`
- otros campos descriptivos donde quieras referencias rápidas

El caso más útil sigue siendo **Ataques**, porque te permite hacer clic de inmediato sobre:

- la tirada para impactar
- los dados de daño
- un ataque completo ya preparado

Para los monstruos es muy cómodo, porque reduce el tiempo que se pierde leyendo fórmulas o reconstruyendo tiradas a mano.

## Cómo insertar un enlace

El flujo correcto es este:

1. abre un campo rich text de la ficha
2. selecciona el texto que quieres convertir en enlace, o coloca el cursor donde quieras insertarlo
3. pulsa el botón `Enlace`
4. elige el tipo de enlace en el selector
5. confirma la creación

Dependiendo del texto seleccionado, el selector puede proponerte enlaces automáticos ya preparados.

## Los cuatro enlaces más útiles para tiradas

### Tirada libre

`Tirada libre` es el enlace más flexible. Siempre está disponible en el selector y sirve cuando quieres crear una tirada configurable sin seguir una estructura rígida.

Es útil para:

- una fórmula completa como `1d6+3`
- un dado simple como `1d20`
- una fórmula que quieras ajustar justo antes de tirar

### Tirar dados

`Tirar dados` solo aparece si el texto seleccionado es una **fórmula de dados válida**.

Ejemplos válidos:

- `1d6`
- `2d8+4`
- `4d4 + 1`

Este enlace es ideal para daño individual, dados de curación, efectos aleatorios y tiradas rápidas separadas.

### Tirada de ataque

`Tirada de ataque` solo aparece si el texto seleccionado es un **modificador válido**, y no una fórmula completa `1d20`.

Ejemplos válidos:

- `+5`
- `-1`
- `0`
- `2`

Cuando creas este enlace, DnDino sabe que debe hacer un **1d20** usando ese modificador. Es perfecto para líneas legibles como:

- `Mordisco +6`
- `Garras +4`

### Tirada de ataque y daño

`Tirada de ataque y daño` es el enlace más potente para la sección **Ataques**.

Siempre está disponible en el selector y abre un configurador dedicado en el que puedes definir:

- modificador de la tirada para impactar
- posible umbral de crítico
- hasta tres fórmulas de daño
- título de cada componente de daño

Es la mejor forma de construir un ataque completo de monstruo o PNJ, porque un solo enlace puede reunir:

- la tirada de ataque
- el daño principal
- daños secundarios
- daño adicional

En combate, este enlace es especialmente útil porque el popover asociado también puede usarse para aplicar el daño a los objetivos elegidos.

## Ejemplo práctico para Ataques

Una forma muy eficaz de escribir un ataque de monstruo es mantener el texto legible para el Director y hacer clicables solo los puntos realmente útiles.

Por ejemplo:

- `Mordisco +6, alcance 1,5 m, un objetivo. Impacto: 1d8+4 perforante.`

Después puedes convertir:

- `+6` en `Tirada de ataque`
- `1d8+4` en `Tirar dados`

o crear directamente un único enlace `Tirada de ataque y daño` sobre el nombre del ataque o una parte de la línea.

## Vincular lugares, personajes y otras referencias

El sistema de enlaces no sirve solo para tiradas.

En campos descriptivos también puedes crear enlaces hacia otros contenidos de la app, como:

- un `Lugar`
- otro `Personaje`
- un `Conjuro`
- una `Dote`
- una `Regla`

Cuando pulsas `Enlace`, el selector también intenta usar el texto seleccionado como filtro inicial:

- si encuentra una coincidencia real en el nombre de los registros, se abre ya filtrado
- si no encuentra resultados reales, el filtro inicial se vacía y ves la lista completa

## Personajes de aventura

El **personaje de aventura** es el nivel que vincula una ficha base con una campaña concreta.

Este registro sirve para gestionar valores que solo tienen sentido **dentro de una aventura**, por ejemplo:

- puntos de golpe actuales
- puntos de golpe temporales
- condiciones
- estado
- inspiración heroica

En otras palabras:

- la ficha base dice **quién es** el personaje
- el personaje de aventura dice **cómo se encuentra** ese personaje dentro de esa campaña

## Presencias en los lugares

La **presencia en un lugar** es otro registro distinto. Sirve para indicar que un personaje o criatura está presente en un lugar concreto, con un nombre y, si hace falta, un estado local.

En el formulario `Añadir presencia al lugar` existen dos posibles orígenes:

- `Personaje de aventura`
- `PNJ / Monstruo`

### Presencia desde personaje de aventura

Si eliges `Personaje de aventura`, el registro del lugar queda vinculado a un personaje ya presente en la campaña.

En este caso:

- la presencia mantiene el vínculo con el personaje de aventura
- no crea una copia autónoma del personaje
- en el mismo lugar no puedes añadir dos veces al mismo personaje de aventura

### Presencia desde PNJ / Monstruo

Si eliges `PNJ / Monstruo`, el lugar crea una **presencia local clonada** a partir de una ficha base de tipo `PNJ` o `Monstruo`.

Este registro tiene sus propios datos locales, como:

- nombre visible
- PG actuales
- PG temporales
- condiciones
- estado
- disposición
- notas del DJ

Aquí el comportamiento cambia según el tipo:

- los **Monstruos** pueden tener varias presencias locales en el mismo lugar
- los **PNJ** se mantienen únicos dentro del mismo lugar y no vuelven a ofrecerse en el selector

Cuando añades varias instancias del mismo monstruo, DnDino propone automáticamente un nombre incremental, por ejemplo:

- `Goblin 2`

## Por qué existe el nombre visible

Tanto las presencias en los lugares como los participantes en combate tienen un campo `Nombre visible`.

Este campo sirve para mantener un nombre **contextual** sin tener que renombrar la ficha base. Es útil, por ejemplo, cuando quieres:

- distinguir copias similares de la misma criatura
- dar un nombre concreto a un PNJ en un solo lugar
- usar un nombre distinto en combate sin cambiar el registro de origen

## Participantes en combate

El **participante en combate** es el nivel operativo usado durante el encuentro.

Un participante puede nacer de tres fuentes distintas:

- un **personaje de aventura**
- una **presencia del lugar**
- una **ficha base**

Cada participante tiene su propio registro específico de combate, con datos como:

- nombre visible
- iniciativa
- CA
- PG máximos
- PG actuales
- PG temporales
- condiciones
- estado
- tiradas de salvación contra la muerte
- orden dentro de la ronda

### Participantes desde personaje de aventura

Si el participante procede de un personaje de aventura:

- mantiene el vínculo con el personaje de campaña
- al final del combate, los valores finales se sincronizan de nuevo con el registro de aventura

### Participantes desde presencia del lugar

Si el participante procede de una presencia del lugar:

- mantiene el vínculo con ese registro del lugar
- si esa presencia usa estado local, el combate puede volver a sincronizar PG, condiciones y estado sobre el registro del lugar

### Participantes desde ficha base

Si el participante nace directamente de una ficha base:

- el registro de combate usa esa ficha como origen
- el comportamiento respecto a instancias múltiples depende del tipo

En el selector de combate:

- un registro base de tipo **Monstruo** puede añadirse varias veces
- un registro base de tipo **PNJ** o **Héroe** no se ofrece más de una vez en el mismo combate

## Sincronización entre niveles

Algunos valores se sincronizan entre niveles, pero no todo se sobrescribe siempre.

### De la ficha base hacia los contextos

La ficha base aporta:

- la identidad del personaje
- estadísticas de referencia
- conjuros
- ataques
- imágenes

### De los contextos hacia los registros vinculados

Las capas operativas pueden sincronizar datos situacionales, sobre todo:

- PG
- condiciones
- estado
- algunas notas locales

En combate, por ejemplo, los valores finales pueden volver a:

- el personaje de aventura vinculado
- la presencia del lugar vinculada, si esa presencia usa estado local

## Diferencia práctica entre los niveles

Una forma simple de recordarlo es esta:

- `Ficha base`: el **modelo general** del personaje
- `Personaje de aventura`: el **estado del personaje dentro de la campaña**
- `Presencia en el lugar`: la **presencia contextual del personaje dentro de un lugar concreto**
- `Participante en combate`: la **versión operativa del personaje dentro del enfrentamiento**

## Cuándo conviene usar cada nivel

### Usa la ficha base cuando:

- necesites crear el personaje
- quieras modificar datos estructurales
- necesites vincular imágenes, conjuros o ataques

### Usa el personaje de aventura cuando:

- quieras vincular un héroe a la campaña
- necesites seguir de forma persistente PG, estado, condiciones e inspiración dentro de la aventura

### Usa la presencia en el lugar cuando:

- quieras poblar un lugar con personajes o criaturas
- quieras dar nombres contextuales a PNJ y monstruos
- quieras crear instancias locales separadas dentro de un lugar

### Usa el participante en combate cuando:

- estés preparando o dirigiendo un enfrentamiento
- necesites iniciativa, PG y condiciones de batalla
- quieras que el combate trabaje con registros contextuales sin ensuciar directamente la ficha base

## En resumen

La sección `Héroes, PNJ y Monstruos` no es solo un archivo de fichas. Es el **nivel de origen** del que nace toda la gestión contextual de personajes dentro de la aplicación.

La lógica general es:

- la **ficha base** define al personaje
- el **personaje de aventura** lo inserta en la campaña
- la **presencia en el lugar** lo contextualiza en un lugar
- el **participante en combate** lo vuelve operativo durante el enfrentamiento

!!! tip
    Si quieres evitar confusiones, recuerda siempre esta diferencia: la ficha base describe al personaje, mientras que aventura, lugar y combate describen su estado en un contexto concreto. No hace falta obsesionarse con la separación teórica; lo importante es que algunos campos solo existen dentro de su propio contexto.
