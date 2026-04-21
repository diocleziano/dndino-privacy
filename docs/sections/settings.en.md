# Settings

The **Settings** section gathers DnDino’s global preferences. You are not working on a single adventure or a single character here. Instead, this is where you define **how the app should behave as a whole**.

Settings mostly affect:

- the overall look of the interface
- top bar behavior
- the `Places` workflow
- the behavior of `Combat`
- image, backup, and snapshot management
- database support and diagnostics

## How the Screen Is Organized

The page is divided into two areas:

- a **left sidebar** with categories
- a **main panel** on the right with the options for the selected section

Available categories are:

- `General`
- `Top Bar`
- `Places`
- `Combat`
- `Media`
- `Theme`
- `Database`
- `Diagnostics`
- `Support`
- `Licenses`

This structure separates daily-use preferences from more technical areas such as backups and diagnostics.

## General

The `General` section gathers the base preferences of the app.

### DM Profile

Here you can customize your profile with:

- `User name`
- `Gender`

The name is reused in other parts of the app, such as the welcome message on the `Home` screen.

### Interface Language

You can choose whether to:

- follow the system language
- force a specific app language

### Global Confirmations

The `Ask for confirmation before deletions` option adds a confirmation step before destructive actions such as removals and deletions.

### Metadata

Inside `General` you also find:

- `Show metadata in app`

This controls whether metadata panels should be shown in the screens that support them.

### Adventure Dashboard Panel Layout

This part is important if you use the `Adventure Dashboard` often.

You can:

- drag panels
- reorder them inside the left or right column
- move them from one column to the other

### Active Theme

Inside `General`, the **currently selected theme** is also shown as a quick summary. The actual theme change is made in the `Theme` section.

### Introductory Guides

From here you can restore the app’s first-use behavior.

The `Reset First Use` button tells DnDino to consider contextual guides and onboarding flows as unseen again.

## Top Bar

The `Top Bar` section defines how the quick tools in the top bar behave.

### Top Bar Look

You can choose whether the top bar is displayed:

- with icons only
- or with icons and labels underneath

### Default Die

DnDino includes a quick dice roller in the top bar. Here you can choose the **default die type** shown when you open it.

### Quick Character Opening

This setting controls how quick opening of characters from the top bar behaves.

You can decide whether the shortcut should lead to:

- a more read-oriented view
- or a mode closer to editing

### Quick Rules Opening

The top bar also allows fast opening of `Rules`.

Here you can decide whether that shortcut should open:

- the full editor
- or a smaller consultation-oriented window

### Players Window Controls in the Top Bar

The `Show players window controls in the top bar` option adds controls in the top bar to manually open or close the `Players Window`.

## Places

The `Places` section contains global preferences used as default behavior in the places dashboard.

### Default Occupant Role

When you add an occupant to a place, DnDino can propose a default starting role.

### Show Parent Place Maps by Default

If enabled, inherited maps from parent places start visible in the `Places` screen.

### Remember Last Visited Place

If enabled, when you come back to the `Places` screen the app tries to restore the last selected place for that adventure.

### Automatically Close the Previous Place

This setting applies during an **active live session**.

When a place is marked as `Being visited`, the place that was previously `Being visited` is automatically marked as `Visited`.

## Combat

The `Combat` section gathers the global preferences of the combat system.

Here you find both presentation options and settings that influence the practical flow of encounters and the `Players Window`.

## Center Panel Order

You can reorder the center combat panels by dragging elements such as:

- `Attacks`
- `Special Abilities`
- `Abilities`
- `Spells`
- `Description`

## Combat Presentation

This subsection controls the overall behavior of combat and player presentation.

### Show Turn to Players by Default

If enabled, new combats start with automatic turn presentation already active.

### Open the Players Window Even with One Monitor

This setting controls the automatic behavior of the `Players Window` in single-screen setups.

### Automatically Show the Current Turn Participant Detail

When the turn changes, the app can:

- automatically select the active participant
- also open their detail

### Automatically Sort by Initiative When Starting

When you press `Start combat`, DnDino can automatically reorder participants by initiative before starting the round.

### Ask for Confirmation Before Ending Combat

This option matters because ending combat is not just a visual close:

- it synchronizes HP and state back into linked records
- it closes the encounter flow

### Show Combat Intro to Players

If enabled, when combat starts the `Players Window` shows a short introduction with the encounter participants.

### Show Final Summary to Players

If enabled, at the end of the encounter the `Players Window` shows a final summary with the main character data.

## Active Participant Information

This subsection decides which current-turn information is shown to players.

You can choose to display:

- `Round`
- `HP`
- `Conditions`
- `Next turn`

## Enemy and NPC Information

This area separately manages what players can see when the active participant is:

- an enemy
- a monster
- an NPC

You can independently control:

- visibility of HP and temporary HP
- visibility of conditions
- visibility of the enemy’s real name

## Media

The `Media` section gathers preferences for image management and presentation windows.

### Fullscreen Player Images

If enabled, images shown to players open in fullscreen mode.

### DM Images on the Main Monitor

This option makes the DM window open by default on the first available screen.

### Remember DM Window Size

If enabled, when you reopen a new image for the DM, the window keeps:

- the last size
- the last position

## Media Maintenance

The `Media maintenance` area covers the more technical side of image handling.

From here you can launch `Clean unused media`, which checks the image files stored by the app and removes those no longer linked to any entity.

## Theme

The `Theme` section lets you choose the app’s **global palette**.

Each theme shows a small visual preview of its main colors, so you can immediately understand how the interface will change.

## Database

The `Database` section is one of the most important areas for data safety.

Here you can find:

- the path of the data folder
- the path of the SQLite database
- the path of the backup folder
- information about the latest snapshots

### Automatic Backup

You can choose:

- automatic backup frequency
- maximum number of automatic snapshots to keep

### Cloud Snapshots

DnDino also manages cloud snapshot behavior.

From here you can choose how cloud saves should behave and view the current state through the summary text shown in the screen.

### Main Actions

Inside the `Database` panel you find the main maintenance buttons:

- `Open data folder`
- `Open backup folder`
- `Create snapshot...`
- `Restore snapshot...`
- `Restore from iCloud`

### Reset App Data

The `Reset app data` function deletes:

- the app database
- the app media

but keeps already-created backups.

### Latest Snapshots

At the bottom of the `Database` section, DnDino also shows the list of the latest snapshots it found.

For each one, it displays:

- file name
- date
- size

## Diagnostics

The `Diagnostics` section is used to inspect the technical state of the SQLite database used by the app.

Here you can:

- refresh diagnostic data
- see the database path
- check whether the file exists
- verify file size and modification date
- see the SQLite version

### Tables

Diagnostics also shows the list of tables found in the database together with the number of records in each one.

## Support

The `Support` section gathers quick ways to contact the app developer.

Here you find:

- support email
- `Request support` button
- `Send a suggestion` button
- `Copy email` button

## Licenses

The `Licenses` section gathers the legal and attribution references used by the app.

At the moment it includes in particular the material related to the **System Reference Document 5.2** for Dungeons & Dragons, with references to:

- the SRD document
- the `CC-BY-4.0` license

!!! tip
    If you are configuring DnDino for the first time, the most useful sections to check first are `General`, `Top Bar`, `Combat`, and `Database`. Those are usually the ones that affect day-to-day use and data safety the most.
