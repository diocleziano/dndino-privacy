# Helden, NSC und Monster

Der Bereich **Helden, NSC und Monster** sammelt alle Basisdatenblätter der Charaktere in der App. Hier erstellst, bearbeitest und klonst du die Datensätze, die später mit Abenteuern, Orten und Kämpfen verknüpft werden können.

Diese Seite ist wichtig, weil DnDino mit **mehreren Charakterebenen** arbeitet, die jeweils einen anderen Zweck haben:

- das **Basisblatt**
- den **Abenteuer-Charakter**
- die **Präsenz am Ort**
- den **Kampfteilnehmer**

Das sind keine sinnlosen Duplikate. Sie dienen dazu, **kontextbezogene Daten getrennt** zu halten, etwa angezeigten Namen, Trefferpunkte, Zustände, Initiative und SL-Notizen, ohne die Verbindung zum ursprünglichen Quelldatensatz zu verlieren.

## Basisblatt

Das **Basisblatt** ist der Hauptdatensatz im Bereich `Helden, NSC und Monster`.

Hier definierst du alles, was grundsätzlich zu diesem Charakter gehört:

- Name
- Typ: `Held`, `NSC` oder `Monster`
- Abstammung, Klasse, Größe, Gesinnung
- Attributswerte
- RK, maximale Trefferpunkte, Geschwindigkeit, Initiative
- Beschreibung, Fähigkeiten, Angriffe
- verknüpfte Bilder
- verknüpfte Zauber
- Ausrüstung und andere Referenzdaten

Das Basisblatt bedeutet nicht automatisch, dass der Charakter bereits in einem Abenteuer, an einem Ort oder in einem Kampf „anwesend“ ist. Es ist das Modell, von dem die weiteren Ebenen abgeleitet werden.

## Charakter erstellen, bearbeiten und klonen

Um einen neuen Datensatz anzulegen:

1. öffne `Helden, NSC und Monster`
2. drücke den Hinzufügen-Button
3. fülle das Charakterformular aus
4. speichere den Datensatz

Du kannst anlegen:

- Helden
- NSC
- Monster

Der gewählte Typ beeinflusst Felder und Verhalten in späteren Bereichen. Zum Beispiel:

- bei **Helden** spielen Kampagnenpräsenz, Inspiration und kontextbezogener Status eine größere Rolle
- bei **Monstern** werden HG, Angriffe und mehrfacher praktischer Einsatz wichtiger

Wenn du ein bestehendes Blatt öffnest, kannst du den Basisdatensatz vollständig bearbeiten. Änderungen hier aktualisieren den Quelldatensatz, überschreiben aber nicht immer automatisch alle kontextbezogenen Datensätze, die bereits in Abenteuern, Orten oder Kämpfen existieren. Das ist gewollt.

Beim **Klonen** wird aus einem bestehenden Blatt ein neues Basisblatt erzeugt. Dabei werden auch verknüpfte Elemente kopiert, zum Beispiel:

- Blattfelder
- verknüpfte Zauber
- strukturierte Angriffe
- verknüpfte Bilder

Das ist besonders nützlich, wenn du:

- ähnliche Varianten desselben Monsters erstellen willst
- von einem bereits vorbereiteten NSC ausgehen möchtest
- schnell mehrere Datensätze mit ähnlicher Struktur aufbauen willst

## Interne Links in Charaktertexten

Eine der nützlichsten Funktionen des Basisblatts, besonders für **NSC** und **Monster**, ist das System der **internen Links** in Rich-Text-Feldern.

Gerade im Bereich **Angriffe** ist das besonders wertvoll, weil es beschreibenden Text in operative Werkzeuge verwandelt, die du direkt während der Sitzung und im Kampf verwenden kannst.

Praktisch kannst du Links einfügen, die direkt öffnen:

- einen Würfelwurf
- einen Angriffswurf
- einen vollständigen Angriff mit Schaden
- einen Charakter
- einen Ort
- einen Zauber
- ein Talent
- eine Regel aus dem Glossar

## Wo sie besonders sinnvoll sind

Interne Links sind vor allem in Rich-Text-Feldern des Blatts nützlich, zum Beispiel:

