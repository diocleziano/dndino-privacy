# Combat

DnDino’s **Combat** mode is designed to be the main operational tracker for an encounter. This page describes the standard combat mode used in DnDino.

Combat always begins in the context of a **place** and carries with it the linked characters, local occupants, and any monsters or NPCs tied to that scene.

This page explains the full flow:

- pre-combat setup
- participant management
- starting the encounter
- using the current turn panel
- applying damage, healing, conditions, and saving throws
- integration with the **Players Window**
- ending the encounter and reviewing the final summary

## Using One or Two Screens

DnDino combat works well even on a **single screen**: the full operational side remains in the main panel, and you can manage participants, turns, damage, conditions, and the final summary without needing a second monitor.

That said, if you do have a dual-screen setup, you can use:

- one main screen for the DM control panel
- a second screen or monitor for the **Players Window**

In that setup the flow becomes even smoother:

- on the DM screen you keep the participant list, round controls, current turn, attack text, DM notes, and quick edits visible
- on the players’ screen you show a clean presentation of the active participant, with image and contextual overlay

In practice:

- on a single screen, you run the whole encounter from the main combat screen
- with two screens, you separate the DM’s technical tracker from the player-facing presentation

!!! tip
    A second screen is not required. It is simply a very useful upgrade when you want to show images and turn information to the players without exposing the DM’s technical panel.

## How the Players Window Works During Combat

When combat starts, DnDino can automatically open or update the **Players Window**.

If player presentation is active:

- at the start of combat it may show a short **intro** with the participants
- during combat it updates to the **current turn participant**
- at the end of the encounter it may show a **final summary**

During combat, the Players Window does not show the DM’s technical panel. Instead, it shows a visual presentation with:

- the image of the active participant
- the name shown to players
- overlay information, if enabled

The overlay can include:

- current round
- current, maximum, and temporary HP
- conditions
- next turn

Enemy information can be handled separately from hero information.

## Players Window and Second-Screen Settings

The most important options live in **Settings**, in the area dedicated to combat presentation and the players window.

### Opening and General Behavior

The main settings are:

- `Open players window even with one monitor`
- `Show players window controls in the top bar`
- `Show combat intro to players`
- `Show final summary to players`

#### Open players window even with one monitor

If this option is enabled, DnDino can automatically open the Players Window even when you are working on a single monitor.

If it is disabled:

- on a single monitor the window does not open automatically
- if it is already open, it will still continue updating

#### Show players window controls in the top bar

If enabled, the top bar shows buttons to:

- open the Players Window manually
- close it manually

#### Show combat intro to players

When you press `Start encounter`, the Players Window can show a short introduction with:

- encounter title
- involved participants
- participant count

If you disable this option, combat jumps straight to the first active participant.

#### Show final summary to players

When combat ends, the Players Window can show a final summary.

The player-facing summary only shows information useful to players, such as:

- damage dealt by heroes
- damage taken by heroes
- the image of the most dangerous enemy

The final player summary stays visible until you change the content in the window or close it.

### Information Shown During a Turn

The settings that control the active participant overlay are:

- `Show round in players window`
- `Show HP in players window`
- `Show conditions in players window`
- `Show next turn in players window`

### Information About Enemies, Monsters, and NPCs

For non-hero participants there are dedicated controls:

- `Show NPC and monster details to players`
- `Show enemy conditions to players`
- `Show enemy names to players`

This lets you decide whether the Players Window should:

- show the creature in a more atmospheric way
- or display more technical information as well

## Where Combat Opens

Combat is created from the context of a **place**. Once opened, DnDino shows a layout with two main columns:

- on the left, the operational combat tracker
- in the center, the main scene panel or the current turn panel

Before combat has started, the center panel shows the **Pre-Combat Summary**.

Once the encounter is active, that same panel becomes the **Current Turn** area.

When combat has ended, the center panel shows the **Final Encounter Summary** for the DM.

## General Screen Structure

### Left Column

The left column contains:

- `Combat controls`
- the participant list header
- the ordered list of participants

The list is framed by two decorative and functional rows:

- `Round Start`
- `Round End`

### Center Panel

The center panel changes depending on combat state:

- **before combat starts**, it shows the pre-combat summary
- **during combat**, it shows the current-turn participant
- **after combat**, it shows the DM final summary

