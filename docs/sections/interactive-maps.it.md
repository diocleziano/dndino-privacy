# Mappe interattive

Le **mappe interattive** servono a navigare visivamente i luoghi dell’avventura su una vera mappa grafica, usando marker cliccabili collegati ai record dei luoghi.

Sono pensate per i casi in cui la semplice struttura ad albero non basta più e vuoi muoverti nello spazio della campagna in modo più naturale, per esempio su:

- una città
- un castello
- un quartiere
- un dungeon
- una regione

## A cosa servono

Le mappe interattive sono utili quando vuoi:

- usare una mappa come superficie principale di navigazione
- aprire i luoghi cliccando su marker visivi
- dare una struttura spaziale più chiara alla campagna
- passare da una mappa di dettaglio a una mappa più ampia

Non sostituiscono i **Luoghi** e non sostituiscono le **Mappe concettuali**:

- i **Luoghi** restano i record veri della campagna
- le **Mappe concettuali** servono a mostrare relazioni logiche e narrative
- le **Mappe interattive** servono invece a navigare luoghi reali sopra un’immagine di mappa

## Da dove nascono

Le mappe interattive non sono un tipo di record separato creato in un modulo a parte. Nascono a partire dalle **mappe immagine** collegate ai luoghi.

In pratica:

1. colleghi una o più immagini di tipo `Mappa` a un luogo
2. scegli quale mappa deve essere usata come mappa interattiva di default
3. su quella mappa aggiungi marker collegati ai luoghi

## Dove si usano

Le mappe interattive vivono nella sezione **Luoghi e Quest**.

Possono essere usate in due modi:

- come **modalità interattiva integrata** nella dashboard dei luoghi
- come **pannello mappa grande** aperto da `Media`

## Differenza tra modalità integrata e pannello grande

### Modalità interattiva integrata

Quando l’avventura ha mappe disponibili, nella dashboard luoghi puoi passare dalla vista normale alla vista `Interattiva`.

In questa modalità:

- la parte sinistra della schermata mostra la mappa al posto dell’albero classico dei luoghi
- il pannello di destra continua a mostrare il dettaglio del luogo selezionato
- cliccando i marker navighi direttamente nei luoghi

### Pannello mappa grande

Dal pannello `Media` di un luogo puoi anche aprire una mappa interattiva in un pannello dedicato più grande.

Questa modalità è utile quando vuoi:

- modificare i marker
- sistemare collegamenti
- lavorare con più precisione sulla mappa

## Come si prepara una mappa interattiva

Il flusso corretto è questo:

1. apri il luogo che deve possedere la mappa
2. vai nella sezione `Media`
3. aggiungi una o più immagini di tipo `Mappa`
4. scegli quale di queste deve diventare la mappa interattiva di default
5. apri la mappa interattiva
6. crea i marker e collegali ai luoghi

## Come si sceglie la mappa di default

Un luogo può avere più mappe collegate. Tra queste, una può essere marcata come mappa interattiva di riferimento.

Quando DnDino deve capire quale mappa mostrare per un luogo, usa questa logica:

- se il luogo ha una mappa selezionata esplicitamente come mappa interattiva, usa quella
- altrimenti usa la prima mappa disponibile del luogo
- se il luogo non ha mappe proprie, può usare la mappa di un luogo padre

## Relazione tra luogo e mappa

Ogni mappa interattiva appartiene a un luogo.

Il luogo proprietario della mappa non è per forza l’unico luogo apribile da quella mappa: i marker possono infatti collegare qualunque luogo della struttura dell’avventura.

## Come si entra nella modalità interattiva

Nella dashboard `Luoghi`, quando esistono mappe disponibili, puoi passare alla vista `Interattiva`.

In quella modalità trovi:

- intestazione della mappa interattiva
- selettore `Mappa`
- eventuale pulsante `Indietro`
- eventuale pulsante `Livello superiore`
- toggle `Mostra nomi marker`
- controlli di zoom
- canvas della mappa

## Selettore mappa

Il menu `Mappa` permette di scegliere quale mappa visualizzare tra quelle disponibili nell’avventura.

## Navigazione tra mappe

La modalità interattiva supporta due tipi di navigazione tra mappe.

### Indietro

Il pulsante `Indietro` riporta alla mappa visualizzata in precedenza.

### Livello superiore

Se il luogo corrente ha un luogo padre che possiede una mappa interattiva, può comparire il pulsante `Livello superiore`.

Questo ti permette di risalire a una mappa più ampia.

## Il canvas della mappa

Il canvas è la superficie centrale in cui viene mostrata la mappa vera e propria.

Qui puoi:

- vedere la mappa
- vedere i marker
- cliccare o doppio cliccare sui marker
- usare zoom e pan

## Zoom e spostamento

Le mappe interattive supportano:

- zoom avanti e indietro
- reset dello zoom
- scroll orizzontale e verticale
- pan trascinando la mappa
- gesto di pinch
- zoom tramite rotella del mouse quando il cursore è sopra la mappa

## Mostra nomi marker

