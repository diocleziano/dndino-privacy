# Abenteuer

Der Bereich **Abenteuer** ist das organisatorische Zentrum einer Kampagne in DnDino. Hier entsteht die Hauptstruktur deiner Arbeit: der Titel der Kampagne, ihre visuelle Identität, die verknüpften Charaktere, Sitzungen, Orte, gemeinsame Bilder, Karten und die Schnellzugriffe auf Kämpfe.

!!! tip
    Stell dir das Abenteuer-Dashboard als das **Hauptquartier der Kampagne** vor: Es ist nicht der Ort, an dem du jede Einzelheit bearbeitest, sondern der Ort, von dem aus du schnell alle wirklich operativen Bereiche erreichst.

Diese Seite erklärt den Hauptablauf:

- Erstellung eines neuen Abenteuers
- Bearbeitung und Verwaltung eines bestehenden Abenteuers
- Funktionsweise des Abenteuer-Dashboards
- Verhältnis zwischen dem Dashboard und den zugehörigen Unterseiten

Spezifischere Bereiche wie **Orte**, **Konzeptkarten**, **Live-Sitzung**, **Charaktere**, **Bilder** und **Karten** werden auf den jeweiligen Unterseiten vertieft.

## Wozu ein Abenteuer dient

In DnDino ist ein Abenteuer der Hauptcontainer für eine Kampagne oder einen Erzählbogen. Es sammelt in einem gemeinsamen Kontext:

- die mit der Kampagne verknüpften Charaktere
- Orte und Quests
- Textsitzungen und Live-Sitzungen
- gemeinsame Bilder
- Karten, die mit Orten verbunden sind
- globale Konzeptkarten
- Kämpfe, die in Orten entstehen, die zum Abenteuer gehören

Ein Abenteuer ist also nicht nur ein Stammdatensatz, sondern der Einstiegspunkt in den operativen Teil der Kampagne.

## Wo ein Abenteuer erstellt wird

Die Erstellung beginnt in der **Abenteuerliste**.

Von dort aus kannst du:

- mit dem Button `Neu` ein neues Abenteuer anlegen
- das erste Abenteuer mit dem großen zentralen Button `Ein Abenteuer erstellen` anlegen, wenn die Datenbank noch leer ist
- ein bestehendes Abenteuer öffnen, indem du auf seine Zeile klickst
- ein bestehendes Abenteuer bearbeiten
- ein vorhandenes Abenteuer klonen
- ein Abenteuer löschen

Die Liste kann außerdem sortiert werden nach:

- Name
- Erstellungsdatum
- letzter Änderung

!!! note
    Wenn du nach **letzter Änderung** sortierst, schaut DnDino nicht nur auf den Abenteuerdatensatz selbst, sondern berücksichtigt auch verbundene Aktivität wie Orte, Sitzungen, Abenteuer-Charaktere, Konzeptkarten und Kämpfe.

## Ein neues Abenteuer erstellen

Wenn du das Erstellungsformular öffnest, zeigt DnDino dir die wichtigsten Kampagneninformationen.

Die Hauptfelder sind:

- `Titel`
- `Autor`
- `Setting`
- `Kurzbeschreibung`
- `Status`

Das Feld **Status** verwendet eine segmentierte Auswahl und erlaubt es, das Abenteuer als zu markieren:

- nicht begonnen
- laufend
- abgeschlossen

## Erweiterte Beschreibung

Unter den Hauptinformationen findest du außerdem einen größeren Bereich **Beschreibung**.

Dieser Bereich dient dazu, eine ausführlichere Darstellung der Kampagne festzuhalten, zum Beispiel:

- den Ton des Abenteuers
- den erzählerischen Kontext
- anfängliche Ziele
- allgemeine Notizen für den Spielleiter

Die lange Beschreibung geht im Dashboard nicht verloren: Falls vorhanden, kann sie dort auch später schnell wieder geöffnet werden.

## Cover und Abenteuerbilder

Im Formular kannst du dem Abenteuer ein **Coverbild** zuweisen. Dieses Cover dient in den Hauptansichten als repräsentatives Bild der Kampagne.

Du kannst auch Bilder im Bereich **Abenteuerbilder** hinzufügen. Diese Bilder:

- bleiben mit dem Abenteuer verknüpft
- gehören zu keinem bestimmten Ort
- können vom Dashboard aus schnell den Spielern oder dem Spielleiter gezeigt werden

Für jedes Bild kannst du verwalten:

- den angezeigten Namen
- Sichtbarkeit für `Spieler`
- Sichtbarkeit für `Spielleiter`

## Ein bestehendes Abenteuer bearbeiten

