# Glossary

This glossary gathers the most important terms used across the app and the guide.

The goal is not to provide dictionary-style definitions, but to clarify **how DnDino actually uses these terms** in its main workflows.

## A

### Adventure

The main campaign or scenario inside which DnDino organizes:

- places
- quests
- adventure characters
- sessions
- maps
- images
- combats

It is the most important narrative and operational container in the app.

### Attack Roll

A type of internal link focused on an offensive roll with a modifier.

### DM Image

An image opened for the DM, separate from the one shown to players.

The `Media` settings control on which monitor it opens and whether position and size should be remembered.

### DM Notes

Private contextual notes for the DM.

In some parts of the app they are always available through a dedicated button and are saved when the popover closes.

### DM Notes Field

Private notes visible only to the DM. They can appear in different contexts of the app, for example on:

- combat participants
- place presences
- other records that support operational notes

They are meant to store working information without showing it to the players.

## C

### Campaign Dashboard

The main screen of a campaign.

From here you can quickly reach the most important panels, such as:

- places and quests
- characters
- sessions
- images
- maps
- concept maps

### Character Sheet

The main record of a character or creature in the `Heroes, NPCs, and Monsters` section.

It does not automatically represent that character in every context: different contextual records can be created from it.

### Combat

The contextual encounter created inside an adventure or a place.

A combat contains:

- participants
- initiative
- rounds
- temporary encounter state
- logic for damage, healing, conditions, and the final summary

### Combat Participant

The record used in combat to represent who takes part in the encounter.

A participant is a contextual layer separate from the base sheet and can have:

- local name
- initiative
- current HP
- conditions
- DM notes
- combat state

### Compact View

A reduced layout or window aimed at quick consultation, used in some app flows instead of the full editor.

### Condition

A temporary state applied to a character or creature, such as a penalty or combat effect.

Conditions can be shown:

- in combat
- in the players window
- in some summaries

### Concept Map

A logical, relational map used to organize ideas, links, factions, places, characters, and subplots.

It is different from an interactive map:

- a concept map organizes relationships and narrative structure
- an interactive map supports spatial navigation

### Contextual Data

Information that does not belong absolutely to the base sheet, but to a specific context instead.

For example:

- a monster's name in a specific combat
- local HP on a presence
- the DM notes of a participant

### Contextual Record

Any record that exists in relation to a specific context rather than as the main sheet.

The most important cases are:

- adventure character
- place presence
- combat participant

### Cover Image

The main image associated with a record, such as an adventure, a character, or a place.

It is mainly used to improve visual recognition in dashboards and main cards.

## D

### Diagnostics

The settings section that shows technical database information, such as:

- file path
- whether the database exists
- size
- tables and record counts

It is useful when you want to understand whether a problem really affects saved data.

## E

### Full Attack

A type of **internal link** used mainly in `Attacks` fields for monsters and NPCs.

It can combine into one link:

- attack roll
- roll mode
- critical threshold
- up to three damage components

During combat it can also be used to apply damage to selected targets.

### Full Editor

An extended window or form used to edit a record in detail instead of relying only on popovers or quick panels.

## F

### Flat Combat

The standard combat mode in DnDino.

It uses a three-area structure:

- participant list on the left
- central panel for the current turn or summaries
- right area or contextual panels depending on the screen

It is the reference combat system described in the guide.

### Form

A screen used to create or edit a record, such as a character, a place, or a spell.

### Free Roll

A very flexible internal link type for dice.

It can be used for formulas such as:

- a single die
- a roll with a modifier
- a freely constructed roll

## G

### Glossary

In the guide, this is the page that explains the meaning of terms used throughout the app.

Inside the app, the term can also refer to rule entries or quick-reference content available from the `Rules` section.

## H

### Hero

The player-facing character type or main protagonist type of the campaign.

In DnDino, `Hero` is distinct from:

- `NPC`
- `Monster`

Heroes follow specific rules, especially in the adventure dashboard and in combat.

## I

### Initiative

The value that determines turn order in combat.

It can be:

- entered manually
- rolled automatically for NPCs and monsters

### Inspector

A detail panel used in screens such as concept maps to edit the properties of the selected element.