- `Angriffe`
- `Besondere Fähigkeiten`
- `Beschreibung`
- andere beschreibende Felder mit schnellen Verweisen

Der nützlichste Fall bleibt jedoch **Angriffe**, weil du damit sofort klickbar machen kannst:

- den Angriffswurf
- die Schadenswürfel
- einen vollständig vorbereiteten Angriff

Gerade bei Monstern spart das Zeit, weil du Formeln nicht ständig neu lesen oder Würfe von Hand rekonstruieren musst.

## Wie man einen Link einfügt

Der richtige Ablauf ist:

1. öffne ein Rich-Text-Feld des Blatts
2. markiere den Text, der zum Link werden soll, oder setze den Cursor an die gewünschte Stelle
3. drücke den Button `Link`
4. wähle im Picker die passende Link-Art
5. bestätige die Erstellung

Je nach markiertem Text kann der Picker bereits einige automatische Vorschläge anzeigen.

## Die vier wichtigsten Wurflinks

### Freier Wurf

`Freier Wurf` ist der flexibelste Link. Er ist im Picker immer verfügbar und eignet sich, wenn du einen konfigurierbaren Wurf ohne starres Format anlegen willst.

Nützlich ist er für:

- eine vollständige Formel wie `1d6+3`
- einen einzelnen Würfel wie `1d20`
- eine Formel, die du vor dem Wurf noch spontan ändern willst

### Würfel werfen

`Würfel werfen` erscheint nur, wenn der markierte Text eine **gültige Würfelformel** ist.

Gültige Beispiele:

- `1d6`
- `2d8+4`
- `4d4 + 1`

Dieser Link ist ideal für einzelne Schadenwürfe, Heilwürfel, Zufallseffekte und schnelle getrennte Würfe.

### Angriffswurf

`Angriffswurf` erscheint nur, wenn der markierte Text ein **gültiger Modifikator** ist und keine vollständige `1d20`-Formel.

Gültige Beispiele:

- `+5`
- `-1`
- `0`
- `2`

Wenn du diesen Link erstellst, weiß DnDino, dass ein **1d20** mit diesem Modifikator geworfen werden soll. Das passt perfekt zu lesbaren Angriffszeilen wie:

- `Biss +6`
- `Klauen +4`

### Angriffswurf und Schaden

`Angriffswurf und Schaden` ist der leistungsstärkste Link für den Bereich **Angriffe**.

Er ist im Picker immer verfügbar und öffnet einen speziellen Konfigurator, in dem du festlegen kannst:

- Modifikator auf den Angriffswurf
- gegebenenfalls kritische Schwelle
- bis zu drei Schadensformeln
- Bezeichnungen für die einzelnen Schadensanteile

Das ist die beste Methode, um einen vollständigen Monster- oder NSC-Angriff vorzubereiten, weil ein einziger Link enthalten kann:

- den Angriffswurf
- Hauptschaden
- Nebenschaden
- zusätzlichen Schaden

Im Kampf ist dieser Link besonders nützlich, weil das zugehörige Popover den Schaden auch direkt auf ausgewählte Ziele anwenden kann.

## Praktisches Beispiel für Angriffe

Eine sehr effektive Art, einen Monsterangriff zu schreiben, ist, den Text für den Spielleiter gut lesbar zu halten und nur die wirklich nützlichen Stellen klickbar zu machen.

Zum Beispiel:

- `Biss +6, Reichweite 1,5 m, ein Ziel. Treffer: 1d8+4 Stichschaden.`

Dann kannst du:

- `+6` in `Angriffswurf`
- `1d8+4` in `Würfel werfen`

umwandeln oder direkt einen einzigen Link `Angriffswurf und Schaden` auf den Namen des Angriffs oder einen Teil der Zeile legen.

## Orte, Charaktere und andere Referenzen verknüpfen

Das Link-System dient nicht nur für Würfe.

In beschreibenden Feldern kannst du auch Verknüpfungen zu anderem App-Inhalt anlegen, etwa zu:

- einem `Ort`
- einem anderen `Charakter`
- einem `Zauber`
- einem `Talent`
- einer `Regel`

Wenn du `Link` drückst, versucht der Picker außerdem, den markierten Text als Anfangsfilter zu verwenden:

