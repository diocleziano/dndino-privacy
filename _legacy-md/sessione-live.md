# Sessione live

La **Sessione live** è il contesto operativo della partita in corso. Non è semplicemente un timer, ma un sistema che tiene insieme:

- il tempo di gioco della sessione
- la timeline degli eventi importanti
- le note DM rapide
- lo stato dei luoghi visitati
- le quest attive o completate
- i combattimenti svolti
- le statistiche aggregate della sessione

In pratica, quando una sessione live è attiva, DnDino sa qual è la campagna “in corso” e usa questo contesto per collegare tra loro varie parti dell’app.

## A cosa serve

La sessione live è utile quando vuoi usare DnDino durante una sessione reale al tavolo, non solo in preparazione.

Serve per:

- tenere traccia del tempo della sessione
- avere una timeline ordinata degli eventi principali
- annotare rapidamente informazioni del DM
- segnare luoghi in visita o visitati
- vedere un riepilogo dinamico della sessione
- raccogliere automaticamente i dati provenienti dal combattimento

## Dove si avvia

La sessione live si avvia dalla **dashboard dell’avventura**, nel pannello `Sessione Live`.

Se non esiste una sessione attiva, il pannello mostra:

- stato pronto
- pulsante `Avvia Sessione Live`

Quando premi il pulsante, DnDino crea una nuova sessione di tipo live e la imposta come sessione globale attiva.

## Una sola sessione live alla volta

DnDino gestisce una sola sessione live attiva per volta.

Se una sessione è già aperta in un’altra avventura:

- la nuova avventura non può avviarne una seconda
- la dashboard mostra un avviso che segnala che la sessione attiva appartiene a un’altra campagna

Questo evita di mischiare timeline, eventi e statistiche tra campagne diverse.

## Cosa succede quando una sessione live è attiva

Quando una sessione live è in corso:

- la barra superiore mostra il suo stato
- il timer continua ad aggiornarsi
- i luoghi seguono questo contesto
- la timeline inizia a raccogliere eventi
- anche il combattimento può inviare dati alla sessione

La sessione live diventa quindi il filo conduttore della partita in corso.

## Stato della sessione

La sessione live può trovarsi in tre stati:

- attiva
- in pausa
- interrotta

### Attiva

È lo stato normale mentre la sessione è in corso. Il timer continua a scorrere e gli eventi vengono registrati con il tempo trascorso corretto.

### In pausa

La sessione può essere messa in pausa dalla dashboard avventura o dalla barra superiore.

Quando è in pausa:

- il timer si ferma
- la sessione resta comunque aperta
- può essere ripresa in un secondo momento

### Interrotta

Se l’app viene chiusa mentre la sessione è ancora attiva, DnDino la riapre come `interrotta` al successivo avvio e registra un evento dedicato nella timeline.

Questo permette di:

- non perdere la sessione
- capire che si è verificata un’interruzione
- riprendere manualmente il lavoro

## Il pannello Sessione Live nella dashboard avventura

Nella dashboard dell’avventura il pannello mostra lo stato corrente della sessione.

Se la sessione appartiene all’avventura aperta, il pannello mostra:

- titolo della sessione
- timer in tempo reale
- stato (`In corso` oppure `In pausa`)
- indicazione che il player è globale
- pulsanti:
  - `Pausa` o `Riprendi`
  - `Chiudi e salva`

Se invece non c’è una sessione live attiva:

- compare il pulsante `Avvia Sessione Live`

Se una sessione è attiva ma appartiene a un’altra avventura:

- il pannello mostra che la sessione live è occupata altrove

## La sessione live nella topbar

Quando una sessione live è attiva, la barra superiore dell’app mostra un indicatore dedicato.

Questo elemento contiene:

- titolo della sessione
- timer
- indicatore di stato

Cliccandolo si apre un popover di controllo rapido.

## Il popover della sessione live nella topbar

Dal popover della topbar puoi fare operazioni molto veloci senza lasciare la schermata attuale.

Qui trovi:

- `Pausa` oppure `Riprendi`
- `Chiudi e salva`
- editor rapido per `Nota DM`
- timeline della sessione
- azioni rapide sul luogo attualmente in visita
- riepilogo live compatto

Questa parte è molto utile quando vuoi lavorare in altre sezioni dell’app ma tenere sempre sotto controllo la sessione attiva.

## Nota DM rapida

Nel popover della sessione live puoi scrivere una **Nota DM** e aggiungerla subito alla timeline.

Questo è utile per annotare al volo:

- decisioni dei giocatori
- spunti narrativi
- conseguenze da ricordare
- idee improvvisate emerse durante la partita

Le note DM vengono registrate come eventi della timeline.

## Timeline della sessione

La timeline è il registro cronologico della sessione live.

Ogni evento memorizza:

- titolo
- dettaglio
- momento della sessione in cui è avvenuto

La timeline può contenere eventi di sistema e note DM.

