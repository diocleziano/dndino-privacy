# Interaktive Karten

**Interaktive Karten** dienen dazu, die Orte eines Abenteuers visuell auf einer echten Kartenabbildung zu navigieren, mithilfe klickbarer Marker, die mit Ortsdatensätzen verknüpft sind.

Sie sind für Fälle gedacht, in denen die einfache Baumstruktur nicht mehr ausreicht und du dich natürlicher durch den Raum der Kampagne bewegen willst, zum Beispiel auf:

- einer Stadt
- einer Burg
- einem Viertel
- einem Dungeon
- einer Region

## Wofür sie gedacht sind

Interaktive Karten sind nützlich, wenn du:

- eine Karte als Hauptoberfläche für Navigation verwenden willst
- Orte durch Klick auf visuelle Marker öffnen willst
- der Kampagne eine klarere räumliche Struktur geben willst
- von einer Detailkarte zu einer größeren Karte wechseln willst

Sie ersetzen weder **Orte** noch **Beziehungsdiagramme**:

- **Orte** bleiben die eigentlichen Datensätze der Kampagne
- **Beziehungsdiagramme** dienen dazu, logische und erzählerische Beziehungen darzustellen
- **Interaktive Karten** dienen stattdessen dazu, reale Orte auf einem Kartenbild zu navigieren

## Woher sie kommen

Interaktive Karten sind kein eigener Datensatztyp aus einem separaten Modul. Sie entstehen aus **Kartenbildern**, die mit Orten verknüpft sind.

Praktisch heißt das:

1. du verknüpfst einem Ort ein oder mehrere Bilder vom Typ `Karte`
2. du wählst aus, welche davon als Standard-Interaktive-Karte verwendet werden soll
3. auf dieser Karte fügst du Marker hinzu, die mit Orten verknüpft sind

## Wo sie verwendet werden

Interaktive Karten leben im Bereich **Orte und Quests**.

Sie können auf zwei Arten genutzt werden:

- als **integrierter interaktiver Modus** im Orte-Dashboard
- als **großes Kartenpanel**, das über `Medien` geöffnet wird

## Unterschied zwischen integriertem Modus und großem Panel

### Integrierter interaktiver Modus

Wenn das Abenteuer über Karten verfügt, kannst du im Orte-Dashboard von der normalen Ansicht in die Ansicht `Interaktiv` wechseln.

In diesem Modus:

- zeigt die linke Bildschirmseite die Karte statt des klassischen Ortsbaums
- zeigt das rechte Panel weiterhin die Details des ausgewählten Ortes
- navigierst du durch Orte, indem du Marker anklickst

### Großes Kartenpanel

Über das Panel `Medien` eines Ortes kannst du eine interaktive Karte auch in einem größeren, dedizierten Panel öffnen.

Dieser Modus ist besonders nützlich, wenn du:

- Marker bearbeiten willst
- Verknüpfungen korrigieren willst
- präziser auf der Karte arbeiten willst

## Wie eine interaktive Karte vorbereitet wird

Der richtige Ablauf ist:

1. öffne den Ort, dem die Karte gehören soll
2. gehe in den Bereich `Medien`
3. füge ein oder mehrere Bilder vom Typ `Karte` hinzu
4. wähle aus, welche davon die Standard-Interaktive-Karte werden soll
5. öffne die interaktive Karte
6. erstelle Marker und verknüpfe sie mit Orten

## Wie die Standardkarte gewählt wird

Ein Ort kann mehrere verknüpfte Karten haben. Eine davon kann als Standard-Interaktive-Karte markiert werden.

Wenn DnDino entscheiden muss, welche Karte für einen Ort angezeigt werden soll, gilt folgende Logik:

- wenn der Ort eine ausdrücklich gewählte interaktive Karte hat, wird diese verwendet
- andernfalls wird die erste verfügbare Karte des Ortes verwendet
- wenn der Ort keine eigenen Karten hat, kann eine Karte eines übergeordneten Ortes verwendet werden

## Beziehung zwischen Ort und Karte

Jede interaktive Karte gehört zu einem Ort.

Der Ort, dem die Karte gehört, ist nicht zwingend der einzige Ort, der von dieser Karte geöffnet werden kann: Marker können auf jeden Ort in der Abenteuerstruktur verweisen.