- findet er eine echte Übereinstimmung in den Namen von Datensätzen, öffnet er bereits gefiltert
- findet er keine echten Treffer, wird der Anfangsfilter geleert und du siehst die vollständige Liste

## Abenteuer-Charaktere

Der **Abenteuer-Charakter** ist die Ebene, die ein Basisblatt mit einer bestimmten Kampagne verbindet.

Dieser Datensatz verwaltet Werte, die **nur innerhalb eines Abenteuers** sinnvoll sind, zum Beispiel:

- aktuelle Trefferpunkte
- temporäre Trefferpunkte
- Zustände
- Status
- heroische Inspiration

Anders gesagt:

- das Basisblatt sagt, **wer** der Charakter ist
- der Abenteuer-Charakter sagt, **wie es ihm in dieser Kampagne gerade geht**

## Präsenzen an Orten

Die **Präsenz am Ort** ist wiederum ein eigener Datensatz. Er sagt aus, dass ein Charakter oder eine Kreatur an einem bestimmten Ort anwesend ist, gegebenenfalls mit lokalem Namen und lokalem Status.

Im Formular `Präsenz zum Ort hinzufügen` gibt es zwei mögliche Ursprünge:

- `Abenteuer-Charakter`
- `NSC / Monster`

### Präsenz aus Abenteuer-Charakter

Wenn du `Abenteuer-Charakter` wählst, wird der Ortsdatensatz mit einem Charakter verbunden, der bereits in der Kampagne vorhanden ist.

Dann gilt:

- die Präsenz bleibt mit dem Abenteuer-Charakter verbunden
- es wird keine autonome Kopie des Charakters angelegt
- derselbe Abenteuer-Charakter kann nicht mehr als einmal am selben Ort hinzugefügt werden

### Präsenz aus NSC / Monster

Wenn du `NSC / Monster` wählst, erzeugt der Ort stattdessen eine **lokal geklonte Präsenz** aus einem Basisblatt vom Typ `NSC` oder `Monster`.

Dieser Datensatz besitzt eigene ortsspezifische Werte wie:

- angezeigter Name
- aktuelle TP
- temporäre TP
- Zustände
- Status
- Gesinnung/Rolle im Kontext
- SL-Notizen

Das Verhalten hängt dann vom Typ ab:

- **Monster** dürfen mehrfach lokal am selben Ort vorkommen
- **NSC** bleiben am selben Ort einzigartig und werden dort im Picker nicht mehrfach angeboten

Wenn du mehrere Instanzen desselben Monsters hinzufügst, schlägt DnDino automatisch einen fortlaufenden Namen vor, zum Beispiel:

- `Goblin 2`

## Warum es den angezeigten Namen gibt

Sowohl Präsenzen an Orten als auch Kampfteilnehmer besitzen ein Feld `Angezeigter Name`.

Dieses Feld dient dazu, einen **kontextbezogenen Namen** zu behalten, ohne das Basisblatt umzubenennen. Das ist zum Beispiel nützlich, wenn du:

- ähnliche Kopien derselben Kreatur unterscheiden willst
- einem NSC nur an einem bestimmten Ort einen besonderen Namen geben willst
- im Kampf einen anderen Namen verwenden willst, ohne den Quelldatensatz zu ändern

## Kampfteilnehmer

Der **Kampfteilnehmer** ist die operative Ebene, die im Gefecht verwendet wird.

Ein Teilnehmer kann aus drei verschiedenen Quellen stammen:

- einem **Abenteuer-Charakter**
- einer **Ortspräsenz**
- einem **Basisblatt**

Jeder Kampfteilnehmer besitzt seinen eigenen kampfspezifischen Datensatz mit Werten wie:

- angezeigter Name
- Initiative
- RK
- max. TP
- aktuelle TP
- temporäre TP
- Zustände
- Status
- Todesrettungswürfe
- Reihenfolge in der Runde

### Teilnehmer aus Abenteuer-Charakteren

Wenn der Teilnehmer aus einem Abenteuer-Charakter stammt:

- bleibt er mit dem Kampagnencharakter verbunden
- werden die Endwerte nach dem Kampf wieder auf den Abenteuer-Datensatz zurückgeschrieben

