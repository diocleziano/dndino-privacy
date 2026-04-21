# Impostazioni

La sezione **Impostazioni** raccoglie le preferenze globali di DnDino. Qui non si lavora su una singola avventura o su un singolo personaggio, ma si definisce **come deve comportarsi l'app nel suo insieme**.

Le impostazioni influenzano soprattutto:

- l'aspetto generale dell'interfaccia
- il comportamento della topbar
- il flusso di `Luoghi`
- il comportamento del `Combattimento`
- la gestione di immagini, backup e snapshot
- il supporto e la diagnostica del database

## Come è organizzata la schermata

La pagina è divisa in due aree:

- una **barra laterale sinistra** con le categorie
- un **pannello principale** a destra con le opzioni della sezione selezionata

Le categorie disponibili sono:

- `Generali`
- `Topbar`
- `Luoghi`
- `Combattimento`
- `Media`
- `Tema`
- `Database`
- `Diagnostica`
- `Supporto`
- `Licenze`

Questa struttura è utile perché separa bene le preferenze di uso quotidiano da quelle più tecniche, come backup e diagnostica.

## Generali

La sezione `Generali` raccoglie le preferenze di base dell'app.

### Profilo DM

Qui puoi personalizzare il tuo profilo con:

- `Nome utente`
- `Genere`

Il nome viene riutilizzato anche in altre parti dell'app, per esempio nel messaggio di benvenuto della `Home`.

### Lingua interfaccia

Puoi decidere se:

- seguire la lingua del sistema
- forzare una lingua specifica dell'app

Questa impostazione è utile soprattutto se vuoi usare DnDino in una lingua diversa da quella principale del Mac.

### Conferme globali

L'opzione `Chiedi conferma per le eliminazioni` aggiunge una conferma prima delle azioni distruttive, come rimozioni ed eliminazioni.

È una protezione utile soprattutto quando lavori rapidamente tra avventure, luoghi e combattimenti.

### Metadati

In `Generali` trovi anche:

- `Mostra metadati nell'app`

`Mostra metadati nell'app` decide se visualizzare o meno i pannelli metadati nelle schermate che li prevedono.

### Disposizione pannelli dashboard avventura

Questa parte è molto importante se usi spesso la `Dashboard Avventura`.

Puoi:

- trascinare i pannelli
- riordinarli all'interno della colonna sinistra o destra
- spostarli da una colonna all'altra

In questo modo la dashboard può essere adattata al tuo modo di lavorare. Per esempio puoi tenere più in alto i pannelli che usi più spesso durante la preparazione.

### Tema attivo

In `Generali` viene anche mostrato il **tema attualmente selezionato**, come riepilogo rapido. Il cambio vero e proprio del tema si fa nella sezione `Tema`.

### Guide introduttive

Da qui puoi ripristinare il comportamento di primo utilizzo dell'app.

Il pulsante `Ripristina Primo Utilizzo` fa in modo che DnDino consideri di nuovo come non ancora viste le guide contestuali e i percorsi introduttivi.

È utile se vuoi:

- rivedere alcune spiegazioni iniziali
- controllare come appare l'onboarding
- testare il comportamento dell'app come se fosse il primo avvio

## Topbar

La sezione `Topbar` definisce il comportamento degli strumenti rapidi presenti nella barra superiore dell'app.

### Aspetto topbar

Puoi scegliere se visualizzare la topbar:

- con sole icone
- oppure con icone e nome sotto

Questa preferenza cambia il livello di compattezza e leggibilità della barra.

### Dado predefinito

DnDino include un lanciadadi rapido nella topbar. Qui puoi scegliere il **tipo di dado predefinito** che viene proposto quando apri quel pannello.

È utile se nella tua campagna usi molto spesso un determinato dado e vuoi ridurre un clic ogni volta.

### Apertura rapida personaggi

Questa impostazione controlla il comportamento dell'apertura rapida dei personaggi dalla topbar.

Puoi decidere se l'apertura veloce deve portare:

- a una visualizzazione più orientata alla lettura
- oppure a una modalità più vicina alla modifica

L'obiettivo è adattare la scorciatoia al tuo uso più frequente.

### Apertura rapida regole

La topbar permette anche un'apertura veloce delle `Regole`.

Da qui puoi decidere se, quando usi quella scorciatoia, DnDino deve aprire:

- l'editor completo
- oppure una finestra più compatta e orientata alla consultazione

### Controlli finestra giocatori nella topbar

L'opzione `Mostra controlli finestra giocatori nella topbar` aggiunge nella barra superiore i controlli per aprire o chiudere manualmente la `Finestra Giocatori`.

Questa opzione è comoda soprattutto se:

