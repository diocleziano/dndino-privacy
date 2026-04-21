# Combattimento

La modalità **Combattimento** di DnDino è pensata per essere il tracker operativo principale dello scontro. Questa pagina descrive la modalità di combattimento standard di DnDino.

Il combattimento nasce sempre nel contesto di un **luogo** e porta con sé i personaggi, le presenze locali e gli eventuali mostri o PNG collegati a quella scena.

Questa pagina spiega il flusso completo:

- preparazione del pre-combattimento
- gestione dei partecipanti
- avvio dello scontro
- utilizzo del turno corrente
- applicazione di danni, cure, condizioni e tiri salvezza
- integrazione con la **Finestra Giocatori**
- chiusura e riepilogo finale

## Utilizzo con uno o due schermi

Il combattimento di DnDino funziona bene anche su **schermo singolo**: tutta la parte operativa resta nel pannello principale e puoi gestire normalmente partecipanti, turni, danni, condizioni e riepilogo finale senza bisogno di un secondo monitor.

Detto questo, se hai a disposizione una configurazione con due schermi, puoi usare:

- uno schermo principale per il pannello di controllo
- un secondo schermo o monitor per la **Finestra Giocatori**

In questa configurazione il flusso diventa ancora più comodo:

- sullo schermo del DM restano visibili la lista dei partecipanti, i controlli del round, il turno corrente, i testi di attacco, le note DM e le modifiche rapide
- sullo schermo dei giocatori viene mostrata una presentazione pulita del partecipante attivo, con immagine e overlay contestuale

In pratica:

- su schermo singolo usi tutto il combattimento dalla schermata principale
- con due schermi separi il pannello tecnico del DM dalla presentazione per i giocatori

!!! tip
    Il secondo schermo non è obbligatorio: è semplicemente un potenziamento molto utile quando vuoi mostrare ai giocatori immagini e informazioni del turno corrente senza esporre il pannello tecnico del DM.

## Come funziona la Finestra Giocatori durante il combattimento

Quando il combattimento viene avviato, DnDino può aprire o aggiornare automaticamente la **Finestra Giocatori**.

Se la presentazione ai giocatori è attiva:

- all’inizio del combattimento può comparire una breve **intro** con i partecipanti
- durante il combattimento la finestra si aggiorna sul **partecipante del turno corrente**
- alla fine dello scontro può comparire un **riepilogo finale**

Durante il combattimento la finestra dei giocatori non mostra il pannello tecnico del DM, ma una presentazione visiva con:

- immagine del partecipante attivo
- nome mostrato ai giocatori
- informazioni di overlay, se abilitate

L’overlay può includere:

- round corrente
- PF attuali, massimi e temporanei
- condizioni
- prossimo turno

Per i nemici, alcune informazioni possono essere trattate in modo separato rispetto agli eroi.

## Impostazioni della Finestra Giocatori e del secondo schermo

Le impostazioni più importanti si trovano in **Impostazioni**, nella sezione dedicata alla presentazione del combattimento e della finestra giocatori.

### Apertura e comportamento generale

Le impostazioni principali sono:

- `Apri la finestra giocatori anche con un solo monitor`
- `Mostra controlli finestra giocatori nella topbar`
- `Mostra intro combattimento ai giocatori`
- `Mostra riepilogo finale ai giocatori`

#### Apri la finestra giocatori anche con un solo monitor

Se questa opzione è attiva, DnDino può aprire automaticamente la finestra dei giocatori anche quando stai lavorando con un solo monitor.

Se è disattiva:

- con un solo monitor la finestra non si apre automaticamente
- se però la finestra è già aperta, continua comunque ad aggiornarsi

#### Mostra controlli finestra giocatori nella topbar

Se attivi questa opzione, nella barra superiore dell’app compaiono i pulsanti per:

- aprire manualmente la finestra giocatori
- chiuderla manualmente

#### Mostra intro combattimento ai giocatori

Quando premi `Avvia scontro`, la finestra dei giocatori può mostrare una breve introduzione con:

- titolo dello scontro
- partecipanti coinvolti
- conteggio dei partecipanti

Se disattivi questa opzione, il combattimento passa direttamente alla presentazione del primo partecipante attivo.

#### Mostra riepilogo finale ai giocatori

Quando il combattimento termina, la finestra dei giocatori può mostrare un riepilogo finale.

Nel riepilogo per i giocatori vengono mostrati solo i dati utili a loro, come:

- danni inflitti dagli eroi
- danni subiti dagli eroi
- immagine del peggior nemico

Il riepilogo finale dei giocatori resta visibile finché non cambi contenuto nella finestra oppure non la chiudi.