## Wie man in den interaktiven Modus wechselt

Im Dashboard `Orte` kannst du, sobald Karten vorhanden sind, in die Ansicht `Interaktiv` wechseln.

In diesem Modus findest du:

- Kopfbereich der interaktiven Karte
- `Karten`-Auswahl
- gegebenenfalls die Schaltfläche `Zurück`
- gegebenenfalls die Schaltfläche `Höhere Ebene`
- Umschalter `Markernamen anzeigen`
- Zoom-Steuerung
- den Karten-Canvas

## Kartenauswahl

Über das Menü `Karte` kannst du auswählen, welche Karte aus den verfügbaren Karten des Abenteuers angezeigt werden soll.

## Navigation zwischen Karten

Der interaktive Modus unterstützt zwei Arten der Kartennavigation.

### Zurück

Die Schaltfläche `Zurück` bringt dich zur zuvor angezeigten Karte zurück.

### Höhere Ebene

Wenn der aktuelle Ort einen übergeordneten Ort mit interaktiver Karte hat, kann die Schaltfläche `Höhere Ebene` erscheinen.

Sie erlaubt dir, zu einer größeren Karte zurückzukehren.

## Der Karten-Canvas

Der Canvas ist die zentrale Fläche, auf der die eigentliche Karte angezeigt wird.

Hier kannst du:

- die Karte sehen
- Marker sehen
- Marker anklicken oder doppelklicken
- Zoom und Pan verwenden

## Zoom und Bewegung

Interaktive Karten unterstützen:

- Hinein- und Herauszoomen
- Zurücksetzen des Zooms
- horizontales und vertikales Scrollen
- Panning durch Ziehen der Karte
- Pinch-Geste
- Zoom per Mausrad, wenn sich der Cursor über der Karte befindet

## Markernamen anzeigen

Mit dem Umschalter `Markernamen anzeigen` kannst du festlegen, ob Markernamen direkt auf der Karte sichtbar sein sollen.

Wenn aktiviert:

- kann jeder Marker seinen eigenen Titel oder, wenn dieser leer ist, den Namen des verknüpften Ortes anzeigen

Wenn deaktiviert:

- bleiben nur die Marker-Symbole sichtbar

## Wie Marker funktionieren

Ein Marker enthält:

- normalisierte Position auf der Karte
- optionalen Titel
- optionale Verknüpfung zu einem Ort

Der Marker wird relativ zu den Kartenkoordinaten gespeichert und bleibt deshalb auch bei geändertem Zoom an der richtigen Stelle.

Marker ändern außerdem ihre Farbe je nach Status des verknüpften Ortes, damit der Fortschritt der Erkundung auf der Karte schneller auf einen Blick erkennbar ist:

- eine Farbe für `Unbesuchte` Orte
- eine Farbe für Orte `Im Besuch`
- eine Farbe für `Besuchte` Orte

Diese Farben sind fest und ändern sich nicht mit dem aktiven Thema, damit ihre Bedeutung in der ganzen App konsistent bleibt.

## Verhalten von Markern im Lesemodus

Wenn du nicht im Bearbeitungsmodus bist:

- wählt ein **einfacher Klick** einen Marker aus
- öffnet ein **Doppelklick** den verknüpften Ort

Im integrierten interaktiven Modus bedeutet das Öffnen eines Ortes, dass das rechte Panel sofort aktualisiert wird.

Im großen Kartenpanel schließt das Öffnen eines Ortes das Kartenpanel und legt den Fokus im Dashboard wieder auf den ausgewählten Ort.

## Wie ein Marker erstellt wird

So erstellst du im großen Kartenpanel einen Marker:

1. öffne die interaktive Karte über `Medien`
2. drücke `Bearbeiten`
3. drücke `Neuer Marker`
4. wähle den zu verknüpfenden Ort aus
5. klicke auf einen Punkt der Karte

## Bearbeitungsmodus

Im großen Panel gibt es einen echten Bearbeitungszustand.

Wenn du `Bearbeiten` drückst:

- wechselt die Karte in den Bearbeitungsmodus
- kannst du neue Marker erstellen
- kannst du bestehende Marker auswählen und bearbeiten
- kannst du Marker ziehen, um sie neu zu positionieren

