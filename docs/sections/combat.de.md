# Kampf

Der **Kampf**-Modus von DnDino ist als zentraler operativer Tracker für eine Begegnung gedacht. Diese Seite beschreibt den Standard-Kampfmodus von DnDino.

Ein Kampf entsteht immer im Kontext eines **Ortes** und übernimmt die verknüpften Charaktere, lokalen Anwesenden sowie alle Monster oder NSC, die zu dieser Szene gehören.

Diese Seite erklärt den vollständigen Ablauf:

- Vorbereitung im Vorkampf
- Verwaltung der Teilnehmenden
- Start der Begegnung
- Nutzung des Panels für den aktuellen Zug
- Anwenden von Schaden, Heilung, Zuständen und Rettungswürfen
- Integration mit dem **Spielerfenster**
- Abschluss der Begegnung und die Endzusammenfassung

## Nutzung mit einem oder zwei Bildschirmen

DnDinos Kampf funktioniert auch auf **einem einzigen Bildschirm** sehr gut: Die komplette operative Seite bleibt im Hauptpanel, und du kannst Teilnehmende, Züge, Schaden, Zustände und die Endzusammenfassung ohne zweiten Monitor verwalten.

Wenn du jedoch ein Setup mit zwei Bildschirmen hast, kannst du verwenden:

- einen Hauptbildschirm für das Kontrollpanel des SL
- einen zweiten Bildschirm oder Monitor für das **Spielerfenster**

In dieser Konfiguration wird der Ablauf noch angenehmer:

- auf dem SL-Bildschirm bleiben Teilnehmendenliste, Rundenkontrollen, aktueller Zug, Angriffstexte, SL-Notizen und Schnellbearbeitungen sichtbar
- auf dem Bildschirm der Spielenden erscheint eine saubere Präsentation des aktiven Teilnehmenden mit Bild und kontextbezogenem Overlay

Praktisch bedeutet das:

- auf einem Bildschirm steuerst du den gesamten Kampf über die Hauptansicht
- mit zwei Bildschirmen trennst du das technische SL-Panel von der Darstellung für die Spielenden

!!! tip
    Ein zweiter Bildschirm ist nicht Pflicht. Er ist einfach eine sehr nützliche Erweiterung, wenn du den Spielenden Bilder und Informationen zum aktuellen Zug zeigen möchtest, ohne das technische Panel des SL offenzulegen.

## So funktioniert das Spielerfenster während des Kampfes

Wenn der Kampf gestartet wird, kann DnDino das **Spielerfenster** automatisch öffnen oder aktualisieren.

Wenn die Präsentation für die Spielenden aktiv ist:

- kann zu Beginn des Kampfes eine kurze **Intro** mit den Teilnehmenden erscheinen
- aktualisiert sich das Fenster während des Kampfes auf den **Teilnehmenden des aktuellen Zugs**
- kann am Ende der Begegnung eine **Endzusammenfassung** erscheinen

Während des Kampfes zeigt das Spielerfenster nicht das technische Panel des SL, sondern eine visuelle Präsentation mit:

- dem Bild des aktiven Teilnehmenden
- dem Namen, der den Spielenden gezeigt wird
- Overlay-Informationen, sofern aktiviert

Das Overlay kann enthalten:

- aktuelle Runde
- aktuelle, maximale und temporäre TP
- Zustände
- nächster Zug

Informationen über Feinde können getrennt von Informationen über Helden behandelt werden.

## Einstellungen für Spielerfenster und zweiten Bildschirm

Die wichtigsten Optionen befinden sich in **Einstellungen**, im Bereich für Kampfpräsentation und Spielerfenster.

### Öffnung und allgemeines Verhalten

Die wichtigsten Einstellungen sind:

- `Spielerfenster auch mit nur einem Monitor öffnen`
- `Steuerung des Spielerfensters in der Topbar anzeigen`
- `Kampf-Intro für Spielende anzeigen`
- `Endzusammenfassung für Spielende anzeigen`

#### Spielerfenster auch mit nur einem Monitor öffnen

Wenn diese Option aktiv ist, kann DnDino das Spielerfenster auch dann automatisch öffnen, wenn du nur mit einem Monitor arbeitest.

Wenn sie deaktiviert ist:

- öffnet sich das Fenster auf einem einzelnen Monitor nicht automatisch
- ist es bereits geöffnet, wird es trotzdem weiter aktualisiert

