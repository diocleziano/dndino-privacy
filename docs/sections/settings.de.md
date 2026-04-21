# Einstellungen

Der Bereich **Einstellungen** sammelt die globalen Voreinstellungen von DnDino. Hier arbeitest du nicht an einem einzelnen Abenteuer oder Charakter, sondern legst fest, **wie sich die App insgesamt verhalten soll**.

Die Einstellungen beeinflussen vor allem:

- das allgemeine Erscheinungsbild der Oberfläche
- das Verhalten der Topbar
- den Ablauf in `Orte`
- das Verhalten des `Kampfs`
- die Verwaltung von Bildern, Backups und Snapshots
- Support und Diagnose der Datenbank

## Aufbau des Bildschirms

Die Seite ist in zwei Bereiche aufgeteilt:

- eine **linke Seitenleiste** mit Kategorien
- ein **Hauptpanel** rechts mit den Optionen des ausgewählten Bereichs

Verfügbare Kategorien sind:

- `Allgemein`
- `Topbar`
- `Orte`
- `Kampf`
- `Medien`
- `Thema`
- `Datenbank`
- `Diagnose`
- `Support`
- `Lizenzen`

Diese Struktur trennt alltagsnahe Einstellungen sauber von technischeren Bereichen wie Backups und Diagnose.

## Allgemein

Der Bereich `Allgemein` enthält die grundlegenden Einstellungen der App.

### SL-Profil

Hier kannst du dein Profil anpassen mit:

- `Benutzername`
- `Geschlecht`

Der Name wird auch an anderen Stellen in der App verwendet, zum Beispiel in der Begrüßung der `Home`.

### Oberflächensprache

Du kannst entscheiden, ob DnDino:

- der Systemsprache folgen soll
- oder eine bestimmte App-Sprache erzwingen soll

### Globale Bestätigungen

Die Option `Bestätigung für Löschvorgänge anfordern` fügt vor destruktiven Aktionen wie Entfernen und Löschen eine Bestätigung ein.

### Metadaten

Unter `Allgemein` findest du außerdem:

- `Metadaten in der App anzeigen`

Diese Option legt fest, ob Metadaten-Panels in den Bildschirmen angezeigt werden sollen, die sie unterstützen.

### Layout der Panels im Abenteuer-Dashboard

Dieser Teil ist wichtig, wenn du das `Abenteuer-Dashboard` häufig verwendest.

Du kannst:

- Panels ziehen
- sie innerhalb der linken oder rechten Spalte neu anordnen
- sie zwischen den Spalten verschieben

### Aktives Thema

Unter `Allgemein` wird außerdem das **aktuell ausgewählte Thema** als schnelle Übersicht angezeigt. Das eigentliche Umschalten erfolgt im Bereich `Thema`.

### Einführungshinweise

Von hier aus kannst du das Erstverhalten der App zurücksetzen.

Die Schaltfläche `Erstnutzung zurücksetzen` weist DnDino an, kontextbezogene Hilfen und Onboarding-Abläufe erneut als ungesehen zu behandeln.

## Topbar

Der Bereich `Topbar` definiert das Verhalten der Schnellwerkzeuge in der oberen Leiste der App.

### Darstellung der Topbar

Du kannst wählen, ob die Topbar angezeigt wird:

- nur mit Symbolen
- oder mit Symbolen und Namen darunter

### Standardwürfel

DnDino enthält einen schnellen Würfelroller in der Topbar. Hier kannst du den **Standardwürfeltyp** festlegen, der beim Öffnen vorgeschlagen wird.

### Schnelles Öffnen von Charakteren

Diese Einstellung steuert das Verhalten des schnellen Öffnens von Charakteren aus der Topbar.

Du kannst entscheiden, ob die Abkürzung zu:

- einer stärker lesefokussierten Ansicht
- oder zu einem eher bearbeitungsnahen Modus

führen soll.

### Schnelles Öffnen von Regeln

Die Topbar erlaubt auch ein schnelles Öffnen der `Regeln`.

Hier kannst du festlegen, ob diese Abkürzung:

- den vollständigen Editor
- oder ein kompakteres, stärker auf Nachschlagen ausgerichtetes Fenster

öffnen soll.

### Steuerung des Spielerfensters in der Topbar

