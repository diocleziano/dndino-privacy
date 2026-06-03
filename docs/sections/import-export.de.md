# Import und Export

DnDino kann Inhalte exportieren und importieren, um sie zwischen Installationen zu verschieben, Arbeitskopien zu erstellen oder Material mit anderen Dungeon Mastern zu teilen.

Importe überschreiben vorhandene Daten nicht automatisch: Vor dem Speichern kannst du prüfen, was hinzugefügt, ersetzt oder übersprungen wird.

## Zauber

Zauber können als JSON-Datei exportiert werden.

Beim Import trennt DnDino:

- neue Zauber
- Zauber mit gleichem Namen, die bereits in der Datenbank vorhanden sind

Für jeden Zauber kannst du entscheiden, ob du ihn:

- als neuen Eintrag importierst
- einen vorhandenen Eintrag ersetzt
- überspringst

Wenn bereits ein Zauber mit gleichem Namen existiert, zeigt die Prüfansicht einen Vergleich zwischen vorhandenem und importiertem Eintrag. So kannst du Stufe, Schule, Quellenbuch, Klassen, Zauberzeit und Dauer kontrollieren, bevor du entscheidest.

Für Konflikte gibt es auch Sammelaktionen, zum Beispiel alle vorhandenen Zauber überspringen oder alle als neue Einträge importieren.

## Charaktere

Charaktere werden als ZIP-Paket exportiert. Es kann enthalten:

- Charakterbogen
- verknüpfte Bilder
- Zauber-Verknüpfungen
- Daten, um den Eintrag in einer anderen Installation wiederherzustellen

Beim Import werden Charaktere mit gleichem Namen nicht automatisch ersetzt. Du kannst sie als neue Einträge importieren, einen vorhandenen Eintrag ersetzen oder sie überspringen.

Wenn der importierte Charakter verknüpfte Zauber hat, versucht DnDino, sie anhand des Namens vorhandenen Zaubern zuzuordnen. Wenn mehrere passende Zauber gefunden werden, kannst du auswählen, welcher verwendet werden soll.

Wenn du Charaktere in eine bereits gefüllte Datenbank importierst, prüfe die Zauber-Verknüpfungen sorgfältig: Zwei Zauber können denselben Namen haben, aber aus unterschiedlichen Quellenbüchern oder Versionen stammen.

## Abenteuer

Abenteuer werden als ZIP-Paket mit den Daten exportiert, die zum Wiederaufbau des Abenteuers nötig sind.

Ein importiertes Abenteuer wird immer als **neues Abenteuer** erstellt. DnDino überschreibt kein vorhandenes Abenteuer, damit Orte, Charaktere oder Sitzungen einer aktiven Kampagne nicht verloren gehen.

Der empfohlene Ablauf ist schrittweise:

1. Zauber importieren oder verknüpfen
2. Charaktere importieren oder verknüpfen
3. Abenteuer importieren

In der Abenteuerprüfung trennt DnDino die Hauptbereiche:

- im Paket enthaltene Zauber
- im Paket enthaltene Charaktere
- Abenteuerstruktur

Für Zauber und Charaktere legst du fest, wie bereits vorhandene Einträge behandelt werden. Danach wird das Abenteuer importiert und die richtigen Charaktere werden mit Orten, Präsenzen und den weiteren Paketinhalten verknüpft.

## Ausrüstung, Talente und Glossar

Ausrüstung, Talente und Glossareinträge können ebenfalls getrennt exportiert und importiert werden.

Der Export erstellt eigene JSON-Dateien. Das ist nützlich, wenn du nur einen Teil deines Materials teilen möchtest, ohne ein ganzes Abenteuer zu exportieren.

Beim Import trennt DnDino neue Datensätze von Datensätzen, die bereits einen Treffer in der Datenbank haben. Für jeden Datensatz kannst du ihn als neu importieren, den vorhandenen ersetzen oder ihn überspringen.

Bei Ausrüstung nutzt der Abgleich Name und Kategorie, damit Waffen, Rüstungen, Werkzeuge und Ausrüstung getrennt bleiben. Bei Talenten wird auch der Talenttyp berücksichtigt. Beim Glossar ist der Name des Eintrags die wichtigste Referenz.

Wenn ein ähnlicher Datensatz bereits existiert, zeigt die Prüfansicht den Vergleich zwischen vorhandenem Inhalt und Import. Mit Sammelaktionen kannst du mehrere Datensätze auf einmal überspringen, importieren oder ersetzen, wenn die Datei viele Elemente enthält.

## Prüfungen vor dem Import

Vor dem Import von Paketen mit Bildern prüft DnDino, ob die Datei lesbar ist und ob genug freier Speicher vorhanden ist, um Medien in den App-Container zu kopieren.

Ist die Datei beschädigt, unvollständig oder inkompatibel, wird der Import mit einer Fehlermeldung abgebrochen, statt Teildaten zu erzeugen.

## Gute Praxis

Vor dem Import wichtiger Inhalte:

- erstelle ein Backup der App
- importiere zuerst Zauber, wenn viele Charaktere sie verwenden
- prüfe Einträge mit gleichem Namen, bevor du sie ersetzt
- nutze den Vergleich zwischen altem und neuem Eintrag, wenn du unsicher bist
- importiere Abenteuer als neu und prüfe danach Verknüpfungen, Orte und Bilder

Der Import ist darauf ausgelegt, deine Datenbank zu schützen: Wähle im Zweifel `Als neu importieren` oder `Überspringen`, statt zu ersetzen.
