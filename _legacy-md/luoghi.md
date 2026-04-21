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

Questo è molto utile perché ti permette di lavorare sul luogo senza doverlo prima aprire e poi cercare l’azione nel pannello di destra.

Le azioni disponibili nel menu contestuale sono:

- `Rimuovi collegamento`
  - compare quando il luogo è mostrato come collegamento sotto un padre e vuoi scollegarlo da quel punto della gerarchia
- `Aggiungi collegamento`
  - per collegare un luogo già esistente sotto il luogo selezionato
- `Aggiungi sottoluogo`
  - per creare rapidamente un nuovo figlio del luogo selezionato
- `Aggiungi personaggio`
  - per aprire subito il pannello di aggiunta presenza nel luogo
- `Crea Mappa Conc.`
  - per creare direttamente una mappa concettuale legata a quel luogo
- `Crea Combattimento`
  - per preparare subito un nuovo combattimento collegato a quel luogo
- `Modifica`
  - per aprire direttamente il form di modifica del luogo

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
- luogo padre / collegamenti ai luoghi padre
- `Tipo`
- `Segnalazione`
- stato del luogo o stato della quest

### Tipo: Luogo o Quest

Il campo `Tipo` permette di scegliere se il record è:

- `Luogo`
- `Quest`

Questa scelta cambia il comportamento del record.

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

Tutti questi campi usano un editor rich text.

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

Questo rende molto più comode sezioni come:

- `Descrizione DM`
- `Descrizione giocatori`
- `Indizi`
- `Tesori`
- `Note`

## Perché sono utili nei luoghi

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

## Esempi pratici

### Collegare un personaggio descritto nel luogo

Se nella descrizione DM o giocatori scrivi qualcosa come:

- `Il capitano Arven controlla l’ingresso della sala.`

puoi selezionare `capitano Arven`, premere `Link` e collegarlo al relativo `Personaggio`.

Il vantaggio è immediato:

- durante la sessione puoi aprire subito la sua scheda
- non devi cercarlo manualmente in un’altra sezione
- il testo del luogo diventa anche un indice narrativo della scena

### Collegare un altro luogo direttamente dal testo

Se nella descrizione scrivi:

- `Dal corridoio nord si raggiunge la Cripta sommersa.`

puoi selezionare `Cripta sommersa`, premere `Link` e collegarla al relativo `Luogo`.

Questo è molto utile quando i testi del luogo contengono:

- passaggi verso altre aree
- riferimenti a stanze vicine
- legami con città, quartieri o dungeon già creati

In questo modo la descrizione non è più solo narrativa: diventa anche una scorciatoia di navigazione.

## Dove conviene usarli

I punti migliori della scheda luogo per usare i link interni sono:

### Descrizione DM

Perfetta per collegare:

- PNG importanti
- mostri collegati alla scena
- altri luoghi
- regole o note di supporto

### Descrizione giocatori

Utile quando vuoi preparare testi leggibili ma già ricchi di riferimenti cliccabili, per esempio:

- nomi di personaggi conosciuti
- città, stanze o edifici
- oggetti o simboli ricorrenti

### Indizi

Molto utile per trasformare gli indizi in una rete navigabile di rimandi, ad esempio:

- verso un altro luogo
- verso un personaggio
- verso una regola

### Note

Ottimo per il master, soprattutto quando vuoi costruire appunti rapidi ma interconnessi.

## Come si inserisce un link nel testo del luogo

Il flusso è lo stesso usato negli altri editor rich text:

1. seleziona il testo che vuoi trasformare in link
2. premi `Link`
3. scegli il record corretto dal picker
4. conferma

Puoi usarlo sia nel form completo del luogo sia nei punti dell’app in cui il contenuto rich text viene poi letto o consultato.

## Ricerca iniziale del picker

Quando premi `Link`, il picker prova a usare il testo selezionato come filtro iniziale.

Se trova una corrispondenza reale nel nome di un record:

- apre il picker già filtrato

Se invece non trova risultati reali:

- svuota il filtro iniziale
- mostra tutta la lista completa

Questo è molto comodo nei luoghi, perché spesso selezioni già il nome corretto del personaggio o del luogo direttamente dal testo.

## Buone pratiche

Per usare bene i link nei luoghi conviene:

- scrivere i nomi dei personaggi in modo coerente con le loro schede
- usare i nomi reali dei luoghi creati nell’avventura
- collegare i punti di passaggio tra aree diverse
- usare i link soprattutto dove il testo descrive relazioni o movimenti

I link interni sono particolarmente efficaci quando il luogo contiene:

- molti personaggi
- percorsi verso più aree
- riferimenti ricorrenti ad altri nodi della campagna

## In sintesi

Nella sezione `Luoghi`, i link interni servono soprattutto a trasformare le descrizioni in una rete di riferimenti rapidi.

Questo ti permette di usare il testo non solo come descrizione narrativa, ma anche come strumento operativo per:

- aprire schede dei personaggi citati
- navigare verso altri luoghi
- consultare regole o riferimenti senza interrompere il flusso della sessione

## Asset del luogo

Ogni luogo può avere asset propri, separati in:

- immagini
- mappe

Nel form puoi:

- aggiungere immagini
- aggiungere mappe
- scegliere la copertina del luogo
- rimuovere la copertina