### Interactive Map

An image-based map enriched with navigable markers.

It is used to move through places visually by opening and linking areas of the campaign.

### Interactive View

The mode of the places dashboard in which the left area shows the interactive map instead of the places tree.

### Internal Link

A link created inside a rich text field that points to app content or a quick action.

It can link, for example, to:

- characters
- places
- rules
- feats
- spells
- dice rolls

### Interactive Marker

A clickable point on an interactive map that represents a link to a place.

Markers can be created, moved, edited, and removed.

### In Visit

The state of a place during a live session.

It marks the place currently being visited or explored.

### Item Metadata

Technical or structural information shown in dedicated panels when the relevant option is enabled in settings.

## L

### Live

In the guide, when it appears on its own, it usually refers to behavior related to the **Live Session** or real-time flows, not to a simple static screen.

### Live Session

The operational context of the ongoing game session.

It is not just a window: it ties together the timer, the active campaign, visited places, quests, and several linked flows.

### Location / Place

A narrative or geographical space in the adventure, such as:

- a city
- a room
- a dungeon area
- a building
- an explorable zone

A place can have:

- descriptions
- images
- maps
- presences
- combats
- hierarchical links to other places

## M

### Map

An image linked to a place or to the adventure, used as visual support.

Not every map is automatically interactive.

### Monster

This glossary page does not define `Monster` separately because in DnDino it mainly matters as a base type distinct from `Hero` and `NPC`, especially in places and combat where duplication rules differ by context.

## N

### Enemy

A contextual role assigned to a participant or a presence.

It does not necessarily match the type of the base sheet: it is a classification used in the context of a place or a combat.

### NPC

`Non-player character`.

In DnDino it is a type distinct from both `Hero` and `Monster`.

In the context of places:

- a base NPC can only be added once to the same place

In the context of combat:

- it is not meant to be duplicated in series like monsters are

## P

### Panel

A visual block or section within a larger screen, for example in the adventure dashboard or in combat.

### Place Dashboard

The operational screen of the `Places` section.

It can be used:

- in standard mode, with the places tree on the left
- in interactive mode, with the interactive map instead of the tree

### Place Presence

A record showing that a character or creature is present in a specific place.

A presence is different from both the base sheet and the combat participant.

It can have:

- contextual name
- place role
- local state
- DM notes

### Popover

A small contextual panel that opens above or near an interface element.

DnDino uses many popovers for:

- dice rolls
- DM notes
- quick descriptions
- contextual details

### Players Window

The dedicated window for content shown to the players on a separate screen or, if you prefer, on the same monitor.

It can show:

- images
- the current combat turn
- combat intro
- the final encounter summary

### Quest

A narrative element or objective managed in the `Places and Quests` section.

Quests coexist with places but have their own dedicated behavior, state, and content.

## R

### Rich Text

A formatted text field that supports:

- text styles
- internal links
- content richer than plain text

It is widely used for descriptions, attacks, and notes.

### Round

The full cycle of turns in combat.

When every participant has completed their turn, the round advances.

## S

### Snapshot

A backup copy of the app's data.

Snapshots can be:

- automatic
- manual
- local
- cloud-based, depending on settings

### State

The general condition of a record in its context.

It can refer, for example, to:

- the state of a place
- the state of a quest
- the state of an adventure character
- the state of a participant

### Sub-place

A child place linked hierarchically to another place.

It is used to build structures such as:

- city and districts
- building and rooms
- area and sub-area

## T

### Top Bar

The upper bar of the app.

It contains quick tools and, depending on settings, may include extra controls such as those for the `Players Window`.

### Turn / Current Turn

The participant currently active in combat.

In `Flat Combat`, it is the focal point of the central panel.

### Saving Throw

A roll based on an ability, often used in combat through the `ST` button.

For unconscious heroes it can also include the death saving throw flow.

## U

### Unconscious

A special hero state in combat when HP drop below zero, but not far enough to cause instant death.

In this range the character:

- is not considered definitively dead
- may need death saving throws

!!! tip
    If you encounter an unclear term while reading the guide, come back here and then reopen the matching section page. The glossary is designed as a bridge between the names used in the interface and the app's real workflows.