- usi spesso il doppio schermo
- vuoi controllare rapidamente la finestra giocatori senza passare da altri pannelli

## Luoghi

La sezione `Luoghi` contiene le preferenze globali che vengono usate come comportamento di default nella dashboard dei luoghi.

### Ruolo presenza predefinito

Quando aggiungi una presenza a un luogo, DnDino può proporre un ruolo iniziale predefinito.

Questa impostazione è utile se, nel tuo stile di lavoro, la maggior parte delle nuove presenze parte con lo stesso tipo di ruolo.

### Mostra mappe dei luoghi padre di default

Se attivi questa opzione, nella schermata `Luoghi` le mappe ereditate dai luoghi padre partono già visibili.

È particolarmente utile nelle avventure con una gerarchia forte di aree e sottoluoghi.

### Ricorda ultimo luogo visitato

Se attivo, quando rientri nella schermata `Luoghi` l'app prova a ripristinare l'ultimo luogo selezionato per quell'avventura.

Questa preferenza rende più rapido riprendere il lavoro da dove eri rimasto.

### Chiudi automaticamente il luogo precedente

Questa impostazione si applica durante una **sessione live attiva**.

Quando un luogo viene segnato `In visita`, il luogo che era prima `In visita` viene marcato automaticamente come `Visitato`.

È utile se vuoi che l'avanzamento dell'esplorazione si mantenga coerente senza dover chiudere manualmente il luogo precedente ogni volta.

## Combattimento

La sezione `Combattimento` raccoglie le preferenze globali del sistema di combattimento.

Qui trovi sia opzioni di presentazione, sia scelte che influenzano il flusso pratico dello scontro e della `Finestra Giocatori`.

## Ordine pannelli centrali

Puoi anche riordinare l'ordine dei pannelli centrali del combattimento, trascinando elementi come:

- `Attacchi`
- `Abilità speciali`
- `Abilità`
- `Incantesimi`
- `Descrizione`

Questo permette di adattare il pannello centrale a ciò che vuoi avere più in alto durante il turno.

## Presentazione combattimento

Questa sottosezione controlla il comportamento generale del combattimento e della presentazione ai giocatori.

### Mostra turno ai giocatori di default

Se attivo, i nuovi combattimenti partono già con la presentazione automatica del turno abilitata.

### Apri la finestra giocatori anche con un solo monitor

Questa preferenza controlla il comportamento automatico della `Finestra Giocatori` nei setup a schermo singolo.

Se la disattivi:

- su un solo monitor la finestra non si apre automaticamente
- ma se è già aperta continua comunque ad aggiornarsi

### Mostra automaticamente il dettaglio del giocatore di turno

Quando il turno cambia, l'app può:

- selezionare automaticamente il partecipante attivo
- aprirne anche il dettaglio

È utile se vuoi che la schermata segua da sola l'azione del turno.

### Ordina automaticamente per iniziativa all'avvio

Quando premi `Avvia combattimento`, DnDino può riordinare automaticamente i partecipanti in base all'iniziativa prima di iniziare il round.

Questa opzione è molto comoda se vuoi evitare un passaggio manuale nel pre-combattimento.

### Chiedi conferma prima di terminare il combattimento

Questa opzione è importante perché la fine del combattimento non è solo una chiusura visiva:

- sincronizza PF e stato sui record collegati
- chiude il flusso dello scontro

La conferma aiuta a evitare chiusure accidentali.

### Mostra intro combattimento ai giocatori

Se attiva, quando il combattimento parte la `Finestra Giocatori` mostra una breve introduzione con i partecipanti allo scontro.

### Mostra riepilogo finale ai giocatori

Se attiva, alla fine dello scontro la `Finestra Giocatori` mostra un riepilogo finale con i dati principali dei personaggi.

## Informazioni partecipante attivo

Questa sottosezione decide quali informazioni del turno corrente mostrare ai giocatori.

Puoi scegliere se rendere visibili:

- `Round`
- `PF`
- `Condizioni`
- `Prossimo turno`

Queste opzioni sono utili per dosare quante informazioni condividere durante la presentazione del turno.

## Informazioni nemici e PNG

Questa parte gestisce separatamente ciò che i giocatori vedono quando il partecipante attivo è un:

- nemico
- mostro
- PNG

Puoi controllare in modo indipendente:

- visibilità di PF e PF temporanei
- visibilità delle condizioni
- visibilità del nome reale del nemico

Se disattivi il nome dei nemici, DnDino li mostra con un nome generico.

Questo è molto utile per mantenere il giusto equilibrio tra chiarezza e segretezza al tavolo.

## Media

La sezione `Media` raccoglie le preferenze per la gestione delle immagini e della finestra di presentazione.

### Immagini giocatori a tutto schermo