### Informazioni mostrate durante il turno

Le impostazioni che regolano l’overlay del partecipante attivo sono:

- `Mostra round nella schermata giocatori`
- `Mostra PF nella schermata giocatori`
- `Mostra condizioni nella schermata giocatori`
- `Mostra prossimo turno nella schermata giocatori`

### Informazioni su nemici, mostri e PNG

Per i partecipanti che non sono eroi esistono controlli dedicati:

- `Mostra dettagli di PNG e mostri ai giocatori`
- `Mostra condizioni dei nemici ai giocatori`
- `Mostra i nomi dei nemici ai giocatori`

Questo permette di decidere se la finestra dei giocatori deve:

- mostrare solo la creatura in modo evocativo
- oppure mostrare anche dati più tecnici

## Dove si apre il combattimento

Il combattimento viene creato dal contesto del **luogo**. Una volta aperto, DnDino mostra una schermata divisa in due colonne principali:

- a sinistra il tracker operativo del combattimento
- al centro il pannello principale della scena o del turno corrente

Quando il combattimento non è ancora iniziato, il pannello centrale mostra il **Riepilogo pre-combattimento**.

Quando lo scontro è attivo, lo stesso pannello diventa l’area dedicata al **Turno corrente**.

Quando il combattimento è terminato, il pannello centrale mostra il **Riepilogo finale dello scontro** per il DM.

## La struttura generale della schermata

### Colonna sinistra

La colonna sinistra contiene:

- `Controllo combattimento`
- intestazione della lista partecipanti
- lista ordinata dei partecipanti

La lista è racchiusa tra due righe decorative e funzionali:

- `Inizio Round`
- `Fine Round`

### Pannello centrale

Il pannello centrale cambia in base allo stato del combattimento:

- **prima dell’avvio** mostra il riepilogo pre-combattimento
- **durante lo scontro** mostra il personaggio o partecipante del turno corrente
- **a fine combattimento** mostra il riepilogo finale del DM

## Pre-combattimento

Il pre-combattimento serve per preparare lo scontro prima di far partire il primo turno.

È la fase in cui conviene sistemare soprattutto tre cose:

- il nome dei mostri, quando vuoi distinguerli meglio al tavolo
- le iniziative degli eroi, inserendole a mano
- le iniziative di PNG e mostri, tirandole automaticamente oppure scrivendole manualmente

## Riepilogo pre-combattimento

La card iniziale mostra una panoramica rapida con metriche come:

- partecipanti
- eroi
- alleati
- nemici
- PF totali dei nemici
- eventuali partecipanti già in condizioni critiche

## Iniziativa personaggi

La sezione `Iniziativa personaggi` raccoglie gli eroi principali e permette di modificare rapidamente l’iniziativa prima di ordinare lo scontro.

Per ogni riga trovi:

- nome del partecipante
- sottotitolo contestuale
- campo iniziativa
- pulsante `Elimina`

## PNG e mostri

La sezione `PNG e mostri` è dedicata ai partecipanti non eroi.

Qui puoi:

- modificare rapidamente l’iniziativa
- rinominare al volo mostri e PNG, così da distinguerli meglio per comodità operativa
- usare `Init PNG/Mostri` per tirare automaticamente l’iniziativa dei non eroi
- inserire a mano il valore dell’iniziativa se preferisci usare il tiro fatto fuori dall’app
- rimuovere rapidamente un partecipante con `Elimina`

## Azioni principali del pre-combattimento

Nel riepilogo pre-combattimento le azioni principali sono:

- `Aggiungi`
- `Ordina`
- `Avvia scontro`

Se almeno un partecipante ha iniziativa `0`, DnDino chiede conferma prima di iniziare.

## Da dove possono arrivare i partecipanti

Il pannello di aggiunta può raccogliere partecipanti da tre origini:

- `Eroi`
- `Presenze Luogo`
- `Globali`

### Eroi

Qui trovi i personaggi avventura già collegati alla campagna. Ogni eroe può entrare nel combattimento una sola volta.

### Presenze Luogo

Qui trovi i personaggi che sono già presenti nel luogo da cui nasce il combattimento. Il loro stato locale può essere riusato come base per lo scontro.

### Globali

Qui trovi schede base non già collegate come eroi dell’avventura.

Nel caso dei globali:

- i `Mostri` possono essere aggiunti più volte
- `Eroi` e `PNG` globali non possono essere aggiunti in duplicato come schede globali pure

## Controllo combattimento

Una volta iniziato lo scontro, il pannello `Controllo combattimento` resta fisso sopra la lista e contiene le azioni principali del round.