#### Steuerung des Spielerfensters in der Topbar anzeigen

Wenn du diese Option aktivierst, erscheinen in der oberen Leiste Schaltflächen, um:

- das Spielerfenster manuell zu öffnen
- es manuell zu schließen

#### Kampf-Intro für Spielende anzeigen

Wenn du `Begegnung starten` drückst, kann das Spielerfenster eine kurze Einleitung anzeigen mit:

- Titel der Begegnung
- beteiligten Teilnehmenden
- Anzahl der Teilnehmenden

Wenn du diese Option deaktivierst, springt der Kampf direkt zur Darstellung des ersten aktiven Teilnehmenden.

#### Endzusammenfassung für Spielende anzeigen

Wenn der Kampf endet, kann das Spielerfenster eine Endzusammenfassung anzeigen.

Die spielerseitige Zusammenfassung zeigt nur Informationen, die für Spielende nützlich sind, zum Beispiel:

- von Helden verursachter Schaden
- von Helden erlittenen Schaden
- das Bild des gefährlichsten Gegners

Die Endzusammenfassung bleibt sichtbar, bis du den Inhalt des Fensters änderst oder es schließt.

### Informationen während eines Zugs

Die Einstellungen, die das Overlay des aktiven Teilnehmenden steuern, sind:

- `Runde im Spielerfenster anzeigen`
- `TP im Spielerfenster anzeigen`
- `Zustände im Spielerfenster anzeigen`
- `Nächsten Zug im Spielerfenster anzeigen`

### Informationen zu Feinden, Monstern und NSC

Für Teilnehmende, die keine Helden sind, gibt es eigene Steuerelemente:

- `NSC- und Monsterdetails für Spielende anzeigen`
- `Zustände von Feinden für Spielende anzeigen`
- `Namen von Feinden für Spielende anzeigen`

Damit kannst du entscheiden, ob das Spielerfenster:

- die Kreatur eher atmosphärisch zeigt
- oder zusätzlich technische Informationen einblendet

## Wo der Kampf geöffnet wird

Der Kampf wird aus dem Kontext eines **Ortes** erstellt. Nach dem Öffnen zeigt DnDino ein Layout mit zwei Hauptspalten:

- links den operativen Kampf-Tracker
- in der Mitte das Hauptpanel der Szene oder des aktuellen Zugs

Bevor der Kampf begonnen hat, zeigt das mittlere Panel die **Vorkampf-Zusammenfassung**.

Sobald die Begegnung aktiv ist, wird dieses Panel zum Bereich für den **Aktuellen Zug**.

Wenn der Kampf beendet ist, zeigt das mittlere Panel die **Abschlusszusammenfassung der Begegnung** für den SL.

## Allgemeine Struktur des Bildschirms

### Linke Spalte

Die linke Spalte enthält:

- `Kampfsteuerung`
- die Kopfzeile der Teilnehmendenliste
- die sortierte Liste der Teilnehmenden

Die Liste ist von zwei dekorativen und funktionalen Zeilen eingerahmt:

- `Rundenbeginn`
- `Rundenende`

### Mittleres Panel

Das mittlere Panel wechselt je nach Kampfstatus:

- **vor dem Start** zeigt es die Vorkampf-Zusammenfassung
- **während des Kampfes** zeigt es den Teilnehmenden des aktuellen Zugs
- **nach dem Kampf** zeigt es die Abschlusszusammenfassung des SL

## Vorkampf

Der Vorkampf dient dazu, die Begegnung vorzubereiten, bevor der erste Zug beginnt.

Hier lohnt es sich vor allem, drei Dinge anzupassen:

- die Namen der Monster, wenn du sie am Tisch klarer unterscheiden möchtest
- die Initiative der Helden, indem du sie manuell einträgst
- die Initiative von NSC und Monstern, indem du sie automatisch würfelst oder manuell einträgst

## Vorkampf-Zusammenfassung

Die Startkarte zeigt eine schnelle Übersicht mit Kennzahlen wie:

- Teilnehmende
- Helden
- Verbündete
- Feinde
- gesamte TP der Feinde
- Teilnehmende, die bereits in einem kritischen Zustand sind

## Charakterinitiative

Der Bereich `Charakterinitiative` sammelt die wichtigsten Helden und erlaubt es dir, ihre Initiative schnell zu bearbeiten, bevor die Begegnung sortiert wird.

Jede Zeile enthält:

- Namen des Teilnehmenden
- kontextbezogenen Untertitel
- Initiativfeld
- Schaltfläche `Löschen`

## NSC und Monster

Der Bereich `NSC und Monster` ist für Teilnehmende gedacht, die keine Helden sind.

Hier kannst du:

- Initiative schnell bearbeiten
- Monster und NSC im Handumdrehen umbenennen
- `Init NSC/Monster` verwenden, um Initiative automatisch zu würfeln
- Initiative manuell eintragen, wenn du den Wurf außerhalb der App benutzt
- einen Teilnehmenden schnell mit `Löschen` entfernen

## Hauptaktionen im Vorkampf

Die wichtigsten Aktionen in der Vorkampf-Zusammenfassung sind:

- `Hinzufügen`
- `Sortieren`
- `Begegnung starten`

Wenn mindestens ein Teilnehmender noch Initiative `0` hat, fragt DnDino vor dem Start nach einer Bestätigung.

## Woher Teilnehmende kommen können

Das Panel zum Hinzufügen von Teilnehmenden kann aus drei Quellen ziehen:

- `Helden`
- `Anwesende am Ort`
- `Global`

### Helden

Hier findest du Abenteuercharaktere, die bereits mit der Kampagne verknüpft sind. Jeder Held kann nur einmal in den Kampf eintreten.

### Anwesende am Ort

Hier findest du Charaktere, die bereits an dem Ort anwesend sind, aus dem der Kampf entsteht. Ihr lokaler Zustand kann als Basis für die Begegnung wiederverwendet werden.

### Global

Hier findest du Grundbögen, die nicht bereits als Abenteuerhelden verknüpft sind.

Für globale Einträge gilt:

- `Monster` können mehrfach hinzugefügt werden
- globale `Helden` und `NSC` können nicht als reine globale Bögen dupliziert werden

## Kampfsteuerung

Sobald die Begegnung begonnen hat, bleibt das Panel `Kampfsteuerung` oberhalb der Liste fixiert und enthält die wichtigsten Aktionen der Runde.

Die Schaltflächen sind in folgenden Zeilen angeordnet:

1. `Hinzufügen` und `Sortieren`
2. `Start/Pause` oder `Fortsetzen` und `Ende`
3. `Zurück` und `Weiter`

Wenn es einen rückgängig machbaren letzten Angriff gibt, erscheint zusätzlich:

- `Letzten Angriff rückgängig machen`

## Teilnehmendenliste

Die Liste auf der linken Seite ist das Herzstück des taktischen Trackings.

Jede eingeklappte Zeile zeigt:

- Position in der Zugreihenfolge, zum Beispiel `1/8`
- Name des Teilnehmenden
- bis zu drei Zustands-Icons
- Badge `Zug`, wenn es sich um den aktiven Teilnehmenden handelt
- RK
- TP
- temporäre TP
- Initiative

Der aktive Teilnehmende ist deutlich stärker hervorgehoben als die anderen:

- farbiges Seitenband
- stärkere Umrandung
- wärmerer Hintergrund
- automatisches Scrollen, um ihn sichtbar zu halten

Die Zeile verwendet außerdem Wirkungseffekte, wenn der Teilnehmende:

- Schaden erhält
- getötet wird
- durch ein Undo wiederhergestellt wird

## Kontextmenü einer Zeile

Mit einem **Rechtsklick** auf die Karte eines Teilnehmenden kannst du das Kontextmenü öffnen.

Derzeit verfügbare Aktion:

- `Löschen`

## Aufklappen einer Teilnehmendenzeile

Wenn du auf eine Zeile klickst, wird sie erweitert und zeigt ihre Schnellkontrollen.

Im erweiterten Bereich findest du:

- bearbeitbaren Namen
- schnelle Zahlenfelder:
  - Initiative
  - TP
  - temporäre TP
  - RK
- Aktionsschaltflächen
- Zustandsblock
- Zugriff auf Fähigkeiten, Spezialfähigkeiten und Zauber, falls vorhanden

## Schnellschaltflächen der Zeile

Die Schnellaktionen können enthalten:

- `Angriff`
- `Schaden`
- `Heilung`
- `RW`
- `SL-Notizen`
- `Bearbeiten`
- `Zustände`

Einige Schaltflächen erscheinen nur, wenn sie für diesen Teilnehmenden sinnvoll sind.

## Angriff

`Angriff` öffnet ein Popover, in dem du auswählen kannst:

