# Reusable Libraries

DnDino Hero separates character data from reusable content.

This avoids entering the same information repeatedly and keeps multiple characters consistent.

## Classes

Classes are shared content.

A class can contain:

- name
- description
- hit die
- primary abilities
- saving throw proficiencies
- skill proficiencies
- weapon, armor, and tool proficiencies
- starting equipment
- class features
- progressions
- subclasses
- spells
- custom free lists

When you edit a class, associated characters read the updated definition.

## Subclasses

Subclasses belong to a class.

Each subclass can have:

- name
- subclass features
- free lists
- spells, when available
- spellcasting ability, if the subclass uses magic

On the character, the subclass is selected per class when that class reaches the required level.

## Progressions

Progressions represent values that change by level.

They can be used for:

- consumable resources
- bonuses
- numeric values
- dice
- descriptive values

Resource progressions can show remaining and total uses, with buttons to consume or restore them.

!!! note
    Bonuses declared in progressions are not applied automatically to ability scores, attacks, or other statistics. Add them manually where they should matter.

Die or bonus progressions can also be referenced by attacks to build additional damage or class-based modifiers.

## Feature Bonuses

Class features and some custom lists can show a bonus built from multiple parts.

A bonus can include:

- die roll
- class level
- proficiency bonus
- ability modifier
- free value
- die or bonus class progression

You can also give the total bonus a name, useful when you want to show a compact formula such as `1d10 + 5`.

## Species

Species are reusable and can include:

- species name
- creature type
- size
- height range
- base speed
- description
- species traits

Traits can depend on level. In the main sheet, only traits available at the current level are shown.

## Backgrounds

Backgrounds can include:

- name
- selectable ability scores
- feat
- skill proficiencies
- tool proficiencies
- equipment
- description

The background name is shared with the character identity.

## Feats, Rules, and Spells

DnDino Hero includes general libraries for:

- feats
- rules
- spells

These elements can be imported, exported, and associated with the character when needed.

Spells can be associated with a character, marked as prepared or not prepared, and shown in the sheet only when actually available.

## Import and Export

The main libraries can be exported and imported as JSON, so you can move content between devices or recover it from DnDino.

When a name already exists, import should ask how to proceed to avoid accidental overwrites.

Import and export are available for:

- classes
- species
- backgrounds
- spells
- feats
- rules