Wenn du ein bestehendes Abenteuer zur Bearbeitung öffnest, ist das Formular im Wesentlichen dasselbe wie bei der Erstellung, enthält aber einen zusätzlichen Abschnitt: **Abenteuer zurücksetzen**.

Das Zurücksetzen löscht nicht die Struktur der Kampagne, sondern setzt den aktuellen Spielzustand zurück. Insbesondere:

- werden alle verknüpften Abenteuer-Charaktere entfernt
- werden alle gespeicherten Sitzungen gelöscht
- werden Orte und Quests auf ihren Ausgangszustand zurückgesetzt
- werden NSC und Monster wieder auf volle HP gesetzt und von Zuständen befreit
- werden vorbereitete Kämpfe zurückgesetzt, ohne ihre Struktur zu löschen

Diese Funktion ist nützlich, wenn du das Gerüst einer Kampagne wiederverwenden oder ein Abenteuer in einen sauberen Zustand zurückbringen möchtest, ohne es von Grund auf neu aufzubauen.

## Klonen und Löschen

Aus der Abenteuerliste heraus kannst du außerdem:

### Ein Abenteuer klonen

Das Klonen erstellt mithilfe des internen Duplizierungsdienstes eine Kopie der Kampagne. Das ist nützlich, wenn du:

- mit einer ähnlichen Struktur starten willst
- ein Grundgerüst wiederverwenden möchtest
- eine Variante einer bestehenden Kampagne erzeugen willst

### Ein Abenteuer löschen

Wenn du ein Abenteuer löschst, entfernt DnDino den Hauptdatensatz und startet zusätzlich die Bereinigung verknüpfter Ressourcen. Außerdem werden globale Charakterreferenzen aktualisiert, damit sie nicht mehr auf das gelöschte Abenteuer zeigen.

## Das Abenteuer-Dashboard öffnen

Wenn du in der Liste auf ein Abenteuer klickst, gelangst du in dessen **Dashboard**, das das eigentliche operative Zentrum der Kampagne ist.

Das Dashboard ist als Bildschirm mit Panels organisiert:

- ein oberer Bereich mit Kopfzeile und Live-Sitzungssteuerung
- zwei untere Spalten mit Karten für die verschiedenen Kampagnenbereiche

Die Reihenfolge der Panels kann in den App-Einstellungen angepasst werden.

## Kopfbereich des Dashboards

Der obere Teil des Dashboards sammelt die wichtigsten Informationen des Abenteuers:

- Cover
- Titel
- Status
- Kurzbeschreibung
- Setting
- Autor

Wenn das Abenteuer auch eine lange Beschreibung besitzt, erscheint ein eigener Button, um sie in einem Popover zu öffnen und zu lesen, ohne das Dashboard zu verlassen.

Von hier aus kannst du auch **Bearbeiten** öffnen, um zum Abenteuerformular zurückzukehren und die Daten zu aktualisieren.

## Live-Sitzung

Neben der Kopfzeile befindet sich das Panel **Live-Sitzung**.

Dieser Bereich dient dazu:

- eine neue Live-Sitzung für das Abenteuer zu starten
- zu sehen, ob eine Sitzung läuft oder pausiert ist
- die verstrichene Zeit zu überwachen
- die Sitzung zu pausieren
- sie zu beenden und zu speichern

Wenn die Live-Sitzung des Abenteuers aktiv ist, folgen der **globale Spieler-Kontext** und die **Orte** diesem Sitzungszusammenhang.

Falls bereits in einem anderen Abenteuer eine Live-Sitzung offen ist, macht das Dashboard das klar sichtbar und erlaubt kein paralleles Starten einer zweiten Sitzung.

## Die Panels des Dashboards

Unterhalb der Kopfzeile zeigt das Dashboard die Hauptpanels des Abenteuers.

Aktuell sind dies:

- `Orte und Quests`
- `Charaktere`
- `Sitzungen`
- `Bilder`
- `Karten`
- `Konzeptkarten`
- `Metadaten`

!!! tip
    In den Einstellungen kannst du sowohl die Spalte als auch die Reihenfolge der Panels im Abenteuer-Dashboard anpassen.

### Orte und Quests

Dieses Panel ist der Einstieg in das Orte-Dashboard.

Hier siehst du schnell:

- die Gesamtzahl der Orte
- die Gesamtzahl der Quests
- die Zahl der abgeschlossenen Quests

Zusätzlich können Schnellzugriffe erscheinen auf:

- den zuletzt nützlichen Ort
- den zuletzt nützlichen Kampf

Wenn du diese Karte öffnest, gelangst du in den Bereich, der Folgendes verwaltet:

- Orte
- Unterorte
- Anwesende
- Ortsbilder
- Karten
- interaktive Karten
- mit Orten verknüpfte Kämpfe

Dieser Teil wird auf der Unterseite **Orte** genauer beschrieben.

### Charaktere

Das Panel **Charaktere** zeigt die mit der Kampagne verknüpften Charaktere.

Hier kannst du:

- bereits verknüpfte Abenteuer-Charaktere sehen
- neue hinzufügen
- sie mit `Alle heilen` schnell vollständig versorgen
- ihren kampagnenspezifischen Zustand öffnen

Dieser Bereich ersetzt nicht den Basis-Charakterbogen, sondern zeigt die kampagnenspezifische Ebene mit Status, HP und Zuständen im jeweiligen Kontext.

Der Unterschied zwischen:

- Basis-Charakterbogen
- Abenteuer-Charakter
- Orts-Charakter
- Kampfteilnehmer

wird auf der Unterseite **Charaktere** ausführlicher erklärt.

### Sitzungen

Das Panel **Sitzungen** sammelt:

- Textsitzungen
- Live-Sitzungen
- Notizen
- Zusammenfassungen
- Timeline-Einträge

Von hier aus kannst du auch eine neue Textsitzung erstellen. Sitzungen sind damit zugleich das erzählerische Gedächtnis und das operative Protokoll der Kampagne.

Dieser Bereich wird auf der Unterseite **Live-Sitzung** und in den Sitzungsabläufen weiter vertieft.

### Bilder

Das Panel **Bilder** sammelt die globalen Abenteuerbilder, also diejenigen, die nicht an einen bestimmten Ort gebunden sind.

Von hier aus kannst du:

- Bilder hinzufügen
- sie seitenweise durchblättern
- sie schnell den Spielern zeigen
- sie schnell dem Spielleiter zeigen

Das ist der richtige Bereich für kampagnenweites Bildmaterial, das nicht zu einem einzelnen Ort gehört.

### Karten

Das Panel **Karten** zeigt alle Karten, die mit den Orten des Abenteuers verbunden sind.

Karten werden hier nicht direkt hinzugefügt: Sie erscheinen im Dashboard, sobald sie bereits mit einem Ort verknüpft wurden.

Von dieser Karte aus kannst du:

- die Karten des Abenteuers durchsuchen
- sie Spielern oder Spielleiter zeigen
- die zugehörige interaktive Karte des Ortes direkt öffnen, falls vorhanden

Dieser Teil wird auf den Unterseiten **Karten** und **Interaktive Karten** weiter ausgeführt.

### Konzeptkarten

Das Panel **Konzeptkarten** sammelt die globalen Konzeptkarten des Abenteuers.

Von hier aus kannst du:

- sehen, wie viele Konzeptkarten existieren
- sie schnell öffnen
- eine neue anlegen

Konzeptkarten sind nützlich, um Ideen, Orte, Charaktere und erzählerische Beziehungen miteinander zu verknüpfen. Sie werden auf ihrer eigenen Unterseite erklärt.

### Metadaten

Wenn die Anzeige von Metadaten in den Einstellungen aktiviert ist, erscheint außerdem ein technisches Panel mit:

- der Abenteuer-ID
- dem Erstellungsdatum
- dem Datum der letzten Änderung

Dieser Bereich ist vor allem für Kontrolle, Diagnose oder fortgeschrittene Verwaltung nützlich.

## Beziehung zu den Unterseiten

Die Seite **Abenteuer** ist eine allgemeine Übersicht. Von hier aus gehen die Unterseiten tiefer auf die einzelnen operativen Werkzeuge ein.

Die Unterseiten dieses Handbuchs werden sein:

- **Orte und Quests**
- **Konzeptkarten**
- **Bilder**
- **Karten**
- **Interaktive Karten**
- **Live-Sitzung**
- **Charaktere**

In der Praxis:

- diese Seite erklärt, **wie ein Abenteuer entsteht und aufgebaut ist** und wie das Abenteuer-Dashboard strukturiert ist
- die Unterseiten erklären, **wie jeder interne Bereich tatsächlich benutzt wird**

## Wann du diesen Bereich verwenden solltest

Der Bereich Abenteuer ist genau richtig, wenn du:

- eine neue Kampagne anlegen möchtest
- Cover, Status und Beschreibung des Abenteuers festlegen willst
- die Arbeit an einer bestehenden Kampagne wieder aufnehmen möchtest
- das Haupt-Dashboard öffnen willst
- eine Live-Sitzung starten möchtest
- schnell zu Orten, Charakteren, Sitzungen, Bildern und Karten der Kampagne gelangen möchtest