- ein oder mehrere Ziele
- den anzuwendenden Schaden

Die Zielauswahl verwendet eine kompakte Liste mit:

- Name
- RK
- TP
- Zustände

Die Zielreihenfolge ist nicht zufällig. DnDino versucht, dir zuerst die sinnvollsten Teilnehmenden vorzuschlagen – abhängig davon, wer angreift.

Im Allgemeinen:

- wenn ein **Held** angreift, kommen zuerst **Feinde**, dann Verbündete, dann Neutrale und zuletzt niedrig priorisierte Monster
- wenn ein Nicht-Held angreift, kommen zuerst **Helden**, dann Verbündete, dann Neutrale und zuletzt weniger passende Feinde

Innerhalb jeder Gruppe werden die Namen anschließend alphabetisch sortiert.

Das Popover wählt nie automatisch ein Ziel vor. Die Auswahl muss manuell erfolgen.

Wenn du einen Angriff auf mehrere Ziele anwendest:

- wird der Schaden auf alle ausgewählten Ziele angewendet
- zeigt das obere Banner mehrere Zeilen, eine pro getroffenem Ziel
- speichert das Undo des letzten Angriffs die gesamte Gruppe zusammen

## Schaden und Heilung

`Schaden` wendet direkten Schaden auf den Teilnehmenden an.

`Heilung` wendet direkte Heilung an.

## RW

`RW` öffnet das Popover für den **Rettungswurf** auf Basis der Werte des Teilnehmenden.

## Zustände

Die Schaltfläche `Zustände` öffnet das Popover zur Verwaltung aktiver Zustände.

Von dort aus kannst du:

- Zustände hinzufügen
- Dauer und Ablaufregeln festlegen
- das Ende eines Zustands an den Zug eines anderen Teilnehmenden koppeln

## SL-Notizen

Die Schaltfläche `SL-Notizen` ist immer sichtbar.

Sie öffnet ein bearbeitbares Popover, in dem du kontextbezogene Notizen zum Teilnehmenden schreiben kannst. Der Inhalt wird gespeichert, sobald das Popover geschlossen wird.

## Bearbeiten

`Bearbeiten` öffnet den Editor des Teilnehmenden.

Er ist nützlich, wenn du tiefer eingreifen musst in:

- Initiative
- RK
- maximale, aktuelle und temporäre TP
- Rolle im Kampf
- verknüpfte Kontextdaten

## Aktueller Zug

Wenn der Kampf aktiv ist, konzentriert sich das mittlere Panel vollständig auf den Teilnehmenden, der gerade am Zug ist.

Die obere Karte zeigt:

- Bild des Teilnehmenden
- Name
- Untertitel
- RK
- TP
- temporäre TP
- Initiative
- Bewegungsrate
- Inspiration, wenn der Teilnehmende ein Abenteuerheld ist
- aktive Zustände
- wichtigste Werte

## Mittlere Panels während des Zugs

Unter der Zugübersicht werden nur Panels mit echtem Inhalt angezeigt.

Mögliche Bereiche sind:

- `Angriffe`
- `Spezialfähigkeiten`
- `Fähigkeiten`
- `Beschreibung`
- `Zauber`

Alle diese Panels sind einklappbar.

Außerdem nutzen sie leichte visuelle Akzente:

- `Angriffe` rot
- `Fähigkeiten` gelb
- `Spezialfähigkeiten` grün
- `Zauber` hellblau
- `Beschreibung` grau

## Angriffe und interne Links

Der Bereich `Angriffe` ist eine der stärksten Seiten des Flat-Kampfes.

Wenn du im Angriffstext des Grundbogens interne Links vorbereitet hast, kannst du sie direkt im Kampf verwenden.

Insbesondere der Link **Kompletter Angriff** ist sehr nützlich, weil er:

- Angriffswurf und Schaden im selben Popover ausführt
- ein oder mehrere Ziele auswählen lässt
- automatisch `Anzuwendender Schaden` vorschlägt
- erlaubt, einzelne Schadenszeilen auszuschließen, wenn du mehrere Komponenten gewürfelt hast und nur einige anwenden willst
- das Popover schließt, sobald der Schaden angewendet wurde

Dadurch lassen sich Monsterangriffe am Tisch sehr schnell abwickeln.

## Charaktere bei 0 TP oder weniger

Im Kampf folgen **Helden** einer anderen Regel als NSC und Monster.

### Helden

Helden können unter `0` TP fallen.

