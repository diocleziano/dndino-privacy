# Live-Session

Die **Live-Session** ist der operative Kontext der laufenden Spielsitzung. Sie ist nicht einfach nur ein Timer, sondern ein System, das Folgendes zusammenhält:

- die Spielzeit der Sitzung
- die Timeline wichtiger Ereignisse
- schnelle SL-Notizen
- den Status besuchter Orte
- aktive oder abgeschlossene Quests
- gespielte Kämpfe
- aggregierte Sitzungsstatistiken

Praktisch bedeutet das: Wenn eine Live-Session aktiv ist, weiß DnDino, welche Kampagne gerade läuft, und nutzt diesen Kontext, um verschiedene Teile der App miteinander zu verbinden.

## Wofür sie gedacht ist

Die Live-Session ist nützlich, wenn du DnDino während einer echten Spielsitzung am Tisch verwenden willst und nicht nur zur Vorbereitung.

Sie dient dazu:

- die Sitzungszeit zu verfolgen
- eine geordnete Timeline der wichtigsten Ereignisse zu führen
- SL-Informationen schnell zu notieren
- Orte als besucht oder in Besuch zu markieren
- eine dynamische Sitzungsübersicht zu sehen
- automatisch Daten aus dem Kampf zu sammeln

## Wo sie gestartet wird

Die Live-Session wird über das **Abenteuer-Dashboard** im Panel `Live-Session` gestartet.

Wenn keine Sitzung aktiv ist, zeigt das Panel:

- Status bereit
- Schaltfläche `Live-Session starten`

Wenn du diese Schaltfläche drückst, erstellt DnDino eine neue Live-Session und setzt sie als global aktive Sitzung.

## Nur eine Live-Session gleichzeitig

DnDino verwaltet immer nur eine aktive Live-Session gleichzeitig.

Wenn bereits in einem anderen Abenteuer eine Sitzung geöffnet ist:

- kann das aktuelle Abenteuer keine zweite starten
- zeigt das Dashboard einen Hinweis, dass die aktive Live-Session zu einer anderen Kampagne gehört

## Was passiert, wenn eine Live-Session aktiv ist

Wenn eine Live-Session läuft:

- zeigt die obere Leiste ihren Status
- aktualisiert sich der Timer weiter
- folgen Orte diesem Kontext
- beginnt die Timeline Ereignisse zu sammeln
- kann auch der Kampf Daten in die Session schicken

Die Live-Session wird dadurch zum roten Faden der laufenden Partie.

## Sitzungsstatus

Die Live-Session kann drei Zustände haben:

- aktiv
- pausiert
- unterbrochen

### Aktiv

Das ist der normale Zustand, solange die Sitzung läuft. Der Timer zählt weiter und Ereignisse werden mit der korrekten verstrichenen Zeit gespeichert.

### Pausiert

Die Sitzung kann über das Abenteuer-Dashboard oder die obere Leiste pausiert werden.

Wenn sie pausiert ist:

- stoppt der Timer
- bleibt die Sitzung trotzdem offen
- kann sie später fortgesetzt werden

### Unterbrochen

Wenn die App geschlossen wird, während die Sitzung noch aktiv ist, öffnet DnDino sie beim nächsten Start als `unterbrochen` wieder und protokolliert ein eigenes Ereignis in der Timeline.

Das macht es möglich:

- die Sitzung nicht zu verlieren
- zu erkennen, dass eine Unterbrechung stattgefunden hat
- die Arbeit manuell wieder aufzunehmen

## Das Live-Session-Panel im Abenteuer-Dashboard

Im Abenteuer-Dashboard zeigt das Panel den aktuellen Sitzungsstatus.

Wenn die Sitzung zum geöffneten Abenteuer gehört, zeigt das Panel:

- Sitzungstitel
- Echtzeit-Timer
- Status (`Läuft` oder `Pausiert`)
- Hinweis, dass der Player global ist
- Schaltflächen:
  - `Pause` oder `Fortsetzen`
  - `Schließen und speichern`

Wenn keine Live-Session aktiv ist:

- erscheint die Schaltfläche `Live-Session starten`

Wenn eine Sitzung aktiv ist, aber zu einem anderen Abenteuer gehört:

- zeigt das Panel, dass die Live-Session derzeit anderswo belegt ist

## Die Live-Session in der Topbar

Wenn eine Live-Session aktiv ist, zeigt die obere Leiste der App einen eigenen Indikator an.

Dieses Element enthält:

- Sitzungstitel
- Timer
- Statusanzeige

Ein Klick darauf öffnet ein Popover zur Schnellsteuerung.

## Das Live-Session-Popover in der Topbar

Über das Popover in der Topbar kannst du sehr schnelle Aktionen ausführen, ohne den aktuellen Bildschirm zu verlassen.

Dort findest du:

- `Pause` oder `Fortsetzen`
- `Schließen und speichern`
- Schnelleditor für `SL-Notiz`
- die Sitzungstimeline
- Schnellaktionen für den aktuell besuchten Ort
- kompakte Live-Zusammenfassung

## Schnelle SL-Notiz

Im Popover der Live-Session kannst du eine **SL-Notiz** schreiben und sofort zur Timeline hinzufügen.

Das ist nützlich, um schnell festzuhalten:

- Entscheidungen der Spielenden
- erzählerische Ideen
- Konsequenzen, an die du dich erinnern willst
- improvisierte Einfälle, die während der Sitzung entstanden sind

SL-Notizen werden als Timeline-Ereignisse gespeichert.

## Sitzungstimeline

Die Timeline ist das chronologische Protokoll der Live-Session.

Jedes Ereignis speichert:

- Titel
- Detail
- den Zeitpunkt innerhalb der Sitzung

Die Timeline kann sowohl Systemereignisse als auch SL-Notizen enthalten.

## Typen aufgezeichneter Ereignisse

Zu den wichtigsten Ereignissen, die DnDino automatisch protokolliert, gehören:

- `Session gestartet`
- `Session pausiert`
- `Session fortgesetzt`
- `Session durch Schließen der App unterbrochen`
- `Ort betreten`
- `Ort verlassen`
- `Ortsstatus aktualisiert`
- `Quest aktiviert`
- `Quest abgeschlossen`
- `Kampf begonnen`
- `Kampf beendet`
- `Im Kampf verursachter Schaden`
- `Im Kampf erlittener Schaden`
- `SL-Notiz`

## Verbindung mit Orten

Die Live-Session ist direkt mit den Orten des aktiven Abenteuers verbunden.

Wenn du im Kontext der Sitzung einen Ort aktualisierst:

- wird die Statusänderung protokolliert
- aktualisiert sich die Timeline
- ändert sich die Live-Zusammenfassung entsprechend

Die wichtigsten ortsbezogenen Werte sind:

- Orte in Besuch
- besuchte Orte
- aktive Quests
- abgeschlossene Quests

## Automatisches Schließen des zuvor besuchten Ortes

In den Einstellungen gibt es außerdem eine Logik, die an die Live-Session gekoppelt ist: Wenn ein Ort auf `In Besuch` gesetzt wird, kann der zuvor in Besuch befindliche Ort automatisch als `Besucht` markiert werden.

Diese Funktion gilt nur, wenn eine aktive Live-Session existiert, und ist sehr nützlich, um das Erkundungstracking konsistent zu halten.

## Live-Zusammenfassung

Die Live-Zusammenfassung aggregiert die wichtigsten Daten, die während der Sitzung gesammelt wurden.

Zu den wichtigsten Werten gehören:

- besuchte Orte
- Orte in Besuch
- aktive Quests
- abgeschlossene Quests
- gespielte Kämpfe
- besiegte Feinde
- gefallene Helden
- gesamte Kampfdauer

Die Live-Session hält außerdem zwei sehr nützliche Übersichten für Charaktere fest:

- von Helden verursachter Schaden
- von Helden erlittener Schaden

## Integration mit dem Kampf

Die Live-Session und der Kampf sind eng miteinander verbunden.

Wenn du während einer Live-Session einen Kampf startest, protokolliert DnDino:

- `Kampf begonnen`

Während des Kampfes kann es protokollieren:

- `Im Kampf verursachter Schaden`
- `Im Kampf erlittener Schaden`

Wenn du den Kampf schließt, protokolliert es:

- `Kampf beendet`
- Dauer der Begegnung
- besiegte Feinde
- gefallene Helden

## Verursachter und erlittener Schaden

Die Live-Session verfolgt Schaden in zwei getrennten Ranglisten:

- `Von Charakteren verursachter Schaden`
- `Von Charakteren erlittener Schaden`

Diese Zählung ist nur für die Abenteuerhelden gedacht, nicht für alle Teilnehmenden eines Kampfes.

## Gefallene Helden

Wenn ein Kampf endet, kann die Live-Zusammenfassung auch den Zähler der **gefallenen Helden** erhöhen.

Dieser Wert wird direkt aus dem Endergebnis des Kampfes gespeist.

## Live-Session und Spielerfenster

Die Live-Session ist nicht dasselbe wie das **Spielerfenster**, aber beide Dinge sind miteinander verbunden.

Die Live-Session liefert den allgemeinen Kontext der Partie, während das Spielerfenster der Kanal für die visuelle Präsentation ist.

Insbesondere:

- während des Kampfes kann das Spielerfenster Intro, aktuellen Zug und Abschlusszusammenfassung zeigen
- außerhalb des Kampfes kann das Spielerfenster weiterhin genutzt werden, um Bilder und Inhalte des aktuell aktiven Kontexts zu zeigen

## Schließen und Speichern

Wenn du `Schließen und speichern` wählst, dann:

- finalisiert DnDino die Sitzung
- speichert die gesammelten Daten
- schreibt die Timeline in die mit dem Abenteuer verknüpfte Sitzung
- schließt den globalen Live-Kontext

Nach dem Schließen bleibt die Sitzung als gespeicherte Sitzung einsehbar.

## Anzeige einer gespeicherten Sitzung

Eine bereits beendete Live-Session kann wieder als Detailansicht geöffnet werden.

Im Detailpanel findest du:

- Zusammenfassung und Timeline
- aufgezeichnete Dauer
- besuchte Orte
- gespielte Kämpfe
- besiegte Feinde
- gefallene Helden
- Ranglisten zu verursachtem und erlittenem Schaden der Charaktere

## Wann die Live-Session besonders sinnvoll ist

Die Live-Session ist besonders nützlich, wenn du:

- DnDino während des Spiels offen halten willst
- schnell festhalten willst, was am Tisch tatsächlich passiert
- wissen willst, welche Orte besucht wurden
- eine geordnete Timeline der Schlüsselmomente haben willst
- Kampf automatisch in die Sitzungszusammenfassung einfließen lassen willst

## In der Praxis

Die Live-Session ist die Brücke zwischen:

- Vorbereitung
- operativer Spielleitung
- finaler Erinnerung an die Sitzung

Gut eingesetzt reduziert sie stark das Risiko, wichtige Informationen während des Spiels zu verlieren, und macht es sehr viel leichter, später nachzuvollziehen, was in der Kampagne tatsächlich passiert ist.