## Pre-Combat

Pre-combat is where you prepare the encounter before starting the first turn.

This is the stage where it is most useful to adjust three things:

- monster names, when you want to distinguish them more clearly at the table
- hero initiative values, by entering them manually
- NPC and monster initiative, by rolling automatically or typing it manually

## Pre-Combat Summary

The opening card shows a quick overview with metrics such as:

- participants
- heroes
- allies
- enemies
- total enemy HP
- participants already in critical condition

## Character Initiative

The `Character Initiative` section gathers the main heroes and lets you quickly edit initiative before sorting the encounter.

Each row includes:

- participant name
- contextual subtitle
- initiative field
- `Delete` button

## NPCs and Monsters

The `NPCs and Monsters` section is dedicated to non-hero participants.

Here you can:

- edit initiative quickly
- rename monsters and NPCs on the fly to distinguish them more clearly
- use `Init NPCs/Monsters` to roll initiative automatically
- enter initiative manually if you prefer using a roll made outside the app
- remove a participant quickly with `Delete`

## Main Pre-Combat Actions

The main actions in the pre-combat summary are:

- `Add`
- `Sort`
- `Start encounter`

If at least one participant still has initiative `0`, DnDino asks for confirmation before starting.

## Where Participants Can Come From

The add-participant panel can pull from three sources:

- `Heroes`
- `Place Occupants`
- `Global`

### Heroes

These are the adventure characters already linked to the campaign. Each hero can enter combat only once.

### Place Occupants

These are characters already present in the place from which combat begins. Their local state can be reused as the basis for the encounter.

### Global

These are base sheets not already linked as campaign heroes.

For global entries:

- `Monsters` can be added multiple times
- global `Heroes` and `NPCs` cannot be duplicated as pure global sheets

## Combat Controls

Once the encounter has started, the `Combat controls` panel stays fixed above the participant list and contains the main round actions.

The button rows are:

1. `Add` and `Sort`
2. `Start/Pause` or `Resume` and `End`
3. `Prev.` and `Next`

If there is a reversible last attack, an extra panel also appears:

- `Undo last attack`

## Participant List

The list on the left is the heart of tactical tracking.

Each collapsed row shows:

- turn position, for example `1/8`
- participant name
- up to three condition icons
- `Turn` badge if it is the active participant
- AC
- HP
- temporary HP
- initiative

The active participant is highlighted much more strongly than the others:

- colored side band
- stronger border
- warmer background
- automatic scroll to keep it visible

The row also uses impact effects when the participant:

- takes damage
- is killed
- is restored by an undo

## Context Menu on a Row

By **right-clicking** a participant card you can open the context menu.

Currently the available action is:

- `Delete`

## Expanding a Participant Row

Clicking a row expands it and reveals its quick controls.

In the expanded area you will find:

- editable name
- quick numeric fields:
  - initiative
  - HP
  - temporary HP
  - AC
- action buttons
- conditions block
- access to abilities, specials, and spells, when present

## Quick Row Buttons

The quick actions can include:

- `Attack`
- `Damage`
- `Heal`
- `Save`
- `DM Notes`
- `Edit`
- `Conditions`

Some buttons only appear when they make sense for that participant.

## Attack

`Attack` opens a popover where you can select:

- one or more targets
- the damage to apply

The target selector uses a compact list with:

- name
- AC
- HP
- conditions

Target ordering is not random. DnDino tries to suggest the most relevant participants first depending on who is attacking.

In general:

- if a **Hero** attacks, **enemies** come first, then allies, then neutrals, and finally lower-priority monsters
- if a non-hero attacks, **heroes** come first, then allies, then neutrals, and finally less relevant enemies

Inside each group, names are then sorted alphabetically.

The popover never pre-selects a target automatically: target selection must be manual.

When you apply one attack to multiple targets:

- damage is applied to all selected targets
- the top banner shows multiple rows, one for each hit target
- the last-attack undo keeps the whole group together

## Damage and Heal

`Damage` applies direct damage to the participant.

`Heal` applies direct healing.

## Save

`Save` opens the **Saving Throw** popover based on the participant’s stats.

## Conditions

The `Conditions` button opens the dedicated popover for active states.

From here you can:

- add conditions
- set duration and expiration rules
- link the end of a condition to another participant’s turn

