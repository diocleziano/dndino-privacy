# Home Page

La **Home Page** è la schermata iniziale di DnDino. Non è un pannello operativo per gestire direttamente ogni modulo dell’app, ma un **punto di accesso rapido** pensato per:

- riprendere subito l’ultima avventura usata
- tornare velocemente agli strumenti principali
- orientarsi all’apertura dell’app

La Home ha quindi due funzioni principali:

- **ripresa rapida**, se hai già una campagna attiva
- **avvio guidato**, se stai iniziando da zero

## Struttura della schermata

La Home è composta da tre aree principali:

1. intestazione di benvenuto
2. riquadro principale dedicato all’ultima avventura o all’avvio iniziale
3. griglia con gli strumenti principali dell’app

## Intestazione di benvenuto

Nella parte alta della schermata compare un saluto iniziale.

Se nelle impostazioni è stato inserito il nome del Dungeon Master, la Home mostra un messaggio personalizzato, ad esempio:

- `Ciao, Marco!`

In caso contrario compare una versione generica:

- `Ciao, DM!`

Sotto al saluto è presente una breve frase che spiega lo scopo della schermata: riprendere il lavoro da dove era stato lasciato oppure aprire subito uno degli strumenti principali.

## Riquadro principale

Il riquadro principale cambia in base allo stato dell’app.

### Se esiste già un’avventura recente

Quando l’app trova un’avventura usata di recente, la Home mostra una card ampia dedicata all’**ultima avventura**.

Questa card contiene:

- il titolo dell’avventura
- una breve descrizione, se presente
- un pulsante `Apri avventura`
- un eventuale pulsante per andare direttamente all’ultimo luogo visitato
- alcune statistiche riassuntive
- una sezione visiva con gli eroi collegati all’avventura

Se l’avventura ha un’immagine di copertina, questa viene usata come sfondo della card. In caso contrario viene mostrato uno sfondo grafico predefinito.

#### Pulsante Apri avventura

Il pulsante principale della card apre direttamente la **dashboard dell’avventura**, cioè il centro operativo della campagna.

È il modo più veloce per riprendere il lavoro.

#### Pulsante Vai all’ultimo luogo visitato

Se l’app conosce l’ultimo luogo aperto all’interno dell’avventura, nella card compare anche un secondo pulsante che porta direttamente a quel luogo.

Questo è utile quando vuoi riprendere subito l’esplorazione o il lavoro su una sezione narrativa precisa della campagna.

## Statistiche dell’avventura

Nel riquadro principale vengono mostrate alcune metriche di riepilogo dell’ultima avventura.

Le statistiche visibili sono:

- `Quest`
- `Luoghi`
- `Sessioni`
- `Combattimenti`

Questi valori servono solo come colpo d’occhio rapido per capire quanto materiale è già stato costruito nella campagna.

## Eroi dell’avventura

Se l’avventura ha eroi collegati, nella parte destra della card compare una sezione dedicata a loro.

Questa area può mostrare:

- il numero totale degli eroi
- i ritratti, se disponibili
- un messaggio che invita ad aggiungere una copertina agli eroi se non ci sono immagini

Quando c’è un solo eroe, il ritratto viene mostrato in modo più grande. Quando gli eroi sono diversi, i ritratti vengono disposti in un insieme compatto.

Questa sezione ha una funzione soprattutto visiva: aiuta a riconoscere subito la campagna a colpo d’occhio.

## Quando non esiste ancora nessuna avventura

Se l’utente non ha ancora avventure disponibili, la Home mostra un riquadro alternativo pensato per accompagnare il primo avvio.

In questo caso la schermata presenta:

- il titolo `Pronto a iniziare`
- una breve descrizione introduttiva
- il pulsante `Vai alle avventure`
- tre passaggi consigliati per iniziare a usare DnDino

I tre passaggi mostrati sono:

1. creare un’avventura
2. aggiungere i personaggi
3. costruire luoghi e quest

Questa versione della Home ha quindi una funzione di onboarding: accompagna l’utente nella creazione della prima campagna.

## Strumenti principali

Sotto al riquadro principale è presente una griglia di card che rappresenta gli strumenti principali dell’app.

Le sezioni accessibili dalla Home sono:

- `Avventure`
- `Eroi, PNG e Mostri`
- `Equipaggiamento`
- `Regole`
- `Generatore Nomi`
- `Impostazioni`

Ogni card contiene:

- titolo
- breve sottotitolo descrittivo
- icona
- sfondo illustrato dedicato

### Avventure

Apre l’elenco delle campagne e permette di:

- creare una nuova avventura
- aprire una campagna esistente
- riprendere il lavoro di preparazione

### Eroi, PNG e Mostri

Porta alla sezione che raccoglie le schede delle creature. Da qui è possibile lavorare su:

- eroi
- PNG
- mostri
- dati base collegati alle schede

!!! tip
    Con il tempo ti accorgerai che molti personaggi possono essere aperti e modificati direttamente anche dall’interno dell’avventura, senza interrompere il tuo flusso di preparazione.

### Equipaggiamento

Apre la sezione dedicata a:

- armi
- armature
- strumenti
- dotazioni

### Regole

Apre il pannello di consultazione rapida delle regole e dei riferimenti. È utile per:

- consultare materiale di supporto
- cercare regole
- consultare contenuti collegati al gioco

### Generatore Nomi

Apre lo strumento per generare rapidamente nomi utili durante la preparazione o l’improvvisazione, ad esempio per:

- PNG
- mostri
- incontri improvvisi

!!! tip
    Durante la sessione ti tornerà spesso più comodo usare il mini generatore di nomi direttamente dalla topbar, senza uscire dalla schermata in cui ti trovi.

### Impostazioni

Apre il pannello delle preferenze globali dell’app e della gestione locale del database.

## Quando usare la Home

La Home è utile soprattutto quando vuoi:

- riprendere velocemente l’ultima campagna
- aprire la dashboard dell’avventura più recente
- tornare all’ultimo luogo visitato
- accedere rapidamente agli strumenti principali dell’app
- iniziare una nuova campagna se il database è ancora vuoto

!!! tip
    Se stai lavorando sempre sulla stessa campagna, il riquadro dell’ultima avventura è il modo più rapido per rientrare subito nel punto giusto senza passare ogni volta dall’elenco completo delle avventure.
