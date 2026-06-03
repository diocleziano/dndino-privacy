# Importación y exportación

DnDino permite exportar e importar contenido para moverlo entre instalaciones, crear copias de trabajo o compartir material con otros Dungeon Masters.

Las importaciones no sobrescriben automáticamente los datos existentes: antes de guardar puedes revisar qué se añadirá, qué se reemplazará y qué se omitirá.

## Conjuros

Los conjuros pueden exportarse en un archivo JSON.

Durante la importación, DnDino distingue:

- conjuros nuevos
- conjuros con el mismo nombre ya presentes en la base de datos

Para cada conjuro puedes elegir si:

- importarlo como registro nuevo
- reemplazar un registro existente
- omitirlo

Cuando ya existe un conjuro con el mismo nombre, la pantalla de revisión muestra una comparación entre el registro actual y el importado. Así puedes comprobar nivel, escuela, manual, clases, tiempo de lanzamiento y duración antes de decidir.

También hay acciones masivas para gestionar conflictos, por ejemplo omitir todos los conjuros ya existentes o importarlos todos como nuevos.

## Personajes

Los personajes se exportan en un paquete ZIP que puede incluir:

- ficha del personaje
- imágenes vinculadas
- enlaces a conjuros
- datos necesarios para reconstruir el registro en otra instalación

Durante la importación, los personajes con el mismo nombre no se reemplazan automáticamente. Puedes importarlos como nuevos, reemplazar un registro existente u omitirlos.

Si el personaje importado tiene conjuros vinculados, DnDino intenta asociarlos a los conjuros ya presentes usando el nombre. Si encuentra varios conjuros compatibles, te pide cuál usar.

Cuando importes personajes en una base de datos ya rica, revisa siempre los enlaces a conjuros: dos conjuros pueden tener el mismo nombre pero venir de manuales o versiones diferentes.

## Aventuras

Las aventuras se exportan en un paquete ZIP con los datos necesarios para reconstruir la aventura.

Una aventura importada se crea siempre como **nueva aventura**. DnDino no sobrescribe una aventura existente, así evitas perder lugares, personajes o sesiones de una campaña activa.

El flujo recomendado es por pasos:

1. importar o vincular conjuros
2. importar o vincular personajes
3. importar la aventura

En la revisión de la aventura, DnDino separa las partes principales:

- conjuros incluidos en el paquete
- personajes incluidos en el paquete
- estructura de la aventura

Para conjuros y personajes puedes decidir cómo gestionar los registros ya presentes. Después, la aventura se importa vinculando los personajes correctos a lugares, presencias y otros contenidos del paquete.

## Equipo, dotes y glosario

El equipo, las dotes y las entradas del glosario también se pueden exportar e importar por separado.

La exportación crea archivos JSON dedicados, útiles para compartir solo una parte del material sin exportar una aventura completa.

Durante la importación, DnDino separa los registros nuevos de los que ya tienen una coincidencia en la base de datos. Para cada registro puedes importarlo como nuevo, reemplazar el existente u omitirlo.

Para el equipo, la coincidencia usa nombre y categoría, para mantener separados armas, armaduras, herramientas y equipo. Para las dotes también se tiene en cuenta el tipo de dote. Para el glosario, la referencia principal es el nombre de la entrada.

Cuando ya existe un registro similar, la pantalla de revisión compara el contenido actual con el importado. Usa las acciones masivas para omitir, importar o reemplazar varios registros a la vez cuando el archivo contiene muchos elementos.

## Comprobaciones antes de importar

Antes de importar paquetes con imágenes, DnDino comprueba que el archivo sea legible y que haya espacio suficiente para copiar los medios dentro del contenedor de la app.

Si el archivo está dañado, incompleto o no es compatible, la importación se interrumpe con un mensaje de error en lugar de crear datos parciales.

## Buenas prácticas

Antes de importar contenido importante:

- crea una copia de seguridad de la app
- importa primero los conjuros si muchos personajes los usarán
- revisa los registros con el mismo nombre antes de reemplazarlos
- usa la comparación entre antiguo y nuevo cuando tengas dudas
- importa las aventuras como nuevas y luego revisa enlaces, lugares e imágenes

La importación está pensada para proteger la base de datos: en caso de duda, elige `Importar como nuevo` u `Omitir` en lugar de reemplazar.