## DM Notes

The `DM Notes` button is always visible.

It opens an editable popover where you can write contextual notes about the participant. The content is saved when the popover closes.

## Edit

`Edit` opens the participant editor panel.

This is useful when you need to make deeper changes to:

- initiative
- AC
- maximum, current, and temporary HP
- combat role
- linked contextual data

## Current Turn

When combat is active, the center panel focuses completely on the participant whose turn it is.

The top card shows:

- participant image
- name
- subtitle
- AC
- HP
- temporary HP
- initiative
- speed
- inspiration, if the participant is an adventure hero
- active conditions
- main stats

## Center Panels During the Turn

Below the turn summary, only panels with real content are shown.

Possible sections are:

- `Attacks`
- `Special Abilities`
- `Abilities`
- `Description`
- `Spells`

All of them are collapsible.

They also use light visual accents:

- `Attacks` red
- `Abilities` yellow
- `Special Abilities` green
- `Spells` light blue
- `Description` gray

## Attacks and Internal Links

The `Attacks` section is one of the strongest parts of flat combat.

If you prepared internal links inside the base sheet attack text, you can use them directly during combat.

In particular, the **Full Attack** link is extremely useful because it:

- rolls attack and damage inside the same popover
- lets you select one or more targets
- automatically suggests `Damage to apply`
- lets you exclude individual damage rows if you rolled multiple components and only want to apply some of them
- closes the popover as soon as damage is applied

This makes monster attacks much faster to run at the table.

## Characters at 0 HP or Lower

In combat, **Heroes** follow a different rule from NPCs and monsters.

### Heroes

Heroes can go below `0` HP.

The rule is:

- between `0` and `-(max HP - 1)`, the character is **Unconscious**
- at `-max HP` or lower, the character dies permanently

When a hero is at `0` HP or lower but not permanently dead:

- they remain in the encounter
- the center panel shows the `Death Saving Throws` card

This card tracks:

- successes
- failures

and lets you quickly register:

- `Success`
- `Failure`

At 3 successes, the character returns to `1` HP. At 3 failures, they die.

### NPCs and Monsters

For non-heroes, behavior is simpler:

- at `0` HP or lower, they are dead

## Turns, Rounds, and Participants Excluded from the Cycle

Inside the turn cycle:

- permanently dead heroes are excluded
- NPCs and monsters at `0` HP or lower are excluded

This means an **Unconscious** hero can still receive a turn, precisely because death saves still need to be handled.

## Impact Banners and Visual Feedback

When an attack hits, DnDino shows a large banner at the top with an immediate recap.

For example:

- who hit
- who was hit
- how much damage was applied
- whether the blow killed the target

If there are multiple targets, the banner shows multiple lines in the same box.

The **Players Window** can also show the hit animation, including all targets involved in the same multi-target attack.

## Undo Last Attack

When you apply an attack, the panel

- `Undo last attack`

appears.

Below the button you see a short summary of what just happened.

If the last attack hit multiple targets, the panel shows the full list of rows that will be restored.

When you confirm the undo:

- targets return to their previous state
- a restore notification appears
- card visual feedback updates as well

## Final Encounter Summary

When combat ends, the center panel switches to the **Final Encounter Summary** for the DM.

This screen shows:

- total rounds
- duration
- enemies killed
- damage dealt
- damage taken

## What Gets Synchronized at the End

When you close combat, DnDino saves the outcome back to the linked records.

For adventure heroes it synchronizes:

- current HP
- temporary HP
- manual conditions
- final state

For place occupants with local state it synchronizes:

- current HP
- temporary HP
- manual conditions
- final state

Combat also updates the linked **live session** data, including:

- damage dealt
- damage taken
- fallen heroes

## When Combat Shines the Most

DnDino combat shines most when you use it like this:

1. you prepare pre-combat carefully
2. you use a second screen with the **Players Window**
3. you rely on attack links for monsters and NPCs
4. you keep the DM on the tracker and the players on the presentation

!!! tip
    Even though combat offers many automations for rolls, full attacks, and fast damage application, DnDino still leaves room for a more traditional way of using dice. You can keep rolling physically or handle the roll outside the app and use combat mainly to apply values quickly and consistently, avoiding the most tedious part: recalculating HP changes by hand every time.
