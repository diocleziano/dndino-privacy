# FAQ

Dieser Bereich sammelt kurze Antworten auf die häufigsten Fragen zu DnDino.

Wenn Sie eine vollständige Erklärung zu einer bestimmten Ansicht brauchen, öffnen Sie danach am besten die passende Seite im Handbuch. Diese FAQ ist vor allem für die häufigsten Praxisfälle gedacht.

## Wie kehre ich sofort zu meiner letzten Kampagne zurück?

Öffnen Sie die `Startseite` und verwenden Sie die Karte der **letzten Abenteuerkampagne**.

Von dort aus können Sie:

- direkt das Abenteuer-Dashboard öffnen
- zum zuletzt besuchten Ort springen, falls vorhanden

Das ist der schnellste Weg, wieder einzusteigen, ohne jedes Mal durch die komplette Abenteuerliste zu gehen.

## Was ist der Unterschied zwischen Basisbogen, Abenteuercharakter, Ortspräsenz und Kampfteilnehmer?

Der **Basisbogen** ist der allgemeine Datensatz eines Charakters oder einer Kreatur.

Aus diesem Bogen kann DnDino getrennte kontextbezogene Datensätze ableiten:

- den **Abenteuercharakter**, der innerhalb einer Kampagne verwendet wird
- die **Ortspräsenz**, die an Orten verwendet wird
- den **Kampfteilnehmer**, der im Kampf verwendet wird

Dieses System trennt:

- kontextbezogene Namen
- Initiative
- aktuelle TP
- DM-Notizen
- lokalen Kampf- oder Ortszustand

Mit anderen Worten: Der Basisbogen bleibt die allgemeine Referenz, während die kontextbezogenen Datensätze die praktische Arbeit am Spieltisch erleichtern.

## Wie füge ich einen Helden zum Abenteuer hinzu?

Öffnen Sie das `Abenteuer-Dashboard` und gehen Sie dann in den Bereich `Charaktere`.

Dort können Sie:

- einen bestehenden Charakter hinzufügen
- mit `Charakter erstellen` einen neuen Charakter anlegen

Wenn Sie einen neuen Charakter direkt aus dem Auswahlfenster erstellen, gelangen Sie nach dem Speichern wieder dorthin zurück und die Liste wird sofort aktualisiert.

## Wie füge ich eine Präsenz zu einem Ort hinzu?

Öffnen Sie den Ort und wechseln Sie in den Bereich `Präsenzen`.

Dort können Sie hinzufügen:

- einen Helden, der bereits mit dem Abenteuer verknüpft ist
- einen `NSC`
- ein `Monster`

Beachten Sie diesen wichtigen Unterschied:

- ein `NSC` bleibt an diesem Ort eindeutig
- ein `Monster` kann mehrfach hinzugefügt werden

So können mehrere Instanzen desselben Monsters am gleichen Ort existieren, ohne dass NSCs versehentlich doppelt angelegt werden.

## Kann ich den Namen eines Monsters ändern, ohne den Basisbogen zu verändern?

Ja.

Genau dafür verwendet DnDino kontextbezogene Datensätze.

Sie können ein Monster umbenennen:

- im Vorkampf
- in Ortspräsenzen
- in anderen lokalen Kontexten, in denen ein besser lesbarer Einsatzname sinnvoll ist

Dadurch wird der Name im ursprünglichen Basisbogen nicht verändert.

## Wie verlinke ich schnell einen Charakter oder einen Ort in einer Beschreibung?

Verwenden Sie in Textfeldern mit internen Links den Befehl `Link`.

Darüber können Sie Verknüpfungen zu folgenden Einträgen erstellen:

- Charakteren
- Orten
- Zaubern
- Regeln
- Talenten

Das ist besonders nützlich:

- in `Orten`, um andere Orte oder Figuren aus der Beschreibung direkt zu verlinken
- in `Charakteren`, besonders bei `Angriffen`, um Würfe oder nützliche Verweise einzubauen

## Wozu dienen Links in Monster-Angriffen?

Sie machen aus einem beschreibenden Text ein praktisches Werkzeug.

In Rich-Text-Angriffsfeldern können Sie Links wie diese einfügen:

- `Voller Angriff`
- `Freier Wurf`
- `Würfeln`
- `Angriffswurf`

Dadurch können Sie:

- schnell würfeln
- Schaden auf Ziele anwenden
- auf andere App-Einträge verweisen

Das ist eine der effektivsten Möglichkeiten, einen Monsterbogen im Kampf wirklich nützlich zu machen.

## Muss ich die automatischen Kampfwürfe verwenden?