Die Regel lautet:

- zwischen `0` und `-(max. TP - 1)` ist der Charakter **Bewusstlos**
- bei `-max. TP` oder weniger stirbt der Charakter endgültig

Wenn ein Held `0` TP oder weniger hat, aber nicht endgültig tot ist:

- bleibt er in der Begegnung
- zeigt das mittlere Panel die Karte `Todesrettungswürfe`

Diese Karte verfolgt:

- Erfolge
- Fehlschläge

und erlaubt es dir, schnell zu markieren:

- `Erfolg`
- `Fehlschlag`

Bei 3 Erfolgen kehrt der Charakter mit `1` TP zurück. Bei 3 Fehlschlägen stirbt er.

### NSC und Monster

Für Nicht-Helden ist das Verhalten einfacher:

- bei `0` TP oder weniger sind sie tot

## Züge, Runden und aus dem Zyklus entfernte Teilnehmende

Innerhalb des Zugzyklus gilt:

- endgültig tote Helden werden ausgeschlossen
- NSC und Monster bei `0` TP oder weniger werden ausgeschlossen

Das bedeutet, dass ein **bewusstloser** Held weiterhin einen Zug haben kann, weil seine Todesrettungswürfe noch verwaltet werden müssen.

## Trefferbanner und visuelles Feedback

Wenn ein Angriff trifft, zeigt DnDino oben ein großes Banner mit einer sofortigen Zusammenfassung.

Zum Beispiel:

- wer getroffen hat
- wer getroffen wurde
- wie viel Schaden angewendet wurde
- ob der Schlag das Ziel getötet hat

Wenn es mehrere Ziele gibt, zeigt das Banner mehrere Zeilen im selben Kasten.

Auch das **Spielerfenster** kann die Trefferanimation zeigen, einschließlich aller Ziele, die in denselben Mehrfachangriff einbezogen waren.

## Letzten Angriff rückgängig machen

Wenn du einen Angriff anwendest, erscheint das Panel

- `Letzten Angriff rückgängig machen`

Unter der Schaltfläche wird eine kurze Zusammenfassung dessen angezeigt, was gerade passiert ist.

Wenn der letzte Angriff mehrere Ziele getroffen hat, zeigt das Panel die vollständige Liste der Zeilen, die wiederhergestellt werden.

Wenn du das Undo bestätigst:

- kehren die Ziele in ihren vorherigen Zustand zurück
- erscheint eine Wiederherstellungsbenachrichtigung
- wird auch das visuelle Feedback der Karten aktualisiert

## Abschlusszusammenfassung der Begegnung

Wenn der Kampf endet, wechselt das mittlere Panel zur **Abschlusszusammenfassung der Begegnung** für den SL.

Dieser Bildschirm zeigt:

- gesamte Runden
- Dauer
- getötete Feinde
- verursachten Schaden
- erlittenen Schaden

## Was am Ende synchronisiert wird

Wenn du den Kampf schließt, speichert DnDino das Ergebnis zurück in die verknüpften Datensätze.

Für Abenteuerhelden werden synchronisiert:

- aktuelle TP
- temporäre TP
- manuelle Zustände
- Endzustand

Für Orts-Anwesende mit lokalem Zustand werden synchronisiert:

- aktuelle TP
- temporäre TP
- manuelle Zustände
- Endzustand

Der Kampf aktualisiert außerdem die verknüpften Daten der **Live-Session**, darunter:

- verursachten Schaden
- erlittenen Schaden
- gefallene Helden

## Wann der Kampf am meisten glänzt

DnDinos Kampf glänzt am meisten, wenn du ihn so einsetzt:

1. du bereitest den Vorkampf gut vor
2. du nutzt zwei Bildschirme zusammen mit dem **Spielerfenster**
3. du nutzt Angriffslinks für Monster und NSC
4. du behältst den SL auf dem Tracker und die Spielenden auf der Präsentation

!!! tip
    Auch wenn der Kampf viele Automatismen für Würfe, komplette Angriffe und schnelles Anwenden von Schaden bietet, lässt DnDino weiterhin Raum für eine klassischere Nutzung von Würfeln. Du kannst weiterhin physisch würfeln oder den Wurf außerhalb der App handhaben und den Kampf vor allem dafür nutzen, Werte schnell und konsistent anzuwenden – ohne den mühsamsten Teil: TP-Änderungen jedes Mal von Hand neu auszurechnen.
