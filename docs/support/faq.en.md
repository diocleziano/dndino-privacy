# FAQ

This section collects quick answers to the most common questions about DnDino.

If you need a full explanation of a specific screen, it is best to open the dedicated guide page afterwards. The FAQ is mainly meant for the most common practical cases.

## How do I jump back into my latest campaign?

Open `Home` and use the **latest adventure** card.

From there you can:

- open the adventure dashboard directly
- jump to the last visited place, if available

It is the fastest way to resume your work without going through the full adventure list every time.

## What is the difference between a base sheet, an adventure character, a place presence, and a combat participant?

The **base sheet** is the general record for a character or creature.

From that sheet, DnDino can create separate contextual records:

- the **adventure character**, used inside a campaign
- the **place presence**, used in places
- the **combat participant**, used in combat

This system keeps separate:

- contextual names
- initiative
- current HP
- DM notes
- local combat or place state

In other words, the base sheet remains the general reference, while contextual records let you work in a practical way during play.

## How do I add a hero to an adventure?

Open the `Adventure Dashboard`, then go to the `Characters` panel.

From there you can:

- add an existing character
- create a new character with `Create character`

If you create a new character from the picker, saving returns you to the selection panel and refreshes the list immediately.

## How do I add a presence to a place?

Open the place and go to the `Presences` panel.

From there you can add:

- a hero already linked to the adventure
- an `NPC`
- a `Monster`

Keep this important distinction in mind:

- an `NPC` remains unique within that place
- a `Monster` can be added more than once

This lets you place multiple instances of the same monster in one place, while avoiding accidental duplication of NPCs.

## Can I rename a monster without changing its base sheet?

Yes.

That is one of the main reasons why DnDino uses contextual records.

You can rename a monster:

- during pre-combat
- in place presences
- in other local contexts where the operational name needs to be easier to read

This does not change the name on the original base sheet.

## How do I quickly link a character or a place inside a description?

In text fields that support internal links, use the `Link` command.

From there you can create links to:

- characters
- places
- spells
- rules
- feats

This is especially useful:

- in `Places`, to link other places or characters mentioned in the description
- in `Characters`, especially in `Attacks`, to link rolls or useful references

## What are links in monster Attacks for?

They turn descriptive text into an operational tool.

Inside rich text attack fields you can add links such as:

- `Full Attack`
- `Free Roll`
- `Roll Dice`
- `Attack Roll`

This lets you:

- roll dice quickly
- apply damage to targets
- link to other app entries

It is one of the most effective ways to make a monster sheet truly useful during combat.

## Am I forced to use automated combat rolls?

No.

DnDino offers a lot of automation, but it does not force you to use it.

You can still:

- roll physical dice at the table
- read results in a traditional way
- apply damage manually

The app mainly helps remove repetitive HP updates and mental math.

## Does combat still work well on a single monitor?

Yes.

`Flat Combat` works well even on a single screen.

Using a second display with the `Players Window` is great for presentation, but it is not required. On one monitor you can still run combat comfortably and decide from the settings how the players window should behave.

## Can I choose how much information players see during combat?

Yes.

In `Settings > Combat`, among other things, you can decide whether players see:

- round number
- HP
- conditions
- next turn
- enemies' real names
- NPC and monster details

This lets you decide whether you want a more transparent combat flow or a more classic DM-screen style.

## How does the final combat summary work?

At the end of combat, DnDino closes the encounter and syncs contextual data back to linked records.

In addition:

- the DM sees the final summary inside combat
- players can see a summary in the `Players Window`, if the option is enabled

The public summary is focused on the player characters, not the enemies.

## What happens if a hero drops below 0 HP?

Heroes can go into negative HP.

The rule handled by the app is:

- between `0` and `-(max HP - 1)`, the hero is `Unconscious`
- at `-max HP` or lower, the hero dies outright

During combat, when a hero is unconscious, DnDino also shows the **death saving throws** panel.

## How do I show an image to the players?

DnDino uses a dedicated window for player-facing presentation.

You can use it:

- during combat
- for adventure images
- in other flows that support presentation

The window behavior is configured in `Settings > Media` and, in part, in `Settings > Combat`.

## How do I back up my data?

Go to `Settings > Database`.

From there you can:

- see where the app data is stored
- open the data folder
- open the backup folder
- create a snapshot manually
- restore a snapshot
- restore from iCloud, if configured

In the same section you can also decide:

- automatic backup frequency
- maximum number of snapshots to keep

## Where can I find technical database information if something looks wrong?

Go to `Settings > Diagnostics`.

There you can check:

- database path
- whether the file exists
- size
- last modified date
- SQLite version
- detected tables and record counts

This is the right place to check when you want to understand whether a problem is only visual or really affects saved data.

## How do I contact support?

Open `Settings > Support`.

From there you can:

- send a support request
- send a suggestion
- copy the contact email

Use `Support` when something is broken or unclear. Use `Suggestion` when you want to propose an improvement or a new feature.

!!! tip
    If an answer here feels too short, use the FAQ as a starting point and then open the dedicated guide page, such as `Characters`, `Places`, `Combat`, or `Settings`.
