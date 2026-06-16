# Combattimento e tavolo

DnDino Hero è pensata per accompagnare il giocatore durante la sessione.

La scheda resta utilizzabile anche senza DnDino, ma alcune funzioni sono predisposte per il gioco locale al tavolo.

## Durante il combattimento

La sezione **Combattimento** raccoglie le informazioni che servono più spesso:

- punti ferita
- PF temporanei
- classe armatura
- iniziativa
- velocità
- ispirazione eroica
- condizioni
- tiri salvezza
- attacchi
- incantesimi preparati
- slot incantesimo
- privilegi e risorse consumabili
- tiri salvezza contro la morte, quando il personaggio è a 0 PF

## Attacchi

Gli attacchi sono pensati per le armi.

Ogni attacco può avere:

- nome
- icona
- proprietà
- padronanza
- competenza
- caratteristica usata per colpire
- bonus al tiro per colpire
- danno principale
- danni aggiuntivi
- bonus ai danni
- progressioni di classe usate nei danni o nei bonus
- eventuali danni aggiuntivi con tipo di danno separato

La visualizzazione mostra il bonus totale e una sintesi dei modificatori che lo compongono.

Se l'arma ha una padronanza attiva, la scheda mostra la padronanza in modo compatto. La descrizione completa può essere consultata senza riempire tutta la card dell'attacco.

## Incantesimi

Gli incantesimi associati al personaggio sono organizzati per livello.

I trucchetti sono sempre disponibili. Gli altri incantesimi possono essere marcati come:

- **Preparato**
- **Non Preparato**

Nella scheda generale e in combattimento vengono mostrati solo gli incantesimi preparati.

## Slot incantesimo

Gli slot sono separati per classe o sottoclasse quando più origini forniscono magia.

Per ogni origine vengono mostrati:

- caratteristica da incantatore
- bonus attacco con incantesimo
- CD tiro salvezza incantesimo
- slot totali
- slot spesi

Gli slot si ripristinano con il riposo lungo.

## Condizioni

Le condizioni sono gestite manualmente.

L'app importa la lista delle condizioni da DnDino, ma non applica automaticamente logiche di rimozione o effetti meccanici. Questo lascia il controllo al giocatore e al master.

## Collegamento locale con DnDino

La comunicazione con DnDino è pensata per rimanere locale.

Il master avvia il collegamento dalla sezione dell'avventura in DnDino. Hero cerca la sessione sulla rete locale, mostra master e avventura trovati e permette di inviare il personaggio attivo.

Al primo collegamento DnDino può chiedere conferma:

- per autorizzare il dispositivo
- per importare il personaggio come nuovo
- per associarlo a un personaggio già esistente

L'associazione usa identificativi interni, non solo il nome del personaggio. Questo evita problemi se il nome viene modificato in seguito.

Quando il collegamento è già stato autorizzato, Hero prova a riconnettersi automaticamente quando torna in primo piano. La hero della scheda mostra anche l'ultimo DnDino collegato, così puoi ricollegarti più rapidamente.

## Sincronizzazione durante il gioco

La sincronizzazione può essere bidirezionale.

Hero può inviare a DnDino:

- PF attuali, massimi e temporanei
- classe armatura
- condizioni
- dadi vita spesi
- ispirazione eroica

DnDino può aggiornare Hero con gli stessi dati. Se è attivo un combattimento, DnDino considera il personaggio del combattimento come sorgente operativa. Quando Hero si riconnette, DnDino invia lo stato attuale del personaggio collegato.

Le notifiche di Hero cercano di descrivere cosa è successo:

- danni subiti
- cure ricevute
- PF temporanei aggiornati
- ispirazione eroica ricevuta o rimossa
- condizioni applicate
- scheda aggiornata

## Chat privata

La sezione **Messaggio privato al DM** appare quando Hero è collegato.

Da qui il giocatore può scrivere al DM. Su DnDino il master riceve una notifica e può aprire la conversazione. La chat resta distinta per personaggio e dispositivo, così due dispositivi con lo stesso account possono usare conversazioni diverse.