Con il toggle `Mostra nomi marker` puoi decidere se vedere anche le etichette dei marker direttamente sopra la mappa.

Quando è attivo:

- ogni marker può mostrare il proprio nome o, se il titolo è vuoto, il nome del luogo collegato

Quando è disattivo:

- restano visibili solo le icone dei marker

## Come funzionano i marker

Un marker contiene:

- posizione normalizzata sulla mappa
- titolo opzionale
- collegamento opzionale a un luogo

Il marker viene salvato rispetto alle coordinate della mappa e quindi continua a stare nel punto corretto anche se cambi zoom.

## Comportamento dei marker in lettura

Quando non sei in modalità modifica:

- **click singolo** su un marker lo seleziona
- **doppio click** apre il luogo collegato

Nella modalità interattiva integrata, aprire un luogo significa aggiornare subito il pannello di destra.

Nel pannello mappa grande, aprire un luogo chiude il pannello della mappa e riporta il focus sul luogo selezionato nella dashboard.

## Come si crea un marker

Per creare un marker nel pannello mappa grande:

1. apri la mappa interattiva da `Media`
2. premi `Modifica`
3. premi `Nuovo marker`
4. scegli il luogo da associare
5. clicca su un punto della mappa

## Modalità Modifica

Nel pannello grande esiste un vero stato di modifica.

Quando premi `Modifica`:

- la mappa entra in modalità editing
- puoi creare nuovi marker
- puoi selezionare marker esistenti per modificarli
- puoi trascinare i marker per riposizionarli

Quando premi `Blocca`, esci dalla modalità di modifica.

## Nuovo marker

Quando attivi `Nuovo marker`:

- DnDino ti chiede prima di scegliere il luogo da associare
- poi ti invita a cliccare sulla mappa per posizionarlo

## Scelta del luogo collegato

Quando stai creando o modificando un marker, nell’inspector a destra compare il selettore dei luoghi.

Qui puoi:

- cercare per nome
- vedere i luoghi organizzati in struttura gerarchica
- assegnare il marker al luogo corretto

## Modificare un marker esistente

Quando un marker è selezionato in modalità editing, nell’inspector puoi modificare:

- `Titolo marker`
- `Luogo collegato`

Se il titolo viene lasciato vuoto, DnDino usa come fallback il nome del luogo collegato o un titolo generico.

## Spostare un marker

In modalità modifica puoi trascinare un marker in un nuovo punto della mappa.

Alla fine del trascinamento DnDino salva:

- nuova posizione X
- nuova posizione Y

## Eliminare un marker

Sempre dall’inspector, quando un marker è selezionato, puoi usare:

- `Elimina marker`

## L’inspector della mappa

Il pannello laterale della mappa grande cambia in base allo stato corrente.

### In lettura

Se non stai modificando, l’inspector mostra semplicemente l’elenco dei marker esistenti.

### Durante la creazione di un marker

Se hai attivato `Nuovo marker`, l’inspector mostra:

- istruzioni
- campo di ricerca
- lista dei luoghi selezionabili

### Durante la modifica di un marker

Se hai selezionato un marker esistente, l’inspector mostra:

- campo titolo
- selettore luogo collegato
- riepilogo del luogo attuale
- pulsante per eliminare il marker

## Elenco dei marker

Anche l’elenco dei marker nell’inspector può essere usato per navigare.

Ogni riga mostra:

- titolo del marker
- luogo collegato, se presente

In lettura, cliccando la riga puoi aprire il luogo collegato.

## Come si comporta la mappa nella modalità integrata

Quando usi la modalità `Interattiva` direttamente nella dashboard luoghi:

- la mappa segue il luogo selezionato
- DnDino prova a mostrare la mappa più adatta per quel luogo
- se il luogo non ha una mappa propria, può usare la mappa di un livello superiore

## Eredità della mappa dal luogo padre

Una parte molto utile del sistema è che un luogo può usare anche una mappa di un livello superiore.

Questo permette scenari come:

- il quartiere usa la mappa della città
- la stanza usa la mappa del castello
- il punto di interesse usa la mappa della regione

## Come aprire una mappa interattiva da Media

Nel pannello `Media` di un luogo, le mappe di tipo `Mappa` possono mostrare l’azione:

- `Apri mappa interattiva`

## Quando conviene usare la modalità integrata

Conviene usare la modalità interattiva integrata quando vuoi:

- navigare rapidamente tra i luoghi
- lavorare con mappa e pannello luogo affiancati
- usare la mappa come alternativa all’albero classico

## Quando conviene usare il pannello grande

Conviene usare il pannello grande quando vuoi:

- creare marker
- spostare marker
- cambiare i collegamenti
- lavorare con più precisione

## In pratica

Le mappe interattive sono lo strumento giusto quando vuoi dare ai luoghi una vera dimensione spaziale.

L’idea chiave è semplice:

- il **luogo** resta il record principale
- la **mappa** diventa la superficie visiva
- il **marker** è il collegamento operativo tra immagine e contenuto
