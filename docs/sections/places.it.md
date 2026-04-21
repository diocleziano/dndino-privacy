# Luoghi

La sezione **Luoghi** raccoglie tutto ciò che riguarda gli spazi di gioco di un’avventura: città, dungeon, stanze, aree narrative, quest collegate, presenze, combattimenti, immagini, mappe e mappe interattive.

È una delle sezioni più ricche dell’app, perché mette insieme:

- struttura narrativa
- stato di esplorazione
- contenuti da mostrare ai giocatori
- presenze contestuali
- accesso rapido ai combattimenti

## A cosa serve la sezione Luoghi

La dashboard dei luoghi serve per organizzare l’avventura sul piano spaziale e narrativo.

Qui puoi:

- creare luoghi e quest
- costruire gerarchie di luoghi e sottoluoghi
- collegare immagini e mappe
- gestire le presenze nel luogo
- creare e riaprire combattimenti legati a uno specifico luogo
- annotare descrizioni separate per DM e giocatori
- usare una mappa interattiva per muoverti tra i luoghi

## Come si raggiunge

La sezione si apre dalla **dashboard avventura**, entrando nella card `Luoghi e Quest`.

Da quella card puoi:

- aprire l’intera dashboard dei luoghi
- usare eventuali scorciatoie rapide verso un luogo recente
- usare eventuali scorciatoie rapide verso un combattimento recente collegato a un luogo

## Struttura della schermata

La dashboard `Luoghi` è organizzata in due modalità principali:

- `Normale`
- `Interattiva`

e in una struttura a due aree:

- **colonna sinistra** con albero, ricerca, filtri e azioni rapide
- **pannello destro** con il dettaglio del luogo selezionato

## Modalità Normale e Interattiva

### Modalità Normale

È la modalità classica, pensata per lavorare direttamente su:

- albero dei luoghi
- dettaglio del luogo selezionato
- presenze
- combattimenti
- media
- note

È la modalità più adatta per preparare e modificare l’avventura.

### Modalità Interattiva

La modalità `Interattiva` si attiva quando nell’avventura esistono mappe interattive disponibili.

In questa modalità il focus si sposta sulla navigazione tramite mappa:

- la parte sinistra della schermata mostra la mappa interattiva al posto dell’albero classico dei luoghi
- i marker possono essere selezionati
- con doppio click si può aprire il luogo collegato nel pannello di destra
- è possibile mostrare o nascondere i nomi dei marker
- è possibile gestire zoom e spostamento sulla mappa

Dal pannello `Media` puoi comunque aprire rapidamente la mappa interattiva associata a una mappa del luogo, ma nella modalità `Interattiva` la mappa diventa proprio il contenuto principale della parte sinistra della dashboard.

## La colonna di sinistra

La colonna sinistra è il pannello di navigazione della sezione.

Qui trovi:

- ricerca
- filtri
- riepilogo rapido
- albero dei luoghi e delle quest

### Menu contestuale sui luoghi nell'albero

Nella modalità ad albero puoi fare **tasto destro su un luogo** per aprire un menu contestuale con azioni rapide direttamente su quel nodo.

Le azioni disponibili nel menu contestuale sono:

- `Rimuovi collegamento`
- `Aggiungi collegamento`
- `Aggiungi sottoluogo`
- `Aggiungi personaggio`
- `Crea Mappa Conc.`
- `Crea Combattimento`
- `Modifica`

Questo menu è uno dei modi più rapidi per costruire la struttura dell’avventura mentre lavori nell’albero.

### Filtri e riepilogo

La sidebar mostra anche un riepilogo compatto con:

- totale dei luoghi
- numero delle quest
- numero dei luoghi in visita

In base alla modalità e al punto della schermata, puoi usare filtri come:

- tutti
- luoghi
- quest
- in visita
- attive

## Creazione di un luogo o di una quest

Per creare un nuovo record usi il pulsante di creazione nella dashboard dei luoghi.

Nel form trovi tre gruppi principali:

- `Informazioni principali`
- `Descrizioni`
- `Asset del luogo`

## Informazioni principali del luogo

Nel form puoi compilare:

- `Nome`
- luogo padre o collegamenti ai luoghi padre
- `Tipo`
- `Segnalazione`
- stato del luogo o stato della quest

### Tipo: Luogo o Quest

Il campo `Tipo` permette di scegliere se il record è:

- `Luogo`
- `Quest`

Se il record è un **Luogo**, usa lo stato di visita:

- non visitato
- in visita
- visitato

Se il record è una **Quest**, usa invece lo stato di avanzamento:

- inattiva
- non disponibile
- attiva
- completata

## Luoghi padre e gerarchia

Il form dei luoghi supporta una gerarchia avanzata.

Puoi selezionare uno o più luoghi padre, e DnDino salva davvero questo collegamento come struttura gerarchica dedicata.

