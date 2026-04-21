# Avventura

La sezione **Avventura** è il centro organizzativo di una campagna in DnDino. Qui nasce la struttura principale del tuo lavoro: il titolo della campagna, la sua identità visiva, i personaggi collegati, le sessioni, i luoghi, le immagini condivise, le mappe e gli accessi rapidi ai combattimenti.

!!! tip
    Pensa alla dashboard avventura come al **quartier generale della campagna**: non è il punto in cui fai tutto nel dettaglio, ma è il posto da cui raggiungi velocemente tutte le aree davvero operative.

Questa pagina spiega il percorso principale:

- creazione di una nuova avventura
- modifica e gestione di un’avventura esistente
- funzionamento della dashboard avventura
- rapporto tra la dashboard e le sottosezioni dedicate

Le aree più specifiche, come **Luoghi**, **Mappe concettuali**, **Sessione live**, **Personaggi**, **Immagini** e **Mappe**, verranno invece approfondite nelle pagine figlie dedicate.

## A cosa serve un’avventura

In DnDino un’avventura è il contenitore principale di una campagna o di un arco narrativo. Serve a raccogliere in un unico contesto:

- i personaggi collegati alla campagna
- i luoghi e le quest
- le sessioni testuali e live
- le immagini condivise
- le mappe associate ai luoghi
- le mappe concettuali globali
- i combattimenti che nascono nei luoghi collegati all’avventura

L’avventura non è quindi solo una scheda anagrafica, ma il punto da cui si entra in tutta la parte operativa della campagna.

## Dove si crea un’avventura

La creazione parte dalla **lista avventure**.

Da questa schermata puoi:

- creare una nuova avventura con il pulsante `Nuova`
- creare la prima avventura dal grande pulsante centrale `Crea un'avventura`, se il database è ancora vuoto
- aprire un’avventura esistente cliccando sulla sua riga
- modificare un’avventura esistente
- clonare un’avventura già presente
- eliminare un’avventura

La lista può anche essere ordinata per:

- nome
- data creazione
- ultima modifica

!!! note
    Quando ordini per **ultima modifica**, DnDino non guarda solo la scheda avventura, ma considera anche attività collegate come luoghi, sessioni, personaggi avventura, mappe concettuali e combattimenti.

## Creazione di una nuova avventura

Quando apri il form di creazione, DnDino ti propone una scheda con le informazioni principali della campagna.

I campi principali sono:

- `Titolo`
- `Autore`
- `Ambientazione`
- `Descrizione breve`
- `Stato`

Il campo **Stato** usa un controllo segmentato e permette di indicare se l’avventura è:

- non iniziata
- in corso
- completata

## Descrizione estesa

Sotto alle informazioni principali trovi anche una sezione **Descrizione** più ampia.

Questa area serve per annotare una presentazione più completa della campagna, ad esempio:

- tono dell’avventura
- contesto narrativo
- obiettivi iniziali
- appunti generali per il master

La descrizione lunga non viene persa nella dashboard: se è presente, può essere riaperta rapidamente anche più avanti.

## Copertina e immagini avventura

Nel form puoi assegnare una **copertina** all’avventura. La copertina viene usata come immagine rappresentativa della campagna nelle schermate principali.

Puoi anche aggiungere immagini nella sezione **Immagini avventura**. Queste immagini:

- restano collegate all’avventura
- non appartengono a un luogo specifico
- possono essere mostrate rapidamente ai giocatori o al master dalla dashboard

Per ogni immagine puoi gestire:

- nome visualizzato
- visibilità per `Giocatori`
- visibilità per `Master`

## Modifica di un’avventura esistente

Quando apri un’avventura esistente in modifica, il form è lo stesso della creazione, ma con una sezione in più: **Ripristino avventura**.

Il ripristino non cancella la struttura della campagna, ma azzera lo stato di gioco corrente. In particolare:

- rimuove tutti i personaggi avventura collegati
- elimina tutte le sessioni salvate
- riporta luoghi e quest allo stato iniziale
- rimette PNG e mostri vivi, a PF massimi e senza condizioni
- azzera i combattimenti preparati senza cancellarne la struttura

Questa funzione è utile quando vuoi riutilizzare l’ossatura di una campagna o riportare l’avventura a uno stato pulito senza ricostruirla da zero.

## Clonazione ed eliminazione

Dalla lista avventure puoi anche:

### Clonare un’avventura

La clonazione crea una copia della campagna attraverso il servizio interno di duplicazione. È utile quando vuoi:

- partire da una struttura simile
- riutilizzare un’impostazione di base
- fare una variante di una campagna esistente

### Eliminare un’avventura

Quando elimini un’avventura, DnDino rimuove il record principale e avvia anche la pulizia delle risorse collegate. In più aggiorna i riferimenti dei personaggi globali per togliere il collegamento all’avventura cancellata.

## Apertura della dashboard avventura

Cliccando su un’avventura nella lista entri nella sua **dashboard**, che è il vero centro operativo della campagna.

La dashboard è organizzata come una schermata a pannelli:

- una fascia superiore con intestazione e controllo sessione live
- due colonne inferiori con card dedicate alle varie aree della campagna

L’ordine dei pannelli può essere personalizzato dalle impostazioni dell’app.

## Intestazione della dashboard

La parte alta della dashboard raccoglie le informazioni essenziali dell’avventura:

- copertina
- titolo
- stato
- descrizione breve
- ambientazione
- autore