Die Option `Steuerung des Spielerfensters in der Topbar anzeigen` fügt in der oberen Leiste Schaltflächen hinzu, um das `Spielerfenster` manuell zu öffnen oder zu schließen.

## Orte

Der Bereich `Orte` enthält globale Einstellungen, die als Standardverhalten im Orte-Dashboard verwendet werden.

### Standardrolle für Anwesende

Wenn du einem Ort einen Anwesenden hinzufügst, kann DnDino eine Standardrolle vorschlagen.

### Karten übergeordneter Orte standardmäßig anzeigen

Wenn diese Option aktiv ist, werden im Bildschirm `Orte` geerbte Karten übergeordneter Orte direkt sichtbar angezeigt.

### Zuletzt besuchten Ort merken

Wenn aktiv, versucht die App beim Zurückkehren in den Bildschirm `Orte`, den zuletzt ausgewählten Ort für dieses Abenteuer wiederherzustellen.

### Vorherigen Ort automatisch schließen

Diese Einstellung gilt während einer **aktiven Live-Session**.

Wenn ein Ort auf `In Besuch` gesetzt wird, wird der zuvor `In Besuch` befindliche Ort automatisch als `Besucht` markiert.

## Kampf

Der Bereich `Kampf` bündelt die globalen Einstellungen des Kampfsystems.

Hier findest du sowohl Darstellungsoptionen als auch Einstellungen, die den praktischen Ablauf einer Begegnung und des `Spielerfensters` beeinflussen.

## Reihenfolge der mittleren Panels

Du kannst die Reihenfolge der mittleren Kampfpanels ändern, indem du Elemente wie diese ziehst:

- `Angriffe`
- `Spezialfähigkeiten`
- `Fähigkeiten`
- `Zauber`
- `Beschreibung`

## Kampfpräsentation

Dieser Unterbereich steuert das allgemeine Verhalten des Kampfs und der Darstellung für Spielende.

### Zug standardmäßig für Spielende anzeigen

Wenn aktiv, starten neue Kämpfe bereits mit aktivierter automatischer Zugpräsentation.

### Spielerfenster auch mit nur einem Monitor öffnen

Diese Einstellung steuert das automatische Verhalten des `Spielerfensters` in Ein-Bildschirm-Setups.

### Details des Teilnehmenden im aktuellen Zug automatisch anzeigen

Wenn der Zug wechselt, kann die App:

- den aktiven Teilnehmenden automatisch auswählen
- auch dessen Detailansicht öffnen

### Beim Start automatisch nach Initiative sortieren

Wenn du `Kampf starten` drückst, kann DnDino die Teilnehmenden automatisch nach Initiative sortieren, bevor die Runde beginnt.

### Vor dem Beenden des Kampfs Bestätigung anfordern

Diese Option ist wichtig, weil das Beenden eines Kampfs nicht nur eine visuelle Schließung ist:

- TP und Status werden auf verknüpfte Datensätze zurückgeschrieben
- der Begegnungsfluss wird abgeschlossen

### Kampf-Intro für Spielende anzeigen

Wenn aktiv, zeigt das `Spielerfenster` beim Start eines Kampfs eine kurze Einführung mit den Teilnehmenden der Begegnung.

### Endzusammenfassung für Spielende anzeigen

Wenn aktiv, zeigt das `Spielerfenster` am Ende der Begegnung eine Endzusammenfassung mit den wichtigsten Charakterdaten.

## Informationen zum aktiven Teilnehmenden

Dieser Unterbereich entscheidet, welche Informationen über den aktuellen Zug den Spielenden angezeigt werden.

Du kannst auswählen, ob sichtbar sein sollen:

- `Runde`
- `TP`
- `Zustände`
- `Nächster Zug`

## Informationen zu Feinden und NSC

Dieser Teil verwaltet separat, was Spielende sehen, wenn der aktive Teilnehmende ein:

- Feind
- Monster
- NSC

ist.

Du kannst unabhängig steuern:

- Sichtbarkeit von TP und temporären TP
- Sichtbarkeit von Zuständen
- Sichtbarkeit des echten Feindnamens

## Medien

Der Bereich `Medien` bündelt Einstellungen zur Bildverwaltung und zu Präsentationsfenstern.