Le immagini e le mappe restano distinte, ma la copertina può essere scelta da qualunque asset del luogo.

Per ogni asset puoi configurare:

- nome visualizzato
- visibilità per `Giocatori`
- visibilità per `Master`
- testo di presentazione

## Modifica di un luogo

Dopo la creazione, il luogo può essere riaperto in modifica dalla dashboard.

Nel pannello di dettaglio c’è sempre un pulsante `Modifica` vicino al nome del luogo selezionato, così puoi tornare subito al form e aggiornare:

- dati principali
- gerarchia
- descrizioni
- immagini
- mappe

## Collegare un luogo esistente come sottoluogo

Oltre a creare un nuovo sottoluogo, la dashboard permette anche di collegare un luogo già esistente come figlio di un altro luogo.

Questo è utile quando vuoi riusare una struttura già creata invece di duplicarla.

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

## Aggiornamento rapido dello stato

Nella hero del luogo puoi cambiare velocemente lo stato senza aprire il form.

Per i **luoghi** puoi aggiornare:

- non visitato
- in visita
- visitato

Per le **quest** puoi aggiornare:

- inattiva
- non disponibile
- attiva
- completata

## Le schede del dettaglio

Il pannello di destra usa una barra di focus con cinque sezioni principali:

- `Panoramica`
- `Presenze`
- `Combattimenti`
- `Media`
- `Note`

### Panoramica

La scheda `Panoramica` raccoglie il contenuto descrittivo del luogo:

- descrizione DM
- descrizione giocatori
- indizi
- tesori
- eventuali mappe concettuali collegate al luogo

È il punto giusto per leggere rapidamente il contenuto narrativo del luogo.

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

Queste note sono modificabili direttamente dalla dashboard senza tornare al form completo del luogo.

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

In questo caso la presenza mantiene il legame con lo stato contestuale di campagna, quindi eredita il personaggio avventura già esistente invece di creare uno stato locale separato.

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

- Goblin
- Goblin 2
- Goblin 3

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

Se invece nasce da un **Personaggio Avventura**, lo stato locale non viene duplicato nello stesso modo: la presenza continua a fare riferimento allo stato contestuale del personaggio collegato all’avventura.

## Ruolo nel luogo

Ogni presenza ha un ruolo contestuale:

- alleato
- neutrale
- nemico

Questo ruolo è importante sia per la lettura della scena sia per alcuni flussi successivi, ad esempio nei combattimenti.

## Note DM sulle presenze

Ogni presenza del luogo ha sempre un pulsante `Note DM`.

Le note:

- possono essere lette e modificate da popover
- vengono salvate localmente sulla presenza del luogo
- restano separate dalle note di altri contesti

Questo è utile quando lo stesso personaggio ha comportamenti o dettagli diversi in luoghi diversi.

## Combattimenti collegati al luogo

I combattimenti nei luoghi nascono direttamente dal luogo selezionato.

Quando crei un nuovo combattimento:

- il combattimento viene salvato come incontro di quel luogo
- compare subito nella scheda `Combattimenti`
- può essere riaperto in un secondo momento

Questo collegamento è importante perché la campagna resta organizzata anche sul piano spaziale: ogni scontro appartiene davvero al luogo in cui è stato preparato o giocato.

## Media del luogo

La sezione media del luogo distingue chiaramente:

- immagini
- mappe

Le immagini sono pensate per illustrazioni, riferimenti o scene.

Le mappe sono pensate per:

- consultazione rapida
- presentazione
- uso interattivo

## Mappe ereditate dai luoghi padre

La dashboard può mostrare anche le mappe dei luoghi padre.

Questo comportamento è controllato da un toggle:

- `Mostra mappe dei luoghi padre`

Quindi il pannello mappe del luogo può farti vedere:

- solo le mappe del luogo corrente
- oppure anche le mappe ereditate lungo la sua gerarchia

## Mappa interattiva

Quando una mappa è selezionata come mappa interattiva del luogo, puoi aprirla direttamente dalla dashboard.

La mappa interattiva supporta:

- zoom
- spostamento
- marker
- navigazione tra luoghi

## Marker della mappa interattiva

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

Puoi anche scegliere se mostrare o nascondere le etichette dei marker.

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

Questo rende la sezione `Luoghi` utile non solo per lo spazio fisico della campagna, ma anche per la sua struttura narrativa.

## Quando usare la sezione Luoghi

La dashboard `Luoghi` è il punto giusto quando vuoi:

- costruire la geografia della campagna
- definire sottoluoghi e collegamenti
- preparare quest e relativo stato
- collocare presenze nel mondo
- collegare immagini e mappe
- usare una mappa interattiva per navigare
- aprire o creare combattimenti legati a uno specifico luogo

## Screenshot suggeriti

- dashboard luoghi completa
- form di creazione luogo
- hero di un luogo selezionato
- scheda `Presenze`
- form `Aggiungi presenza al luogo`
- scheda `Combattimenti`
- scheda `Media`
- esempio di mappa interattiva con marker

!!! tip
    Se l’avventura è molto grande, la sezione `Luoghi` funziona meglio se la usi come una vera mappa mentale della campagna: luoghi per la struttura, quest per i nodi narrativi, presenze per chi occupa la scena e combattimenti per ciò che succede in quel punto del mondo.
