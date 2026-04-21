# Heroes, NPCs, and Monsters

The **Heroes, NPCs, and Monsters** section contains all the base character records in the app. This is where you create, edit, and clone the records that can later be linked to adventures, places, and combats.

This page matters because DnDino uses **multiple character layers**, each with a different purpose:

- the **base sheet**
- the **adventure character**
- the **place occupant**
- the **combat participant**

These are not pointless duplicates. They exist so DnDino can keep **contextual data separate**, such as display name, hit points, conditions, initiative, and DM notes, while still preserving the link to the original source record.

## Base Sheet

The **base sheet** is the main record stored in `Heroes, NPCs, and Monsters`.

Here you define everything that belongs to the character in a general sense:

- name
- type: `Hero`, `NPC`, or `Monster`
- ancestry, class, size, alignment
- ability scores
- AC, maximum hit points, speed, initiative
- description, abilities, attacks
- linked images
- linked spells
- equipment and other reference data

The base sheet does not automatically mean the character is “present” in an adventure, a place, or a combat. It is the model from which the later layers are derived.

## Creating, Editing, and Cloning a Character

To create a new record:

1. open `Heroes, NPCs, and Monsters`
2. press the add button
3. fill in the character form
4. save the record

You can create:

- heroes
- NPCs
- monsters

The chosen type affects later fields and behaviors. For example:

- for **heroes**, it makes sense to talk about campaign presence, inspiration, and contextual state
- for **monsters**, CR, attacks, and repeated operational use become more important

When you open an existing sheet, you can edit the base record in full. Changes made here update the source record, but they do not always overwrite every contextual record already created in adventures, places, or combat. This is intentional.

**Cloning** creates a new base sheet from an existing one and copies linked elements such as:

- sheet fields
- linked spells
- structured attacks
- linked images

It is especially useful when you want to:

- create similar variants of the same monster
- start from a prepared NPC
- quickly build several records with the same structure

## Internal Links in Character Text

One of the most useful features of the base sheet, especially for **NPCs** and **Monsters**, is the system of **internal links** inside rich text fields.

This is especially valuable in **Attacks**, because it turns descriptive text into operational tools that are ready to use during play and in combat.

In practice, you can insert links that open:

- a dice roll
- an attack roll
- a full attack with damage
- a character
- a place
- a spell
- a feat
- a glossary rule

## Where They Are Most Useful

Internal links are especially valuable in rich text fields such as:

- `Attacks`
- `Special Abilities`
- `Description`
- other descriptive fields where you want fast references

The most useful case is still **Attacks**, because it lets you make the following directly clickable:

- the attack roll
- the damage dice
- a complete prepared attack

For monsters, this is extremely convenient because it cuts down the time spent reading formulas or rebuilding rolls by hand.

## How to Insert a Link

The correct flow is:

1. open a rich text field in the sheet
2. select the text you want to turn into a link, or place the cursor where you want to insert one
3. press the `Link` button
4. choose the type of link in the picker
5. confirm creation

Depending on the selected text, the picker may already suggest some ready-made automatic links.

## The Four Most Useful Roll Links

### Free Roll

`Free Roll` is the most flexible link. It is always available in the picker and is useful when you want a configurable roll without following a rigid structure.

It is useful for:

- a full formula like `1d6+3`
- a simple die like `1d20`
- a formula you may want to edit right before rolling

### Roll Dice

`Roll Dice` only appears if the selected text is a **valid dice formula**.

Valid examples:

- `1d6`
- `2d8+4`
- `4d4 + 1`

This link is ideal for single damage expressions, healing dice, random effects, and fast separate rolls.

### Attack Roll

`Attack Roll` only appears if the selected text is a **valid modifier**, not a full `1d20` formula.

Valid examples:

- `+5`
- `-1`
- `0`
- `2`

When you create this link, DnDino knows it should roll a **1d20** using that modifier. It is perfect for readable attack lines such as:

- `Bite +6`
- `Claws +4`

### Attack Roll and Damage

`Attack Roll and Damage` is the most powerful link for the **Attacks** section.

It is always available in the picker and opens a dedicated configurator where you can set:

- attack roll modifier
- critical threshold if needed
- up to three damage formulas
- labels for each damage component

It is the best way to build a full monster or NPC attack, because one link can contain:

- the attack roll
- primary damage
- secondary damage
- additional damage

In combat, this link is especially useful because the connected popover can also be used to apply damage to selected targets.

## Practical Attack Example

A very effective way to write a monster attack is to keep the text readable for the DM and make only the useful parts clickable.

For example:

- `Bite +6, reach 5 ft., one target. Hit: 1d8+4 piercing damage.`

You can then turn:

- `+6` into `Attack Roll`
- `1d8+4` into `Roll Dice`

or create a single `Attack Roll and Damage` link on the attack name or part of the line.

## Linking Places, Characters, and Other References

The link system is not only for dice.