## Tipi di eventi registrati

Gli eventi più importanti che DnDino registra automaticamente includono:

- `Sessione avviata`
- `Sessione in pausa`
- `Sessione ripresa`
- `Sessione interrotta per chiusura app`
- `Entrata nel luogo`
- `Uscita dal luogo`
- `Stato luogo aggiornato`
- `Quest attivata`
- `Quest completata`
- `Combattimento iniziato`
- `Combattimento finito`
- `Danno inflitto in combattimento`
- `Danno subito in combattimento`
- `Nota DM`

Questo rende la sessione live molto utile anche come memoria rapida di ciò che è successo davvero al tavolo.

## Collegamento con i luoghi

La sessione live è collegata direttamente ai luoghi dell’avventura attiva.

Quando aggiorni un luogo all’interno del contesto della sessione:

- il cambio di stato viene registrato
- la timeline si aggiorna
- il riepilogo live cambia di conseguenza

I dati più importanti tracciati dal lato luoghi sono:

- luoghi in visita
- luoghi visitati
- quest attive
- quest completate

## Chiusura automatica del luogo precedente in visita

Nelle impostazioni esiste anche una logica collegata alla sessione live: quando un luogo viene messo `In visita`, il luogo che era prima in visita può essere segnato automaticamente come `Visitato`.

Questa funzione vale solo quando esiste una sessione live attiva ed è molto utile per mantenere coerente il tracciamento dell’esplorazione.

## Riepilogo live

Il riepilogo live aggrega i dati più importanti raccolti durante la sessione.

Tra i valori principali ci sono:

- luoghi visitati
- luoghi in visita
- quest attive
- quest completate
- combattimenti svolti
- nemici sconfitti
- eroi caduti
- durata totale dei combattimenti

La sessione live tiene anche due riepiloghi molto utili per i personaggi:

- danni inflitti dagli eroi
- danni subiti dagli eroi

## Integrazione con il combattimento

La sessione live e il combattimento sono strettamente collegati.

Quando avvii un combattimento durante una sessione live, DnDino registra:

- `Combattimento iniziato`

Durante il combattimento può registrare:

- `Danno inflitto in combattimento`
- `Danno subito in combattimento`

Quando chiudi il combattimento registra:

- `Combattimento finito`
- durata dello scontro
- nemici sconfitti
- eroi caduti

Questo significa che la sessione live riceve automaticamente i dati più importanti del combattimento senza bisogno di reinserirli a mano.

## Danni inflitti e danni subiti

La sessione live traccia i danni con due classifiche separate:

- `Danni inflitti dai personaggi`
- `Danni subiti dai personaggi`

Il conteggio è pensato solo per gli eroi dell’avventura, non per tutti i partecipanti dello scontro.

Questo rende il riepilogo più utile per leggere l’andamento della sessione dal punto di vista del party.

## Eroi caduti

Quando un combattimento termina, il riepilogo della sessione live può incrementare anche il conteggio degli **eroi caduti**.

Questo dato viene alimentato direttamente dal risultato finale del combattimento.

## Sessione live e Finestra Giocatori

La sessione live non coincide con la **Finestra Giocatori**, ma le due cose sono collegate.

La sessione live fornisce il contesto generale della partita, mentre la finestra giocatori è il canale di presentazione visiva.

In particolare:

- durante il combattimento la finestra giocatori può mostrare intro, turno corrente e riepilogo finale
- fuori dal combattimento, la finestra giocatori può comunque essere usata per mostrare immagini e contenuti del contesto attivo

## Chiusura e salvataggio

Quando scegli `Chiudi e salva`, DnDino:

- finalizza la sessione
- salva i dati raccolti
- persiste la timeline nella sessione collegata all’avventura
- chiude il contesto live globale

Dopo la chiusura, la sessione resta consultabile come sessione salvata.

## Visualizzazione della sessione salvata

Una sessione live già conclusa può essere riaperta come dettaglio.

Nel pannello di dettaglio trovi:

- riepilogo e timeline
- durata registrata
- luoghi visitati
- combattimenti svolti
- nemici sconfitti
- eroi caduti
- classifiche di danni inflitti e subiti dai personaggi

Questa visualizzazione è utile sia come archivio della campagna sia come base per scrivere un resoconto più narrativo.

## Quando conviene usare la sessione live

La sessione live è particolarmente utile quando vuoi:

- tenere DnDino aperto durante la partita
- segnare rapidamente cosa succede davvero al tavolo
- sapere quali luoghi sono stati visitati
- avere una timeline ordinata degli eventi chiave
- far confluire automaticamente il combattimento nel riepilogo della sessione

## In pratica

La sessione live è il ponte tra:

- preparazione
- gestione operativa della partita
- memoria finale della sessione

Se usata bene, riduce molto il rischio di perdere informazioni importanti durante il gioco e rende più semplice ricostruire dopo cosa è successo davvero nella campagna.