Questo significa che un luogo può:

- stare alla radice dell’avventura
- vivere come sottoluogo di un altro luogo
- essere collegato anche in più punti della struttura, quando serve

Il form impedisce comunque di creare cicli, perché esclude automaticamente il luogo stesso e il suo sottoalbero dai possibili padri selezionabili.

## Segnalazioni del luogo

Ogni luogo può avere una o più segnalazioni speciali, mostrate anche nella dashboard.

Le segnalazioni disponibili sono:

- pericoloso
- importante
- segreto
- bloccato

Servono come evidenziatori rapidi per leggere meglio l’avventura a colpo d’occhio.

## Descrizioni del luogo

La sezione `Descrizioni` del form è divisa in più campi ricchi:

- `Descrizione DM`
- `Descrizione giocatori`
- `Indizi`
- `Tesori`
- `Note`

Questa distinzione è molto utile, perché ti permette di separare:

- ciò che il master deve sapere
- ciò che i giocatori possono vedere o scoprire
- informazioni di supporto come indizi e tesori

## Link interni nei testi del luogo

Anche nella sezione `Luoghi` il sistema dei **link interni** è molto utile.

Qui non serve tanto per automatizzare attacchi come nella scheda personaggio, ma soprattutto per rendere il testo del luogo **navigabile** e più rapido da usare durante la sessione.

Nei campi rich text del luogo puoi inserire collegamenti verso:

- `Personaggio`
- `Luogo`
- `Incantesimo`
- `Talento`
- `Regola`
- e, quando serve, anche link di tiro

### Perché sono utili nei luoghi

I luoghi contengono spesso testo ricco di riferimenti:

- personaggi presenti o nominati
- luoghi collegati
- oggetti o incantesimi menzionati
- regole particolari di scena

Trasformare questi riferimenti in link interni permette di:

- aprire rapidamente la scheda di un personaggio citato
- saltare direttamente a un altro luogo dell’avventura
- consultare un incantesimo o una regola senza uscire dal contesto
- costruire descrizioni più dense ma comunque facili da navigare

### Esempi pratici

Puoi collegare un personaggio descritto nel luogo, per esempio `capitano Arven`, oppure un altro luogo citato nel testo, come `Cripta sommersa`.

In questo modo la descrizione non è più solo narrativa: diventa anche una scorciatoia di navigazione.

### Dove conviene usarli

I punti migliori della scheda luogo per usare i link interni sono:

- `Descrizione DM`
- `Descrizione giocatori`
- `Indizi`
- `Note`

### Ricerca iniziale del picker

Quando premi `Link`, il picker prova a usare il testo selezionato come filtro iniziale.

Se trova una corrispondenza reale nel nome di un record:

- apre il picker già filtrato

Se invece non trova risultati reali:

- svuota il filtro iniziale
- mostra tutta la lista completa

## Asset del luogo

Ogni luogo può avere asset propri, separati in:

- immagini
- mappe

Nel form puoi:

- aggiungere immagini
- aggiungere mappe
- scegliere la copertina del luogo
- rimuovere la copertina

Per ogni asset puoi configurare:

- nome visualizzato
- visibilità per `Giocatori`
- visibilità per `Master`
- testo di presentazione

## Hero del luogo

Quando selezioni un luogo, il pannello di destra mostra una hero con:

- copertina del luogo
- nome
- tipo (`Luogo` o `Quest`)
- stato corrente
- eventuali segnalazioni
- catena gerarchica del luogo

In più compare un riepilogo rapido con:

- `Presenze`
- `Sottoluoghi`
- `Immagini`
- `Mappe`

## Le schede del dettaglio

Il pannello di destra usa una barra di focus con cinque sezioni principali:

- `Panoramica`
- `Presenze`
- `Combattimenti`
- `Media`
- `Note`

### Panoramica

La scheda `Panoramica` raccoglie:

- descrizione DM
- descrizione giocatori
- indizi
- tesori
- eventuali mappe concettuali collegate al luogo

### Presenze

La scheda `Presenze` raccoglie i personaggi presenti nel luogo.

Da qui puoi:

- vedere tutte le presenze del luogo
- aggiungere una nuova presenza
- aprire il dettaglio contestuale della presenza
- cambiare il ruolo nel luogo
- leggere o modificare le `Note DM`
- rimuovere la presenza

### Combattimenti

La scheda `Combattimenti` mostra tutti gli scontri collegati al luogo.

Da qui puoi:

- creare un nuovo combattimento per il luogo
- riaprire un combattimento esistente
- vedere se è non iniziato, in pausa o concluso
- eliminare un combattimento

### Media

La scheda `Media` raccoglie:

- immagini del luogo
- mappe del luogo
- eventuali mappe ereditate dai luoghi padre, se attive

