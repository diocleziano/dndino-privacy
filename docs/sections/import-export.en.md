# Import and Export

DnDino lets you export and import content to move it between installations, create working copies, or share material with other Dungeon Masters.

Imports never overwrite existing data automatically: before saving, you can review what will be added, replaced, or skipped.

## Spells

Spells can be exported as a JSON file.

During import, DnDino separates:

- new spells
- spells with the same name already in the database

For each spell, you can choose whether to:

- import it as a new record
- replace an existing record
- skip it

When a spell with the same name already exists, the review screen shows a comparison between the current record and the imported one. This lets you check level, school, sourcebook, classes, casting time, and duration before deciding.

Bulk actions are also available for conflicts, for example skipping all existing spells or importing them all as new records.

## Characters

Characters are exported as a ZIP package that can include:

- character sheet
- linked images
- spell links
- data needed to rebuild the record in another installation

During import, characters with the same name are not replaced automatically. You can import them as new records, replace an existing record, or skip them.

If the imported character has linked spells, DnDino tries to match them to existing spells by name. If multiple matching spells are found, you can choose which one to use.

When importing characters into an existing database, always review spell links: two spells can share the same name but come from different sourcebooks or versions.

## Adventures

Adventures are exported as a ZIP package with the data needed to rebuild the adventure.

An imported adventure is always created as a **new adventure**. DnDino does not overwrite an existing adventure, so you do not risk losing places, characters, or sessions from an active campaign.

The recommended flow is step by step:

1. import or link spells
2. import or link characters
3. import the adventure

In the adventure review, DnDino separates the main parts:

- spells included in the package
- characters included in the package
- adventure structure

For spells and characters, you choose how to handle records that already exist. After that, the adventure is imported by linking the correct characters to places, presences, and the other package contents.

## Equipment, Feats, and Glossary

Equipment, feats, and glossary entries can also be exported and imported separately.

Export creates dedicated JSON files, useful when you want to share only part of your material without exporting an entire adventure.

During import, DnDino separates new records from records that already have a match in the database. For each record, you can import it as new, replace the existing one, or skip it.

For equipment, matching uses both name and category, so weapons, armor, tools, and gear stay distinct. For feats, the feat type is also considered. For the glossary, the main reference is the entry name.

When a similar record already exists, the review screen compares the current content with the imported one. Use bulk actions to skip, import, or replace multiple records at once when the file contains many items.

## Checks Before Importing

Before importing packages with images, DnDino checks that the file is readable and that there is enough free space to copy media into the app container.

If the file is damaged, incomplete, or incompatible, the import stops with an error message instead of creating partial data.

## Best Practices

Before importing important content:

- create an app backup
- import spells first if many characters will use them
- review records with the same name before replacing them
- use the old/new comparison when unsure
- import adventures as new, then verify links, places, and images

Import is designed to protect your database: when in doubt, choose `Import as new` or `Skip` instead of replacing.