In descriptive fields you can also create links to other app content, such as:

- a `Place`
- another `Character`
- a `Spell`
- a `Feat`
- a `Rule`

This is extremely useful when you want the text to become navigable.

When you press `Link`, the picker also tries to use the selected text as an initial filter:

- if it finds a real match in record names, it opens already filtered
- if it finds no real result, the initial filter is cleared and you see the full list

## Adventure Characters

The **adventure character** is the layer that links a base sheet to a specific campaign.

This record stores values that only make sense **inside an adventure**, such as:

- current hit points
- temporary hit points
- conditions
- state
- heroic inspiration

In other words:

- the base sheet says **who the character is**
- the adventure character says **how that character currently stands inside a given campaign**

## Place Occupants

The **place occupant** is another distinct record. It exists to say that a character or creature is present in a specific place, with a local name and possibly a local state.

In the `Add occupant to place` form there are two possible origins:

- `Adventure Character`
- `NPC / Monster`

### Occupant from Adventure Character

If you choose `Adventure Character`, the place record is linked to a character already present in the campaign.

In this case:

- the occupant remains linked to the adventure character
- it does not create a separate autonomous copy
- the same adventure character cannot be added twice to the same place

### Occupant from NPC / Monster

If you choose `NPC / Monster`, the place creates a **local cloned occupant** from a base sheet of type `NPC` or `Monster`.

This local record has its own place-specific data, such as:

- display name
- current HP
- temporary HP
- conditions
- state
- disposition
- DM notes

The behavior then depends on the type:

- **Monsters** can have multiple local instances in the same place
- **NPCs** remain unique within the same place and are not offered again in the picker there

When you add multiple instances of the same monster, DnDino automatically proposes an incremental name such as:

- `Goblin 2`

## Why Display Name Exists

Both place occupants and combat participants include a `Display Name` field.

This field exists to preserve a **contextual name** without renaming the base sheet. It is useful, for example, when you want to:

- distinguish similar copies of the same creature
- give an NPC a specific name in one place only
- use a different name in combat without changing the source record

## Combat Participants

The **combat participant** is the operational layer used during a fight.

A participant can come from three different sources:

- an **adventure character**
- a **place occupant**
- a **base sheet**

Each combat participant has its own combat-specific record, with data such as:

- display name
- initiative
- AC
- max HP
- current HP
- temp HP
- conditions
- state
- death saves
- round order

### Participants from Adventure Characters

If the participant comes from an adventure character:

- it stays linked to that campaign character
- at the end of combat, final values are synchronized back onto the adventure record

### Participants from Place Occupants

If the participant comes from a place occupant:

- it stays linked to that place record
- if the occupant uses local state, combat can synchronize HP, conditions, and state back to the place record

### Participants from Base Sheets

If the participant comes directly from a base sheet:

- the combat record uses that sheet as its source
- the behavior regarding multiple instances depends on type

In the combat picker:

- a base record of type **Monster** can be added more than once
- a base record of type **NPC** or **Hero** is not offered more than once in the same combat

## Synchronization Between Layers

Some values are synchronized across layers, but not everything is always overwritten.

### From Base Sheet to Contexts

The base sheet provides:

- the identity of the character
- reference statistics
- spells
- attacks
- images

### From Contexts Back to Linked Records

Operational layers may instead synchronize situational data, especially:

- HP
- conditions
- state
- some local notes

In combat, for example, final values may be pushed back to:

- the linked adventure character
- the linked place occupant, if that occupant uses local state

## Practical Difference Between the Layers

An easy way to remember the logic is:

- `Base Sheet`: the **general model** of the character
- `Adventure Character`: the **state of that character inside the campaign**
- `Place Occupant`: the **contextual presence of that character in a specific place**
- `Combat Participant`: the **operational version of that character inside the fight**

## When to Use Each Layer

### Use the base sheet when:

- you need to create the character
- you want to edit structural data
- you need to link images, spells, or attacks

### Use the adventure character when:

- you want to link a hero to the campaign
- you need persistent HP, state, conditions, and inspiration inside the adventure

### Use the place occupant when:

- you want to populate a place with characters or creatures
- you want contextual names for NPCs and monsters
- you want separate local instances inside a place

### Use the combat participant when:

- you are preparing or running a fight
- you need initiative, HP, and battle conditions
- you want combat to work on contextual records without directly dirtying the base sheet

## In Summary

The `Heroes, NPCs, and Monsters` section is not just an archive of sheets. It is the **source layer** from which all contextual character management inside the app is built.

The overall logic is:

- the **base sheet** defines the character
- the **adventure character** places that character inside a campaign
- the **place occupant** contextualizes that character in a place
- the **combat participant** makes that character operational in a fight

!!! tip
    If you want to avoid confusion, always remember this distinction: the base sheet describes the character, while adventure, place, and combat describe that character's state in a specific context. You don't need to focus too much on the abstract separation itself; what matters is that some fields only exist in their own context.