Da qui puoi:

- sfogliare le immagini
- sfogliare le mappe
- mostrarle ai giocatori
- mostrarle al master
- aprire direttamente una mappa interattiva

### Note

La scheda `Note` è dedicata alle note rapide del luogo per il DM.

## Presenze del luogo

Le presenze del luogo sono gestite in modo contestuale e separato rispetto ad avventura e combattimento.

Questo permette di avere:

- nomi visualizzati contestuali
- ruolo nel luogo
- note DM locali
- stato locale, quando serve

## Due origini possibili per una presenza

Quando aggiungi una presenza al luogo, il form ti chiede l’`Origine`.

Le sorgenti possibili sono:

- `Personaggio Avventura`
- `Scheda base`

### Personaggio Avventura

Questa origine usa un personaggio già collegato all’avventura.

In questo caso la presenza mantiene il legame con lo stato contestuale di campagna.

### Scheda base

Questa origine clona un record base di tipo:

- `PNG`
- `Mostro`

I record di tipo `Eroe` non sono selezionabili in questa modalità.

## Regole di unicità delle presenze

Nella dashboard dei luoghi DnDino applica regole precise:

- un `Personaggio Avventura` può essere collocato una sola volta nello stesso luogo
- un `PNG` base può essere aggiunto una sola volta nello stesso luogo
- un `Mostro` base può essere aggiunto più volte nello stesso luogo

Quando aggiungi più istanze dello stesso mostro, il nome visualizzato viene numerato automaticamente, ad esempio:

- `Goblin`
- `Goblin 2`
- `Goblin 3`

## Dati della presenza nel luogo

Nel form della presenza puoi impostare:

- `Ruolo incontro`
- `Nome visualizzato`
- `Condizioni`
- `Note DM`

Se la presenza nasce da una **scheda base** (`PNG` o `Mostro`), hai anche lo stato locale del luogo:

- PF temporanei
- PF attuali
- stato

Se invece nasce da un **Personaggio Avventura**, la presenza continua a fare riferimento allo stato contestuale del personaggio collegato all’avventura.

## Ruolo nel luogo

Ogni presenza ha un ruolo contestuale:

- alleato
- neutrale
- nemico

Questo ruolo è importante sia per la lettura della scena sia per alcuni flussi successivi, ad esempio nei combattimenti.

## Combattimenti collegati al luogo

I combattimenti nei luoghi nascono direttamente dal luogo selezionato.

Quando crei un nuovo combattimento:

- il combattimento viene salvato come incontro di quel luogo
- compare subito nella scheda `Combattimenti`
- può essere riaperto in un secondo momento

## Media del luogo

La sezione media del luogo distingue chiaramente:

- immagini
- mappe

La dashboard può mostrare anche le mappe dei luoghi padre tramite il toggle:

- `Mostra mappe dei luoghi padre`

## Mappa interattiva

Quando una mappa è selezionata come mappa interattiva del luogo, puoi aprirla direttamente dalla dashboard.

La mappa interattiva supporta:

- zoom
- spostamento
- marker
- navigazione tra luoghi

### Marker della mappa interattiva

Ogni marker può avere:

- posizione sulla mappa
- titolo
- luogo bersaglio associato

I marker possono essere:

- creati
- spostati
- rinominati
- associati a un luogo
- eliminati

Comportamento base:

- click singolo: seleziona il marker
- doppio click: apre il luogo collegato nel pannello di destra

## Relazione tra Luoghi, Mappe e Mappe Interattive

Conviene pensare a queste tre cose come a livelli diversi:

- il **luogo** è il contenitore narrativo e strutturale
- la **mappa** è un asset visuale collegato al luogo
- la **mappa interattiva** è una mappa scelta come supporto navigabile, arricchita da marker

## Quest nella sezione Luoghi

Le quest vivono nella stessa sezione dei luoghi, ma hanno un comportamento dedicato.

Una quest:

- compare nell’albero insieme ai luoghi
- usa uno stato di avanzamento invece dello stato di visita
- può comunque avere descrizioni, note, immagini, mappe, presenze e collegamenti contestuali

## Quando usare la sezione Luoghi

La dashboard `Luoghi` è il punto giusto quando vuoi:

- costruire la geografia della campagna
- definire sottoluoghi e collegamenti
- preparare quest e relativo stato
- collocare presenze nel mondo
- collegare immagini e mappe
- usare una mappa interattiva per navigare
- aprire o creare combattimenti legati a uno specifico luogo

!!! tip
    Se l’avventura è molto grande, la sezione `Luoghi` funziona meglio se la usi come una vera mappa mentale della campagna: luoghi per la struttura, quest per i nodi narrativi, presenze per chi occupa la scena e combattimenti per ciò che succede in quel punto del mondo.