Wenn du `Sperren` drückst, verlässt du den Bearbeitungsmodus.

## Neuer Marker

Wenn du `Neuer Marker` aktivierst:

- bittet DnDino dich zuerst, den zu verknüpfenden Ort auszuwählen
- danach wirst du aufgefordert, auf die Karte zu klicken, um den Marker zu platzieren

## Auswahl des verknüpften Ortes

Wenn du einen Marker erstellst oder bearbeitest, zeigt der Inspector rechts die Ortsauswahl.

Von dort aus kannst du:

- nach Namen suchen
- Orte in hierarchischer Struktur sehen
- den Marker dem richtigen Ort zuweisen

## Einen bestehenden Marker bearbeiten

Wenn ein Marker im Bearbeitungsmodus ausgewählt ist, kannst du im Inspector ändern:

- `Markertitel`
- `Verknüpfter Ort`

Wenn der Titel leer bleibt, verwendet DnDino ersatzweise den Namen des verknüpften Ortes oder einen allgemeinen Titel.

## Einen Marker verschieben

Im Bearbeitungsmodus kannst du einen Marker an einen neuen Punkt der Karte ziehen.

Am Ende der Bewegung speichert DnDino:

- neue X-Position
- neue Y-Position

## Einen Marker löschen

Ebenfalls im Inspector kannst du, wenn ein Marker ausgewählt ist, Folgendes verwenden:

- `Marker löschen`

## Der Karten-Inspector

Das Seitenpanel der großen Karte verändert sich je nach aktuellem Zustand.

### Im Lesemodus

Wenn du nicht bearbeitest, zeigt der Inspector einfach die Liste der vorhandenen Marker.

### Während der Erstellung eines Markers

Wenn `Neuer Marker` aktiv ist, zeigt der Inspector:

- Hinweise
- Suchfeld
- Liste auswählbarer Orte

### Während der Bearbeitung eines Markers

Wenn du einen bestehenden Marker ausgewählt hast, zeigt der Inspector:

- Titelfeld
- Auswahl des verknüpften Ortes
- Zusammenfassung des aktuellen Ortes
- Schaltfläche zum Löschen des Markers

## Markerliste

Auch die Markerliste im Inspector kann zur Navigation verwendet werden.

Jede Zeile zeigt:

- Markertitel
- verknüpften Ort, falls vorhanden

Im Lesemodus kannst du durch Klick auf eine Zeile den verknüpften Ort öffnen.

## Verhalten der Karte im integrierten Modus

Wenn du den Modus `Interaktiv` direkt im Orte-Dashboard verwendest:

- folgt die Karte dem ausgewählten Ort
- versucht DnDino, die passendste Karte für diesen Ort zu zeigen
- kann, wenn der Ort keine eigene Karte hat, eine Karte einer höheren Ebene verwendet werden

## Vererbung einer Karte vom übergeordneten Ort

Ein sehr nützlicher Teil des Systems ist, dass ein Ort auch eine Karte einer höheren Ebene verwenden kann.

Das erlaubt Szenarien wie:

- ein Viertel nutzt die Stadtkarte
- ein Raum nutzt die Burgkarte
- ein interessanter Ort nutzt die Regionskarte

## Wie man eine interaktive Karte aus Medien öffnet

Im Panel `Medien` eines Ortes können Karten vom Typ `Karte` die Aktion anzeigen:

- `Interaktive Karte öffnen`

## Wann der integrierte Modus sinnvoll ist

Der integrierte interaktive Modus ist sinnvoll, wenn du:

- schnell zwischen Orten navigieren willst
- mit Karte und Orts-Panel nebeneinander arbeiten willst
- die Karte als Alternative zum klassischen Baum nutzen willst

## Wann das große Panel sinnvoll ist

Das große Panel ist sinnvoll, wenn du:

- Marker erstellen willst
- Marker verschieben willst
- Verknüpfungen ändern willst
- präziser arbeiten willst

## In der Praxis

Interaktive Karten sind das richtige Werkzeug, wenn du Orten eine echte räumliche Dimension geben willst.

Die Grundidee ist einfach:

- der **Ort** bleibt der Hauptdatensatz
- die **Karte** wird zur visuellen Oberfläche
- der **Marker** ist die operative Verbindung zwischen Bild und Inhalt
