# Sessione live

La **Sessione live** è il contesto operativo della partita in corso. Non è semplicemente un timer, ma un sistema che tiene insieme:

- il tempo di gioco della sessione
- la timeline degli eventi importanti
- le note DM rapide
- lo stato dei luoghi visitati
- le quest attive o completate
- i combattimenti svolti
- le statistiche aggregate della sessione

In pratica, quando una sessione live è attiva, DnDino sa qual è la campagna in corso e usa questo contesto per collegare tra loro varie parti dell’app.

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

La sessione live si avvia dal controllo al centro della **topbar** quando sei dentro una pagina dell'avventura, per esempio dashboard, luoghi o combattimenti.

Se non esiste una sessione attiva, il controllo mostra l'azione di avvio. Quando la premi, DnDino chiede conferma e poi crea una nuova sessione live per l'avventura corrente.

Questo evita di dover tornare alla dashboard solo per avviare la sessione: il comando resta nel punto più comodo mentre lavori nei luoghi o prepari un combattimento.

## Una sola sessione live alla volta

DnDino gestisce una sola sessione live attiva per volta.

Se una sessione è già aperta in un’altra avventura:

- la nuova avventura non può avviarne una seconda
- la dashboard mostra un avviso che segnala che la sessione attiva appartiene a un’altra campagna

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

## Controllo Sessione Live nella topbar

Nelle pagine dell'avventura, la topbar mostra il controllo della sessione live al centro.

Se la sessione appartiene all’avventura aperta, il controllo mostra:

- titolo della sessione
- timer in tempo reale
- stato (`In corso` oppure `In pausa`)

Se invece non c’è una sessione live attiva:

- compare il comando per avviare la sessione live dell'avventura corrente

Se una sessione è attiva ma appartiene a un’altra avventura:

- il controllo segnala che la sessione live è in uso altrove

## La sessione live nella topbar

Quando una sessione live è attiva, la topbar mostra un controllo dedicato con stato e timer. La descrizione completa della topbar è nella pagina `Topbar`.

![Sessione live attiva nella topbar](../images/en_sessionelive_attiva_topbar.png){ .img-shot }

## Il pannello rapido della sessione live

Dal pannello rapido della sessione puoi fare operazioni molto veloci senza lasciare la schermata attuale.

Qui trovi:

- `Pausa` oppure `Riprendi`
- `Chiudi e salva`
- editor rapido per `Nota DM`
- timeline della sessione
- azioni rapide sul luogo attualmente in visita
- riepilogo live compatto

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
- `Nota DM`

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

## Ricreare una sessione live già giocata

Se durante una partita hai dimenticato di avviare la sessione live, puoi ricrearla manualmente dalla card **Sessioni** della dashboard avventura.

La sessione ricreata non è una semplice nota: viene salvata come sessione live e usa i dati reali già presenti nell'avventura.

Quando la crei puoi indicare:

- ora di inizio e ora di fine
- luoghi visitati durante la sessione
- note della sessione

DnDino include automaticamente i combattimenti completati e avviati nell'intervallo selezionato. In questo modo le statistiche della sessione possono usare danni, nemici sconfitti, durata degli scontri e tempi medi dei turni già registrati dai combattimenti reali.

Questa funzione è pensata per recuperare una sessione giocata senza perdere il valore delle statistiche.

## Eliminare una sessione

Nella lista delle sessioni, ogni riga ha un pulsante di eliminazione. Prima della cancellazione DnDino mostra una conferma, perché l'operazione rimuove definitivamente la sessione salvata.

## Riepilogo live

![Riepilogo sessione live](../images/en_sessionelive_riepilogo_1.png){ .img-shot }
![Grafici sessione live](../images/en_sessionelive_riepilogo_2.png){ .img-shot }


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
- tempo medio dei turni, quando arriva dai combattimenti conclusi

## Integrazione con il combattimento

La sessione live e il combattimento sono strettamente collegati.

Quando avvii un combattimento durante una sessione live, DnDino registra:

- `Combattimento iniziato`

Durante il combattimento può registrare:

- i dati aggregati utili al riepilogo e alle statistiche

Quando chiudi il combattimento registra:

- `Combattimento finito`
- durata dello scontro
- nemici sconfitti
- eroi caduti

## Danni inflitti e danni subiti

La sessione live traccia i danni con due classifiche separate:

- `Danni inflitti dai personaggi`
- `Danni subiti dai personaggi`

Il conteggio è pensato solo per gli eroi dell’avventura, non per tutti i partecipanti dello scontro.

Nel dettaglio della sessione salvata possono comparire anche grafici dedicati ai combattimenti conclusi durante quella sessione:

- danni inflitti per combattimento
- danni subiti per combattimento
- tempo medio dei turni per combattimento

Ogni combattimento resta sull'asse orizzontale in ordine cronologico. I personaggi che hanno partecipato vengono mostrati anche quando in uno scontro hanno fatto o subito `0` danni, così la lettura della serie resta coerente. Se un personaggio non partecipa a un combattimento, invece, non viene inserito in quel punto.

Questi grafici servono a capire chi ha inciso di più durante la sessione e chi ha assorbito più danni nel corso degli scontri.

Il grafico dei turni aiuta invece a capire quanto tempo richiedono in media gli eroi e il DM durante gli scontri della sessione.

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
- grafici dei danni inflitti e subiti nei combattimenti della sessione
- grafico del tempo medio dei turni, se disponibile

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