Se attivo, le immagini mostrate ai giocatori vengono aperte in modalità fullscreen.

### Immagini DM sul monitor principale

Questa opzione fa sì che la finestra del DM venga aperta di default sul primo schermo disponibile, invece di seguire altre logiche di monitor secondario.

### Ricorda dimensione finestra DM

Se attivo, quando riapri una nuova immagine per il DM la finestra mantiene:

- ultima dimensione
- ultima posizione

È una preferenza utile se lavori sempre con un assetto fisso di schermi e finestre.

## Manutenzione media

La sezione `Manutenzione media` serve per il lato più tecnico della gestione immagini.

Da qui puoi lanciare `Ripulisci media inutilizzati`, che controlla i file immagine salvati dall'app e rimuove quelli che non risultano più collegati ad alcuna entità.

Questa funzione è utile per:

- liberare spazio
- ripulire file residui
- mantenere ordinata la cartella dati

## Tema

La sezione `Tema` permette di scegliere la **palette globale** dell'app.

Ogni tema mostra una piccola anteprima visiva con i colori principali, così puoi capire subito come cambierà l'aspetto generale dell'interfaccia.

Il tema selezionato si applica in modo trasversale alle varie sezioni dell'app.

## Database

La sezione `Database` è una delle più importanti per la sicurezza dei dati.

Qui trovi:

- il percorso della cartella dati
- il percorso del database SQLite
- il percorso della cartella backup
- informazioni sugli snapshot più recenti

Questa sezione è utile sia per uso quotidiano sia per interventi di manutenzione o recupero dati.

### Backup automatico

Puoi scegliere:

- la frequenza del backup automatico
- il numero massimo di snapshot automatici da mantenere

Questo permette di trovare un equilibrio tra sicurezza e quantità di copie conservate.

### Snapshot cloud

DnDino gestisce anche la modalità degli snapshot cloud.

Da qui puoi scegliere il comportamento relativo ai salvataggi cloud e vedere lo stato corrente tramite il testo di riepilogo mostrato nella schermata.

### Azioni principali

Nel pannello `Database` trovi i pulsanti più importanti di manutenzione:

- `Apri cartella dati`
- `Apri cartella backup`
- `Crea snapshot...`
- `Ripristina snapshot...`
- `Ripristina da iCloud`

Queste azioni coprono il ciclo completo di salvataggio e recupero.

### Reimpostazione applicazione

La funzione `Reimposta dati applicazione` cancella:

- database dell'app
- media dell'app

ma mantiene i backup già creati.

È una funzione drastica, pensata soprattutto per:

- ripartenze pulite
- test
- recuperi dopo problemi gravi

### Ultimi snapshot

Nella parte bassa della sezione `Database` viene mostrato anche l'elenco degli ultimi snapshot trovati.

Per ciascuno vengono mostrati:

- nome file
- data
- dimensione

Questo aiuta a controllare rapidamente se il sistema di snapshot sta lavorando come previsto.

## Diagnostica

La sezione `Diagnostica` serve a controllare lo stato tecnico del database SQLite usato dall'app.

Qui puoi:

- aggiornare i dati diagnostici
- vedere il path del database
- controllare se il file esiste
- verificarne dimensione e data di modifica
- vedere la versione SQLite

### Tabelle

La diagnostica mostra anche l'elenco delle tabelle trovate nel database, insieme al numero di record presenti in ciascuna.

Questa sezione è particolarmente utile quando:

- stai controllando un problema tecnico
- vuoi verificare che il database sia stato creato correttamente
- devi capire se alcuni dati sono realmente presenti

## Supporto

La sezione `Supporto` raccoglie i canali rapidi per contattare chi sviluppa l'app.

Qui trovi:

- l'email di supporto
- il pulsante `Richiedi supporto`
- il pulsante `Invia un consiglio`
- il pulsante `Copia email`

Questa sezione è pensata per due casi diversi:

- problemi, bug o dubbi da chiarire
- suggerimenti per miglioramenti o nuove funzioni

## Licenze

La sezione `Licenze` raccoglie i riferimenti legali e di attribuzione usati dall'app.

Attualmente include in particolare la parte relativa al materiale del **System Reference Document 5.2** di Dungeons & Dragons, con i relativi riferimenti:

- al documento SRD
- alla licenza `CC-BY-4.0`

Questa sezione è soprattutto informativa, ma utile se vuoi sapere con precisione da quali riferimenti regolistici deriva una parte compatibile dell'app.

!!! tip
    Se stai configurando DnDino per la prima volta, le sezioni più utili da controllare subito sono `Generali`, `Topbar`, `Combattimento` e `Database`. In genere sono quelle che incidono di più sull'uso quotidiano e sulla sicurezza dei dati.