Le righe dei pulsanti sono:

1. `Aggiungi` e `Ordina`
2. `Avvia/Pausa` o `Riprendi` e `Fine`
3. `Prec.` e `Succ.`

In più, se esiste un ultimo attacco annullabile, compare anche il riquadro:

- `Annulla ultimo attacco`

## Lista partecipanti

La lista a sinistra è il cuore del tracking tattico.

Ogni riga chiusa mostra:

- posizione nel turno, per esempio `1/8`
- nome del partecipante
- fino a tre icone condizioni
- badge `Turno` se è il partecipante attivo
- CA
- PF
- PF temporanei
- iniziativa

Il partecipante di turno è evidenziato in modo molto più forte rispetto agli altri:

- fascia colorata laterale
- bordo accentuato
- fondo più caldo
- scroll automatico della lista per mantenerlo visibile

La riga usa anche effetti di impatto quando il partecipante:

- subisce danni
- viene ucciso
- viene ripristinato da un undo

## Menu contestuale sulla riga

Con il **tasto destro** sulla card del partecipante puoi aprire il menu contestuale.

Attualmente l’azione disponibile è:

- `Elimina`

## Espansione della riga partecipante

Cliccando sulla riga, il partecipante si espande e mostra i suoi controlli rapidi.

Nella parte espansa trovi:

- nome modificabile
- campi numerici rapidi:
  - iniziativa
  - PF
  - PF temporanei
  - CA
- pulsanti operativi
- blocco condizioni
- accesso ad abilità, speciali e incantesimi, se presenti

## Pulsanti rapidi della riga

Le azioni rapide possono includere:

- `Attacca`
- `Danni`
- `Cura`
- `TS`
- `Note DM`
- `Modifica`
- `Condizioni`

Alcuni pulsanti compaiono solo se hanno senso per quel partecipante.

## Attacca

`Attacca` apre un popover per selezionare:

- uno o più bersagli
- il danno da applicare

Il selettore bersagli usa una lista compatta con:

- nome
- CA
- PF
- condizioni

L’ordine dei bersagli non è casuale: DnDino prova a proporti prima i partecipanti più sensati in base a chi sta attaccando.

In generale:

- se attacca un **Eroe**, vengono proposti prima i **nemici**, poi gli alleati, poi i neutrali e infine i mostri fuori da quel contesto prioritario
- se attacca un partecipante non eroe, vengono proposti prima gli **eroi**, poi gli alleati, poi i neutrali e infine i nemici meno adatti

Dentro ogni gruppo, i nomi vengono poi ordinati alfabeticamente.

Il popover non pre-seleziona automaticamente un bersaglio: la scelta deve essere fatta manualmente.

Quando applichi un attacco a più bersagli:

- il danno viene applicato a tutti i selezionati
- il banner in alto mostra più righe, una per ogni bersaglio colpito
- l’undo dell’ultimo attacco conserva tutto il gruppo

## Danni e Cura

`Danni` applica danni diretti al partecipante.

`Cura` applica guarigione diretta.

## TS

`TS` apre il popover del **Tiro salvezza** basato sulle caratteristiche del partecipante.

## Condizioni

Il pulsante `Condizioni` apre il popover dedicato alla gestione degli stati attivi.

Da qui puoi:

- aggiungere condizioni
- scegliere durata e regole di scadenza
- collegare la fine di una condizione al turno di un altro partecipante

## Note DM

Il pulsante `Note DM` è sempre visibile.

Apre un popover modificabile in cui puoi scrivere note contestuali sul partecipante. Il contenuto viene salvato alla chiusura del popover.

## Modifica

`Modifica` apre il pannello editor del partecipante.

Serve quando hai bisogno di intervenire in modo più profondo su:

- iniziativa
- CA
- PF massimi, attuali e temporanei
- ruolo nel combattimento
- dati contestuali collegati

## Turno corrente

Quando il combattimento è attivo, il pannello centrale si concentra completamente sul partecipante di turno.

La card superiore mostra:

- immagine del partecipante
- nome
- sottotitolo
- CA
- PF
- PF temporanei
- iniziativa
- velocità
- ispirazione, se il partecipante è un eroe dell’avventura
- condizioni attive
- caratteristiche principali

## Pannelli centrali del turno

Sotto al riepilogo del turno compaiono solo i pannelli che hanno davvero contenuto.

Le sezioni possibili sono:

- `Attacchi`
- `Abilità speciali`
- `Abilità`
- `Descrizione`
- `Incantesimi`

Tutti questi pannelli sono collassabili.

Inoltre hanno un leggero accento visivo differenziato:

- `Attacchi` rosso
- `Abilità` giallo
- `Abilità speciali` verde
- `Incantesimi` celeste
- `Descrizione` grigio

## Attacchi e link interni

La sezione `Attacchi` è uno dei punti più forti del combattimento flat.

Se nella scheda base del personaggio hai preparato i link interni negli attacchi, durante il combattimento puoi usarli direttamente da qui.

In particolare, il link **Attacco completo** è molto utile perché:

- esegue tiro per colpire e danni nello stesso popover
- permette di selezionare uno o più bersagli
- propone automaticamente `Danno da applicare`
- ti lascia escludere singole righe danno se hai tirato più componenti e vuoi applicarne solo alcune
- chiude il popover appena applichi i danni

## Personaggi a 0 PF o meno

Nel combattimento i personaggi di tipo **Eroe** seguono una regola diversa da PNG e mostri.

### Eroi

Gli eroi possono scendere sotto `0` PF.

La regola è:

- tra `0` e `-(PF massimi - 1)` il personaggio è **Incosciente**
- a `-PF massimi` o meno il personaggio muore definitivamente

Quando un eroe è a `0` PF o meno ma non è morto in modo definitivo:

- resta nello scontro
- nel pannello centrale compare la card `Tiri salvezza contro la morte`

Questa card tiene traccia di:

- successi
- fallimenti

e permette di registrare rapidamente:

- `Successo`
- `Fallimento`

Se raggiunge 3 successi, il personaggio torna a `1` PF. Se raggiunge 3 fallimenti, muore.

### PNG e Mostri

Per i non eroi il comportamento è più semplice:

- a `0` PF o meno risultano morti

## Turni, round e partecipanti esclusi dal ciclo

Nel ciclo dei turni:

- gli eroi morti definitivamente vengono esclusi
- PNG e mostri a `0` PF o meno vengono esclusi

Questo significa che un eroe **Incosciente** può ancora avere un turno, proprio perché deve poter gestire i tiri salvezza contro la morte.

## Banner di impatto e feedback visivo

Quando un attacco va a segno, DnDino mostra un grande banner in alto con un riepilogo immediato.

Per esempio:

- chi colpisce
- chi viene colpito
- quanti danni sono stati applicati
- se il colpo ha ucciso il bersaglio

Se i bersagli sono più di uno, il banner mostra più righe nello stesso riquadro.

Anche la **Finestra Giocatori** può mostrare l’animazione del colpo, includendo tutti i bersagli coinvolti nello stesso attacco multi-target.

## Annulla ultimo attacco

Quando applichi un attacco, compare il pannello:

- `Annulla ultimo attacco`

Sotto al pulsante viene mostrato un piccolo riepilogo di quello che è successo.

Se l’ultimo attacco ha colpito più bersagli, il pannello mostra l’elenco completo delle righe che verranno ripristinate.

Quando confermi l’annullamento:

- i bersagli tornano allo stato precedente
- compare una notifica di ripristino
- anche il feedback visivo delle card viene aggiornato

## Riepilogo finale dello scontro

Quando termini il combattimento, il pannello centrale passa al **Riepilogo finale dello scontro** per il DM.

Questa schermata mostra:

- round totali
- durata
- nemici uccisi
- danni inflitti
- danni subiti

## Cosa viene sincronizzato alla fine

Quando chiudi il combattimento, DnDino salva il risultato sui record collegati.

Per gli eroi dell’avventura vengono sincronizzati:

- PF attuali
- PF temporanei
- condizioni manuali
- stato finale

Per le presenze del luogo con stato locale vengono sincronizzati:

- PF attuali
- PF temporanei
- condizioni manuali
- stato finale

Inoltre il combattimento aggiorna anche i dati collegati alla **sessione live**, compresi:

- danni inflitti
- danni subiti
- eroi caduti

## Quando il combattimento rende di più

Il combattimento di DnDino rende al massimo quando lo usi così:

1. prepari bene il pre-combattimento
2. usi il doppio schermo con la **Finestra Giocatori**
3. sfrutti i link negli `Attacchi` per mostri e PNG
4. tieni il DM sul tracker e i giocatori sulla presentazione

!!! tip
    Anche se il combattimento offre molte automazioni per tiri, attacchi completi e applicazione rapida dei danni, DnDino lascia comunque spazio a un uso più classico del dado. Puoi continuare a tirare fisicamente o gestire il lancio fuori dall’app e usare il combattimento soprattutto per applicare i valori in modo veloce e coerente, evitando solo la parte più scomoda: ricalcolare ogni volta a mano differenze e aggiornamenti dei punti ferita.