Nein.

DnDino bietet viele Automatisierungen, zwingt Sie aber nicht dazu.

Sie können weiterhin:

- physische Würfel am Tisch benutzen
- Ergebnisse klassisch ablesen
- Schaden manuell anwenden

Die App nimmt Ihnen vor allem die wiederkehrenden TP-Anpassungen und Kopfrechenarbeit ab.

## Funktioniert der Kampf auch mit nur einem Monitor gut?

Ja.

`Flat Combat` funktioniert auch auf einem einzelnen Bildschirm sehr gut.

Ein zweiter Bildschirm mit dem `Spielerfenster` ist für die Präsentation besonders praktisch, aber keine Voraussetzung. Auch auf nur einem Monitor können Sie den Kampf problemlos nutzen und in den Einstellungen festlegen, wie sich das Spielerfenster verhalten soll.

## Kann ich festlegen, wie viele Informationen die Spieler im Kampf sehen?

Ja.

Unter `Einstellungen > Kampf` können Sie unter anderem steuern, ob die Spieler Folgendes sehen:

- Rundennummer
- TP
- Zustände
- nächster Zug
- den echten Namen von Gegnern
- Details zu NSCs und Monstern

So können Sie entscheiden, ob der Kampf transparenter oder eher klassisch hinter dem DM-Schirm ablaufen soll.

## Wie funktioniert die Kampfzusammenfassung am Ende?

Am Ende des Kampfes schließt DnDino die Begegnung und synchronisiert die kontextbezogenen Daten zurück auf die verknüpften Datensätze.

Zusätzlich gilt:

- der DM sieht die Endzusammenfassung im Kampf selbst
- die Spieler können eine Zusammenfassung im `Spielerfenster` sehen, wenn die Option aktiv ist

Die öffentliche Zusammenfassung konzentriert sich auf die Spielercharaktere und nicht auf die Gegner.

## Was passiert, wenn ein Held unter 0 TP fällt?

Helden können in den negativen Bereich fallen.

Die von der App umgesetzte Regel lautet:

- zwischen `0` und `-(max. TP - 1)` ist der Held `Bewusstlos`
- bei `-max. TP` oder weniger stirbt der Held sofort

Während des Kampfes zeigt DnDino bei einem bewusstlosen Helden außerdem den Bereich für **Todesrettungswürfe** an.

## Wie zeige ich den Spielern ein Bild?

DnDino verwendet dafür ein eigenes Präsentationsfenster.

Sie können es nutzen:

- während des Kampfes
- für Abenteuerbilder
- in anderen Abläufen, die Präsentation unterstützen

Das Verhalten dieses Fensters wird unter `Einstellungen > Medien` und teilweise unter `Einstellungen > Kampf` festgelegt.

## Wie sichere ich meine Daten?

Gehen Sie zu `Einstellungen > Datenbank`.

Dort können Sie:

- sehen, wo die App-Daten gespeichert sind
- den Datenordner öffnen
- den Backup-Ordner öffnen
- manuell einen Snapshot erstellen
- einen Snapshot wiederherstellen
- aus iCloud wiederherstellen, falls eingerichtet

Im selben Bereich können Sie außerdem festlegen:

- die Häufigkeit automatischer Backups
- die maximale Anzahl gespeicherter Snapshots

## Wo finde ich technische Informationen zur Datenbank, wenn etwas nicht stimmt?

Gehen Sie zu `Einstellungen > Diagnose`.

Dort können Sie prüfen:

- den Pfad der Datenbank
- ob die Datei vorhanden ist
- ihre Größe
- das Datum der letzten Änderung
- die SQLite-Version
- gefundene Tabellen und Datensatzanzahlen

Das ist der richtige Bereich, wenn Sie herausfinden möchten, ob ein Problem nur optisch ist oder tatsächlich die gespeicherten Daten betrifft.

## Wie kontaktiere ich den Support?

Öffnen Sie `Einstellungen > Support`.

Dort können Sie:

- eine Support-Anfrage senden
- einen Vorschlag senden
- die Kontakt-E-Mail kopieren

Nutzen Sie `Support`, wenn etwas nicht funktioniert oder unklar ist. Nutzen Sie `Vorschlag`, wenn Sie eine Verbesserung oder eine neue Funktion anregen möchten.

!!! tip
    Wenn eine Antwort hier zu knapp wirkt, nutzen Sie die FAQ als Ausgangspunkt und öffnen Sie anschließend die passende Handbuchseite, etwa `Charaktere`, `Orte`, `Kampf` oder `Einstellungen`.
