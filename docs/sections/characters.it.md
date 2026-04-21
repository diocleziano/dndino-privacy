# Eroi, PNG e Mostri

La sezione **Eroi, PNG e Mostri** raccoglie tutte le schede base dei personaggi dell’app. È il punto in cui si creano, si modificano e si clonano i record che poi possono essere collegati alle avventure, ai luoghi e ai combattimenti.

Questa pagina è importante perché in DnDino esistono **più livelli di personaggio**, ognuno con uno scopo diverso:

- la **scheda base**
- il **personaggio avventura**
- la **presenza nel luogo**
- il **partecipante al combattimento**

Non sono duplicazioni inutili: servono per mantenere **dati contestuali separati**, come nome visualizzato, punti ferita, condizioni, iniziativa e note DM, senza perdere il collegamento con la scheda originale.

## Scheda base

La **scheda base** è il record principale salvato nella sezione `Eroi, PNG e Mostri`.

Qui definisci tutto ciò che appartiene al personaggio in modo generale:

- nome
- tipo: `Eroe`, `PNG` o `Mostro`
- razza, classe, taglia, allineamento
- caratteristiche
- CA, PF massimi, velocità, iniziativa
- descrizione, abilità, attacchi
- immagini collegate
- incantesimi collegati
- equipaggiamento e altri dati di riferimento

La scheda base non rappresenta automaticamente un personaggio “presente” in un’avventura, in un luogo o in un combattimento. È il modello da cui partono i livelli successivi.

## Creare, modificare e clonare un personaggio

Per creare una nuova scheda:

1. apri la sezione `Eroi, PNG e Mostri`
2. premi il pulsante di aggiunta
3. compila il form del personaggio
4. salva il record

Nel form puoi creare:

- eroi
- PNG
- mostri

Il tipo scelto influenza campi e comportamenti nelle sezioni successive. Per esempio:

- per gli **eroi** hanno senso presenza in avventura, ispirazione e stato contestuale
- per i **mostri** diventano più rilevanti GS, attacchi e uso multiplo nei contesti operativi

Aprendo una scheda esistente puoi modificarla in ogni sua parte. Le modifiche fatte qui aggiornano il record sorgente, ma non sovrascrivono sempre automaticamente tutti i dati contestuali già creati in avventura, nei luoghi o nel combattimento. Questo è voluto.

La **clonazione** crea una nuova scheda base partendo da una già esistente, copiando anche elementi collegati come:

- campi della scheda
- incantesimi collegati
- attacchi strutturati
- immagini collegate

È utile soprattutto per:

- creare varianti simili dello stesso mostro
- partire da un PNG già impostato
- costruire rapidamente più schede con struttura simile

## Link interni nei testi del personaggio

Una delle funzioni più utili della scheda base, soprattutto per **PNG** e **Mostri**, è il sistema dei **link interni** nei campi rich text.

Questa funzione è particolarmente preziosa nella sezione **Attacchi**, perché ti permette di trasformare il testo descrittivo in strumenti operativi pronti da usare durante la sessione e nel combattimento.

In pratica puoi inserire link che aprono direttamente:

- un tiro di dado
- un tiro per colpire
- un attacco completo con danni
- un personaggio
- un luogo
- un incantesimo
- un talento
- una regola del glossario

## Dove conviene usarli

I link interni sono particolarmente utili nei campi rich text della scheda, per esempio:

- `Attacchi`
- `Abilità speciali`
- `Descrizione`
- altri campi descrittivi in cui vuoi inserire riferimenti rapidi

Il caso più utile in assoluto resta però **Attacchi**, perché ti permette di rendere immediatamente cliccabili:

- il tiro per colpire
- i dadi danno
- un attacco completo già pronto

Per i mostri è molto comodo, perché riduce il tempo speso a leggere formule o ricostruire ogni volta i tiri a mano.

## Come si inserisce un link

Il flusso corretto è questo:

1. apri un campo rich text della scheda
2. seleziona il testo che vuoi trasformare in link, oppure posiziona il cursore dove vuoi inserirlo
3. premi il pulsante `Link`
4. scegli il tipo di collegamento dal picker
5. conferma la creazione del link

In base al testo selezionato, il picker può proporti alcuni link automatici già pronti.

## I quattro link più utili per i lanci

### Tiro libero

`Tiro libero` è il link più flessibile. È sempre disponibile nel picker e serve quando vuoi creare un lancio configurabile senza dover rispettare una struttura rigida.

È utile per:

- una formula completa come `1d6+3`
- un semplice dado come `1d20`
- una formula che vuoi poi modificare al volo prima del lancio

### Tira Dadi

`Tira Dadi` compare solo se il testo selezionato è una **formula dadi valida**.

Esempi validi:

- `1d6`
- `2d8+4`
- `4d4 + 1`

Questo link è ideale per danni singoli, dadi di guarigione, effetti casuali e lanci rapidi separati.

### Tiro per colpire

`Tiro per colpire` compare solo se il testo selezionato è un **modificatore valido**, non una formula completa `1d20`.

Esempi validi:

- `+5`
- `-1`
- `0`
- `2`

Quando crei questo link, DnDino sa che deve eseguire un **1d20** usando quel modificatore. È quindi perfetto quando negli attacchi vuoi scrivere qualcosa di leggibile, per esempio:

- `Morso +6`
- `Artigli +4`

### Tiro per colpire e danni

`Tiro per colpire e danni` è il link più potente per la sezione **Attacchi**.

È sempre disponibile nel picker e apre un configuratore dedicato in cui puoi impostare:

- modificatore al tiro per colpire
- eventuale soglia di critico
- fino a tre formule danno
- titolo dei singoli danni

È il modo migliore per costruire un attacco completo da mostro o PNG, perché in un solo link puoi concentrare:

- il tiro per colpire
- i danni principali
- eventuali danni secondari
- eventuali danni aggiuntivi

Nel combattimento questo link è particolarmente utile, perché il popover collegato può essere usato anche per applicare i danni ai bersagli.

## Esempio pratico per Attacchi

Un modo molto efficace di scrivere un attacco di mostro è usare testo leggibile per il DM e link cliccabili solo nei punti utili.

Per esempio:

- `Morso +6, portata 1,5 m, un bersaglio. Colpisce: 1d8+4 perforanti.`

Poi puoi trasformare:

- `+6` in `Tiro per colpire`
- `1d8+4` in `Tira Dadi`

oppure creare direttamente un solo link `Tiro per colpire e danni` sul nome dell’attacco o su una parte del testo.

## Collegare luoghi, personaggi e altri riferimenti

Il sistema di link non serve solo per i tiri. Nei campi descrittivi puoi anche creare collegamenti verso altri contenuti dell’app, per esempio:

- un `Luogo`
- un altro `Personaggio`
- un `Incantesimo`
- un `Talento`
- una `Regola`

Questo è molto utile quando vuoi rendere il testo navigabile.

Quando premi `Link`, il picker prova anche a usare il testo selezionato come filtro iniziale:

- se trova una corrispondenza reale nel nome dei record, apre il picker già filtrato
- se non trova risultati reali, il filtro iniziale viene svuotato e vedi la lista completa

## Personaggi avventura

Il **personaggio avventura** è il livello che collega una scheda base a una specifica campagna.

Questo record serve a gestire valori che hanno senso **solo dentro un’avventura**, per esempio:

- punti ferita attuali
- punti ferita temporanei
- condizioni
- stato
- ispirazione eroica

In altre parole:

- la scheda base dice **chi è** il personaggio
- il personaggio avventura dice **come sta** quel personaggio dentro una certa campagna

## Presenze nei luoghi

La **presenza nel luogo** è un record diverso ancora. Serve per dire che un personaggio o una creatura è presente in un luogo specifico, con un nome e uno stato eventualmente locali.

Nel form `Aggiungi presenza al luogo` esistono due origini possibili:

- `Personaggio Avventura`
- `PNG / Mostro`

### Presenza da Personaggio Avventura

Se scegli `Personaggio Avventura`, il record del luogo viene collegato a un personaggio già presente nella campagna.

In questo caso:

- la presenza mantiene il collegamento con il personaggio avventura
- non crea una copia autonoma del personaggio
- nel luogo non puoi aggiungere lo stesso personaggio avventura più di una volta

### Presenza da PNG / Mostro

Se scegli `PNG / Mostro`, il luogo crea invece una **presenza locale clonata** a partire da una scheda base di tipo `PNG` o `Mostro`.

Questo record ha dati propri per il luogo, come:

- nome visualizzato
- PF attuali
- PF temporanei
- condizioni
- stato
- disposizione
- note DM

In questo caso il comportamento cambia in base al tipo:

- i **Mostri** possono avere più presenze locali nello stesso luogo
- i **PNG** restano unici nello stesso luogo e non vengono riproposti più volte nel selettore

Quando aggiungi più istanze dello stesso mostro, DnDino propone automaticamente un nome progressivo, per esempio:

- `Goblin 2`

