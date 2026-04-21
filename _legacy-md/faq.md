# FAQ

Questa sezione raccoglie risposte rapide alle domande più comuni su DnDino.

Se hai bisogno di una spiegazione completa di una schermata specifica, ti conviene poi aprire anche la pagina dedicata della guida. La FAQ serve soprattutto per i casi pratici più frequenti.

## Come riprendo subito l'ultima campagna?

Apri la `Home` e usa la card dell'**ultima avventura**.

Da lì puoi:

- aprire direttamente la dashboard dell'avventura
- andare all'ultimo luogo visitato, se disponibile

È il modo più rapido per rientrare nel lavoro senza passare ogni volta dall'elenco completo delle avventure.

## Qual è la differenza tra scheda base, personaggio avventura, presenza luogo e partecipante al combattimento?

La **scheda base** è il record generale del personaggio o della creatura.

Da quella scheda possono nascere record contestuali separati:

- il **personaggio avventura**, usato dentro una campagna
- la **presenza luogo**, usata nei luoghi
- il **partecipante al combattimento**, usato nello scontro

Questo sistema serve per mantenere separati:

- nomi contestuali
- iniziativa
- PF correnti
- note operative
- stato locale del combattimento o del luogo

In altre parole, la scheda base resta il riferimento generale, mentre i record contestuali servono per lavorare in modo pratico durante la sessione.

## Come aggiungo un eroe all'avventura?

Apri la `Dashboard Avventura`, poi vai nel pannello `Personaggi`.

Da lì puoi:

- aggiungere un personaggio esistente
- creare un nuovo personaggio con `Crea personaggio`

Se crei un nuovo personaggio dal picker, al salvataggio torni al pannello di selezione e la lista si aggiorna subito.

## Come aggiungo una presenza a un luogo?

Apri il luogo e vai nel pannello `Presenze`.

Da lì puoi aggiungere:

- un eroe già collegato all'avventura
- un `PNG`
- un `Mostro`

Ricorda questa differenza importante:

- un `PNG` resta unico nel luogo
- un `Mostro` può essere aggiunto più volte

Questo permette di avere più istanze dello stesso mostro nello stesso luogo, ma evita duplicazioni non volute dei PNG.

## Posso cambiare il nome di un mostro senza modificare la scheda base?

Sì.

È proprio uno dei motivi per cui DnDino usa record contestuali.

Puoi rinominare un mostro:

- nel pre-combattimento
- nelle presenze dei luoghi
- in altri contesti locali dove il nome operativo deve essere più comodo da leggere

Questo non cambia il nome della scheda base originale.

## Come collego rapidamente un personaggio o un luogo dentro una descrizione?

Nei campi di testo che supportano i link interni usa il comando `Link`.

Da lì puoi creare collegamenti verso:

- personaggi
- luoghi
- incantesimi
- regole
- talenti

Questo è molto utile:

- nei `Luoghi`, per collegare altri luoghi o personaggi citati nella descrizione
- nei `Personaggi`, soprattutto in `Attacchi`, per collegare tiri o riferimenti utili

## A cosa servono i link negli Attacchi dei mostri?

Servono a trasformare un testo descrittivo in uno strumento operativo.

Nei campi rich text degli attacchi puoi inserire link come:

- `Attacco completo`
- `Tiro libero`
- `Tira Dadi`
- `Tiro per colpire`

Questo permette di:

- lanciare rapidamente i dadi
- applicare i danni ai bersagli
- collegare riferimenti ad altre voci dell'app

È uno dei modi più efficaci per rendere davvero utile la scheda di un mostro durante il combattimento.

## Sono obbligato a usare i tiri automatici del combattimento?

No.

DnDino offre molte automazioni, ma non ti obbliga a usarle.

Puoi continuare a:

- tirare i dadi fisicamente al tavolo
- leggere i risultati in modo tradizionale
- applicare i danni manualmente

L'app ti aiuta soprattutto a togliere il lavoro ripetitivo di aggiornamento dei PF e delle differenze matematiche.

## Il combattimento funziona bene anche con un solo monitor?

Sì.

Il `Combattimento Flat` funziona bene anche su schermo singolo.

Il doppio schermo con `Finestra Giocatori` dà il meglio in presentazione, ma non è un requisito. Su un solo monitor puoi usare il combattimento senza problemi e decidere dalle impostazioni come deve comportarsi la finestra giocatori.

## Posso decidere quante informazioni mostrare ai giocatori durante il combattimento?

Sì.

Nelle `Impostazioni > Combattimento` puoi controllare, tra le altre cose, se mostrare ai giocatori:

- round
- PF
- condizioni
- prossimo turno
- nome reale dei nemici
- dettagli di PNG e mostri

Questo ti permette di scegliere se vuoi un combattimento più trasparente oppure più “da DM screen”.

## Come funziona il riepilogo finale del combattimento?

Alla fine del combattimento DnDino chiude lo scontro e sincronizza i dati contestuali sui record collegati.

In più:

- il DM vede il riepilogo finale nel combattimento
- i giocatori possono vedere un riepilogo nella `Finestra Giocatori`, se l'opzione è attiva

Il riepilogo pubblico è centrato sui personaggi e non sui nemici.

## Cosa succede se un eroe scende sotto 0 PF?

Gli eroi possono andare in negativo.

La regola gestita dall'app è questa:

- tra `0` e `-(PF massimi - 1)` l'eroe è `Incosciente`
- a `-PF massimi` o meno l'eroe muore definitivamente

Nel combattimento, quando un eroe è incosciente, DnDino mostra anche il pannello per i **tiri salvezza contro la morte**.

## Come mostro un'immagine ai giocatori?

DnDino usa una finestra dedicata per la presentazione ai giocatori.

Puoi usarla:

- durante il combattimento
- nelle immagini dell'avventura
- in altri flussi che supportano la presentazione

Il comportamento della finestra si regola nelle `Impostazioni > Media` e, in parte, nelle `Impostazioni > Combattimento`.

## Come faccio backup dei dati?

Vai in `Impostazioni > Database`.

Da lì puoi:

- vedere dove si trovano i dati dell'app
- aprire la cartella dati
- aprire la cartella backup
- creare manualmente uno snapshot
- ripristinare uno snapshot
- ripristinare da iCloud, se configurato

Nella stessa sezione puoi anche decidere:

- frequenza dei backup automatici
- numero massimo di snapshot mantenuti

## Dove trovo informazioni tecniche sul database se qualcosa non torna?

Vai in `Impostazioni > Diagnostica`.

Lì puoi controllare:

- path del database
- presenza del file
- dimensione
- ultima modifica
- versione SQLite
- tabelle trovate e numero di record

È la sezione giusta da controllare se vuoi capire se un problema è solo visivo oppure riguarda davvero i dati salvati.

## Come contatto il supporto?

Apri `Impostazioni > Supporto`.

Da lì puoi:

- inviare una richiesta di supporto
- inviare un consiglio
- copiare l'email di riferimento

Usa `Supporto` quando qualcosa non funziona o non è chiaro. Usa `Consiglio` quando vuoi proporre un miglioramento o una nuova funzione.

!!! tip
    Se una risposta qui ti sembra troppo breve, usa la FAQ come punto di partenza e poi apri la pagina dedicata della guida, per esempio `Personaggi`, `Luoghi`, `Combattimento` o `Impostazioni`.