### Bilder für Spielende im Vollbild

Wenn aktiv, werden Bilder, die den Spielenden gezeigt werden, im Vollbild geöffnet.

### SL-Bilder auf dem Hauptmonitor

Diese Option sorgt dafür, dass das SL-Fenster standardmäßig auf dem zuerst verfügbaren Bildschirm geöffnet wird.

### Größe des SL-Fensters merken

Wenn aktiv, behält das SL-Fenster beim erneuten Öffnen eines Bildes:

- die letzte Größe
- die letzte Position

## Medienwartung

Der Bereich `Medienwartung` deckt die technische Seite der Bildverwaltung ab.

Von hier aus kannst du `Nicht verwendete Medien bereinigen` starten. Dabei prüft die App gespeicherte Bilddateien und entfernt solche, die nicht mehr mit irgendeiner Entität verknüpft sind.

## Thema

Der Bereich `Thema` erlaubt dir die Auswahl der **globalen Farbpalette** der App.

Jedes Thema zeigt eine kleine visuelle Vorschau seiner Hauptfarben, damit du sofort sehen kannst, wie sich die Oberfläche verändern wird.

## Datenbank

Der Bereich `Datenbank` ist einer der wichtigsten für die Datensicherheit.

Hier findest du:

- den Pfad des Datenordners
- den Pfad der SQLite-Datenbank
- den Pfad des Backup-Ordners
- Informationen über die neuesten Snapshots

### Automatisches Backup

Du kannst wählen:

- die Frequenz des automatischen Backups
- die maximale Anzahl automatischer Snapshots, die aufbewahrt werden sollen

### Cloud-Snapshots

DnDino verwaltet auch das Verhalten von Cloud-Snapshots.

Hier kannst du festlegen, wie sich Cloud-Sicherungen verhalten sollen, und den aktuellen Status über den Zusammenfassungstext im Bildschirm ablesen.

### Hauptaktionen

Im Panel `Datenbank` findest du die wichtigsten Wartungsschaltflächen:

- `Datenordner öffnen`
- `Backup-Ordner öffnen`
- `Snapshot erstellen...`
- `Snapshot wiederherstellen...`
- `Aus iCloud wiederherstellen`

### App-Daten zurücksetzen

Die Funktion `App-Daten zurücksetzen` löscht:

- die App-Datenbank
- die App-Medien

behält jedoch bereits erstellte Backups.

### Letzte Snapshots

Im unteren Teil des Bereichs `Datenbank` zeigt DnDino außerdem die Liste der zuletzt gefundenen Snapshots an.

Für jeden Snapshot werden angezeigt:

- Dateiname
- Datum
- Größe

## Diagnose

Der Bereich `Diagnose` dient dazu, den technischen Zustand der von der App verwendeten SQLite-Datenbank zu prüfen.

Hier kannst du:

- Diagnosedaten aktualisieren
- den Datenbankpfad sehen
- prüfen, ob die Datei existiert
- Dateigröße und Änderungsdatum überprüfen
- die SQLite-Version sehen

### Tabellen

Die Diagnose zeigt außerdem die Liste der in der Datenbank gefundenen Tabellen zusammen mit der Anzahl der Datensätze in jeder einzelnen.

## Support

Der Bereich `Support` bündelt die schnellen Wege, um die entwickelnde Person der App zu kontaktieren.

Hier findest du:

- die Support-E-Mail
- die Schaltfläche `Support anfordern`
- die Schaltfläche `Vorschlag senden`
- die Schaltfläche `E-Mail kopieren`

## Lizenzen

Der Bereich `Lizenzen` sammelt die rechtlichen Hinweise und Quellenangaben, die von der App verwendet werden.

Derzeit enthält er insbesondere den Teil zum **System Reference Document 5.2** von Dungeons & Dragons mit Verweisen:

- auf das SRD-Dokument
- auf die Lizenz `CC-BY-4.0`

!!! tip
    Wenn du DnDino zum ersten Mal einrichtest, sind die nützlichsten Bereiche, die du sofort prüfen solltest, `Allgemein`, `Topbar`, `Kampf` und `Datenbank`. Das sind in der Regel die Bereiche, die sich am stärksten auf den täglichen Einsatz und auf die Datensicherheit auswirken.