Se l’avventura ha anche una descrizione lunga, compare un pulsante dedicato per aprirla in un popover e leggerla senza uscire dalla dashboard.

Da qui puoi anche entrare in **Modifica** per tornare al form dell’avventura e aggiornarne i dati.

## Sessione live

Accanto all’intestazione c’è il pannello **Sessione live**.

Questa sezione serve per:

- avviare una nuova sessione live per l’avventura
- vedere se una sessione è in corso oppure in pausa
- monitorare il tempo trascorso
- mettere in pausa la sessione
- chiuderla e salvarla

Quando la sessione live dell’avventura è attiva, il **player globale** e i **luoghi** seguono questo contesto.

Se esiste già una sessione live aperta in un’altra avventura, la dashboard lo segnala chiaramente e non ti lascia avviarne una seconda in parallelo.

## I pannelli della dashboard

Sotto l’intestazione la dashboard mostra i pannelli principali dell’avventura.

Quelli previsti attualmente sono:

- `Luoghi e Quest`
- `Personaggi`
- `Sessioni`
- `Immagini`
- `Mappe`
- `Mappe Concettuali`
- `Metadati`

!!! tip
    Dalle impostazioni è possibile modificare l'ordine dei pannelli all'interno della Dashboard Avventura, sia nella scelta della colonna che nella scelta dell'ordine.

### Luoghi e Quest

Questo pannello è il punto di ingresso alla dashboard dei luoghi.

Da qui vedi rapidamente:

- numero totale dei luoghi
- numero delle quest
- numero delle quest completate

In più possono comparire accessi rapidi a:

- ultimo luogo utile
- ultimo combattimento utile

Aprendo questa card entri nella sezione che gestisce:

- luoghi
- sottoluoghi
- presenze
- immagini di luogo
- mappe
- mappe interattive
- combattimenti collegati ai luoghi

Questa parte verrà descritta meglio nella sottopagina dedicata ai **Luoghi**.

### Personaggi

Il pannello **Personaggi** mostra i personaggi collegati alla campagna.

Qui puoi:

- vedere i personaggi avventura già collegati
- aggiungerne di nuovi
- curarli rapidamente con `Cura tutti`
- aprire il loro stato contestuale di campagna

Questa sezione non sostituisce la scheda base del personaggio: mostra il livello di collegamento specifico all’avventura, con stato, PF e condizioni contestuali.

La differenza tra:

- scheda base personaggio
- personaggio avventura
- personaggio luogo
- partecipante al combattimento

verrà approfondita nella sottopagina dedicata ai **Personaggi**.

### Sessioni

Il pannello **Sessioni** raccoglie:

- sessioni testuali
- sessioni live
- appunti
- riepiloghi
- timeline

Da qui puoi anche creare una nuova sessione testuale. Le sessioni sono quindi la memoria narrativa e operativa della campagna.

Questa area sarà approfondita nella sottopagina dedicata alla **Sessione live** e alla gestione delle sessioni.

### Immagini

Il pannello **Immagini** raccoglie le immagini globali dell’avventura, cioè quelle non legate a un luogo specifico.

Da qui puoi:

- aggiungere immagini
- sfogliarle per pagine
- mostrarle rapidamente ai giocatori
- mostrarle rapidamente al master

Questa è la zona giusta per tutto il materiale visivo “di campagna” che non appartiene a un singolo luogo.

### Mappe

Il pannello **Mappe** mostra tutte le mappe collegate ai luoghi dell’avventura.

Le mappe non si aggiungono qui direttamente: compaiono in dashboard quando sono già state collegate a un luogo.

Da questa card puoi:

- sfogliare le mappe dell’avventura
- mostrarle a giocatori o master
- aprire direttamente la relativa mappa interattiva del luogo, se presente

Questa parte sarà approfondita nella sottopagina dedicata a **Mappe** e **Mappe interattive**.

### Mappe Concettuali

Il pannello **Mappe Concettuali** raccoglie le mappe globali dell’avventura.

Da qui puoi:

- vedere quante mappe concettuali esistono
- aprirle rapidamente
- crearne una nuova

Le mappe concettuali sono utili per collegare tra loro idee, luoghi, personaggi e relazioni narrative. Verranno approfondite nella sottopagina dedicata.

### Metadati

Se nelle impostazioni hai attivato la visualizzazione dei metadati, compare anche un pannello tecnico con:

- ID dell’avventura
- data di creazione
- data ultima modifica

È una sezione utile soprattutto per controllo, diagnostica o gestione avanzata.

## Relazione con le sottopagine

La pagina **Avventura** è una panoramica generale. Da qui in poi le aree figlie servono ad approfondire i singoli strumenti operativi.

Le sottopagine di questa guida saranno:

- **Luoghi e Quest**
- **Mappe concettuali**
- **Immagini**
- **Mappe**
- **Mappe interattive**
- **Sessione live**
- **Personaggi**

In pratica:

- questa pagina spiega **come nasce e come si struttura** un’avventura e come è fatta la Dashboard Avventura
- le pagine figlie spiegano **come si usa davvero ogni sezione interna**

## Quando usare questa sezione

La sezione Avventura è il punto giusto quando vuoi:

- creare una nuova campagna
- definire copertina, stato e descrizione dell’avventura
- riprendere il lavoro da una campagna esistente
- entrare nella dashboard principale
- avviare una sessione live
- raggiungere velocemente luoghi, personaggi, sessioni, immagini e mappe della campagna