## Perché esiste il nome visualizzato

Sia nelle presenze dei luoghi sia nei partecipanti al combattimento esiste un campo `Nome visualizzato`.

Questo campo serve a mantenere un nome **contestuale** senza dover rinominare la scheda base. È utile, per esempio, quando vuoi:

- distinguere copie simili della stessa creatura
- dare un nome specifico a un PNG in un solo luogo
- usare un nome diverso nel combattimento senza cambiare il record sorgente

## Partecipanti al combattimento

Il **partecipante al combattimento** è il livello operativo usato nello scontro.

Un partecipante può nascere da tre sorgenti diverse:

- un **personaggio avventura**
- una **presenza del luogo**
- una **scheda base**

Ogni partecipante al combattimento ha il proprio record con dati specifici dello scontro, come:

- nome visualizzato
- iniziativa
- CA
- PF massimi
- PF attuali
- PF temporanei
- condizioni
- stato
- tiri salvezza contro la morte
- ordine nel round

### Partecipanti da personaggio avventura

Se il partecipante nasce da un personaggio avventura:

- resta collegato al personaggio della campagna
- a fine combattimento i valori finali vengono sincronizzati di nuovo sul record avventura

### Partecipanti da presenza del luogo

Se il partecipante nasce da una presenza del luogo:

- resta collegato a quel record del luogo
- se la presenza ha stato locale, il combattimento può sincronizzare di nuovo PF, condizioni e stato sul record del luogo

### Partecipanti da scheda base

Se il partecipante nasce direttamente da una scheda base:

- il record combattimento usa quella scheda come sorgente
- il comportamento rispetto alle istanze multiple dipende dal tipo

Nel selettore combattimento, infatti:

- un record base di tipo **Mostro** può essere aggiunto più volte
- un record base di tipo **PNG** o **Eroe** non viene riproposto più volte nello stesso combattimento

## Sincronizzazione tra i livelli

Alcuni valori vengono sincronizzati tra livelli diversi, ma non tutto viene sovrascritto sempre.

### Dalla scheda base verso i contesti

La scheda base fornisce:

- identità del personaggio
- statistiche di riferimento
- incantesimi
- attacchi
- immagini

### Dai contesti verso i record collegati

I livelli operativi possono invece sincronizzare dati situazionali, soprattutto:

- PF
- condizioni
- stato
- alcune note locali

Nel combattimento, per esempio, i valori finali possono tornare:

- sul personaggio avventura collegato
- sulla presenza del luogo collegata, se quella presenza usa stato locale

## Differenza pratica tra i livelli

Per ricordare meglio la logica, puoi leggerla così:

- `Scheda base`: il **modello generale** del personaggio
- `Personaggio avventura`: lo **stato del personaggio dentro la campagna**
- `Presenza nel luogo`: la **presenza contestuale del personaggio in un luogo specifico**
- `Partecipante al combattimento`: la **versione operativa del personaggio nello scontro**

## Quando conviene usare ogni livello

### Usa la scheda base quando:

- devi creare il personaggio
- vuoi modificare i dati strutturali
- devi collegare immagini, incantesimi o attacchi

### Usa il personaggio avventura quando:

- vuoi collegare un eroe alla campagna
- devi tenere traccia di PF, stato, condizioni e ispirazione in modo persistente nell’avventura

### Usa la presenza nel luogo quando:

- vuoi popolare un luogo con personaggi o creature
- vuoi dare nomi contestuali a PNG e mostri
- vuoi creare istanze locali separate dentro un luogo

### Usa il partecipante al combattimento quando:

- stai preparando o gestendo uno scontro
- ti servono iniziativa, PF e condizioni di battaglia
- vuoi che il combattimento lavori su record contestuali senza sporcare direttamente la scheda base

## In sintesi

La sezione `Eroi, PNG e Mostri` non è solo un archivio di schede. È il **livello sorgente** da cui nasce tutta la gestione contestuale dei personaggi dentro l’app.

La logica generale è questa:

- la **scheda base** definisce il personaggio
- il **personaggio avventura** lo inserisce nella campagna
- la **presenza nel luogo** lo contestualizza in un luogo
- il **partecipante al combattimento** lo rende operativo nello scontro

!!! tip
    Se vuoi evitare confusione, pensa sempre a questa distinzione: la scheda base descrive il personaggio, mentre avventura, luogo e combattimento descrivono il suo stato in un contesto preciso. Non serve fissarsi troppo sulla separazione teorica: considera soprattutto che alcuni campi esistono solo nel loro contesto.