### Teilnehmer aus Ortspräsenzen

Wenn der Teilnehmer aus einer Ortspräsenz stammt:

- bleibt er mit diesem Ortsdatensatz verknüpft
- kann der Kampf HP, Zustände und Status auf diesen Ortsdatensatz zurückschreiben, falls die Präsenz lokalen Status verwendet

### Teilnehmer aus Basisblättern

Wenn der Teilnehmer direkt aus einem Basisblatt stammt:

- verwendet der Kampfeintrag dieses Blatt als Quelle
- hängt das Verhalten bei Mehrfachinstanzen vom Typ ab

Im Kampf-Picker gilt:

- ein Basisdatensatz vom Typ **Monster** kann mehrfach hinzugefügt werden
- ein Basisdatensatz vom Typ **NSC** oder **Held** wird im selben Kampf nicht mehrfach angeboten

## Synchronisierung zwischen den Ebenen

Einige Werte werden zwischen den Ebenen synchronisiert, aber nicht immer alles wird überschrieben.

### Vom Basisblatt in die Kontexte

Das Basisblatt liefert:

- Identität des Charakters
- Referenzwerte
- Zauber
- Angriffe
- Bilder

### Von Kontexten zurück in verknüpfte Datensätze

Die operativen Ebenen können dagegen situative Werte zurückschreiben, vor allem:

- TP
- Zustände
- Status
- einige lokale Notizen

Im Kampf können Endwerte zum Beispiel zurückfließen auf:

- den verknüpften Abenteuer-Charakter
- die verknüpfte Ortspräsenz, falls diese lokalen Status verwendet

## Praktischer Unterschied zwischen den Ebenen

Zum Merken kannst du die Logik so lesen:

- `Basisblatt`: das **allgemeine Modell** des Charakters
- `Abenteuer-Charakter`: der **Zustand des Charakters innerhalb der Kampagne**
- `Präsenz am Ort`: die **kontextbezogene Anwesenheit des Charakters an einem bestimmten Ort**
- `Kampfteilnehmer`: die **operative Version des Charakters im Gefecht**

## Wann welche Ebene sinnvoll ist

### Nutze das Basisblatt, wenn:

- du den Charakter erstellen musst
- du strukturelle Daten ändern willst
- du Bilder, Zauber oder Angriffe verknüpfen möchtest

### Nutze den Abenteuer-Charakter, wenn:

- du einen Helden mit der Kampagne verknüpfen willst
- du TP, Status, Zustände und Inspiration dauerhaft im Abenteuer nachverfolgen willst

### Nutze die Ortspräsenz, wenn:

- du einen Ort mit Charakteren oder Kreaturen bevölkern willst
- du NSC und Monstern kontextbezogene Namen geben willst
- du getrennte lokale Instanzen in einem Ort brauchst

### Nutze den Kampfteilnehmer, wenn:

- du ein Gefecht vorbereitest oder leitest
- du Initiative, TP und Kampfzustände brauchst
- der Kampf mit kontextbezogenen Datensätzen arbeiten soll, ohne direkt das Basisblatt zu verändern

## Kurz zusammengefasst

Der Bereich `Helden, NSC und Monster` ist nicht nur ein Archiv von Charakterblättern. Er ist die **Quellschicht**, aus der die gesamte kontextbezogene Charakterverwaltung innerhalb der App entsteht.

Die Grundlogik ist:

- das **Basisblatt** definiert den Charakter
- der **Abenteuer-Charakter** setzt ihn in die Kampagne
- die **Präsenz am Ort** verortet ihn in einem bestimmten Ort
- der **Kampfteilnehmer** macht ihn im Gefecht handlungsfähig

!!! tip
    Wenn du Verwirrung vermeiden willst, merke dir immer diesen Unterschied: Das Basisblatt beschreibt den Charakter, während Abenteuer, Ort und Kampf seinen Zustand in einem bestimmten Kontext beschreiben. Du musst dich nicht zu sehr an der theoretischen Trennung festbeißen; wichtig ist vor allem, dass einige Felder nur in ihrem jeweiligen Kontext existieren.
