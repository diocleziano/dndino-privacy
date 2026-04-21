# Mappe concettuali

La sezione **Mappe concettuali** serve a costruire una rappresentazione visiva delle relazioni tra luoghi, personaggi, mappe concettuali e note libere.

Non è una mappa geografica e non è una lavagna generica: è uno strumento pensato per collegare i nodi della campagna in modo rapido, leggibile e navigabile.

Puoi usarla per:

- organizzare la struttura narrativa dell’avventura
- collegare luoghi e personaggi
- tracciare relazioni tra elementi importanti
- aggiungere riquadri tematici
- annotare idee direttamente su nodi, riquadri e collegamenti

## Dove si trova

Le mappe concettuali si aprono da due punti principali:

- dalla **dashboard avventura**, nel pannello `Mappe Concettuali`
- dalla dashboard di un **luogo**, quando vuoi creare o aprire una mappa concettuale legata a quel luogo

Questo significa che una mappa concettuale può essere:

- **globale di avventura**
- **legata a un luogo specifico**

## Come è fatta la schermata

La schermata delle mappe concettuali è divisa in tre colonne principali:

- **sidebar sinistra** con palette e lista delle mappe
- **canvas centrale** dove costruisci la mappa
- **inspector a destra** con i dettagli dell’elemento selezionato

## Sidebar: palette e sorgenti

La sidebar di sinistra raccoglie tutto ciò che puoi inserire nella mappa.

Le categorie principali sono:

- `Luoghi`
- `Personaggi`
- `Mappe`

In più puoi lavorare con:

- filtri
- ricerca testuale
- creazione di riquadri
- creazione di nodi liberi

## Filtri della palette

La palette supporta un filtro dedicato con queste modalità:

- `Tutto`
- `Luoghi`
- `Personaggi`
- `Mappe`

## Ricerca nella palette

La barra di ricerca della palette serve per trovare rapidamente:

- un luogo
- un personaggio
- una mappa concettuale già esistente

## Cosa puoi trascinare nel canvas

Nel canvas puoi trascinare:

- luoghi dell’avventura
- personaggi disponibili per l’avventura
- altre mappe concettuali
- nodi liberi

I personaggi disponibili nella palette non sono tutti i personaggi del database in modo indiscriminato: il sistema usa i personaggi collegati all’avventura.

## Luoghi nella palette

I luoghi nella palette vengono mostrati tenendo conto della gerarchia dei luoghi dell’avventura.

## Personaggi nella palette

I personaggi mostrati nella palette hanno un sottotitolo informativo che può includere:

- tipo
- razza
- classe

## Mappe nella palette

La sezione `Mappe` della palette mostra le altre mappe concettuali dell’avventura.

Questo è utile perché una mappa concettuale può contenere un nodo che punta a un’altra mappa concettuale, creando una rete di mappe collegate tra loro.

## Creare una nuova mappa concettuale

Puoi creare una nuova mappa concettuale:

- dalla dashboard avventura
- dalla dashboard di un luogo
- direttamente dalla schermata mappe concettuali, se già ne stai gestendo una

Quando viene creata, DnDino le assegna automaticamente un nome progressivo come:

- `Mappa concettuale`
- `Mappa concettuale 2`
- `Mappa concettuale 3`

## Rinominare una mappa

Il titolo della mappa attiva è modificabile direttamente nella schermata.

Quando esci dal campo o confermi la modifica, DnDino salva il nuovo nome della mappa.

## Eliminare una mappa

Selezionando una mappa attiva puoi eliminarla con il pulsante `Elimina`.

## Il canvas centrale

Il **canvas** è la zona principale in cui costruisci la mappa.

Qui puoi:

- trascinare nodi dalla palette
- spostare i nodi
- creare riquadri
- collegare nodi e riquadri con frecce
- leggere la struttura generale della campagna a colpo d’occhio

## Tipi di elementi nel canvas

Nel canvas esistono tre famiglie principali di elementi:

- **nodi**
- **riquadri**
- **collegamenti**

### Nodi

I nodi rappresentano:

- un luogo
- un personaggio
- una mappa concettuale
- un nodo libero

### Riquadri

I riquadri servono per raggruppare visivamente più nodi in un’area comune.

### Collegamenti

I collegamenti sono frecce che uniscono nodi e riquadri.

## Nodi normali e nodi liberi

### Nodi collegati a record reali

Quando trascini nel canvas un luogo, un personaggio o una mappa concettuale, crei un nodo collegato a un record reale dell’app.

Questo significa che il nodo:

- mostra il titolo reale dell’elemento
- può mostrare il sottotitolo contestuale
- può aprire il record collegato dall’inspector

### Nodo libero

Il `Nodo libero` è un nodo speciale per idee e appunti non collegati a un record reale.

È utile per:

- annotazioni narrative
- concetti astratti
- eventi
- gruppi di idee
- promemoria di design

## Riquadri di gruppo

Il pulsante `Riquadro` crea un contenitore visivo all’interno del canvas.

Un riquadro:

- ha un titolo
- ha una nota dedicata
- può essere spostato
- può essere ridimensionato
- può essere collassato
- può contenere automaticamente i nodi che ricadono al suo interno

## Come si spostano i nodi

I nodi possono essere trascinati liberamente nel canvas.

La loro posizione viene salvata nella mappa, quindi l’organizzazione resta persistente.

## Come si spostano i riquadri

Anche i riquadri possono essere trascinati.

Quando sposti un riquadro, DnDino può spostare insieme anche i nodi che ne fanno parte, mantenendo il gruppo leggibile.

## Ridimensionare un riquadro

I riquadri possono essere ridimensionati tramite gli angoli.

## Collassare un riquadro

Un riquadro può essere collassato.

Quando è collassato:

- occupa meno spazio
- i nodi interni vengono nascosti dal canvas
- i collegamenti degli elementi nascosti non appesantiscono la lettura

## Creare un collegamento

I collegamenti tra elementi si creano trascinando dal punto di aggancio di un nodo o di un riquadro verso un altro elemento compatibile.

Puoi collegare:

- nodo → nodo
- nodo → riquadro
- riquadro → nodo
- riquadro → riquadro

DnDino evita:

- collegamenti duplicati identici
- collegamenti da un elemento a sé stesso

## A cosa servono le frecce

Le frecce servono a rappresentare relazioni, per esempio:

- un personaggio che controlla un luogo
- un luogo che porta a un altro
- una mappa che rimanda a una sottomappa
- un gruppo tematico collegato a un nodo narrativo

## Inspector: dettagli dell’elemento selezionato

La colonna destra cambia contenuto in base a ciò che selezioni.

Può mostrare i dettagli di:

- un nodo
- un riquadro
- un collegamento
- oppure della mappa nel suo complesso, se non hai nulla di selezionato

## Se selezioni un nodo

Quando selezioni un nodo, l’inspector mostra:

- titolo
- sottotitolo
- eventuale pulsante `Apri record`
- descrizione contestuale, se disponibile
- note del nodo
- pulsante per eliminare il nodo

### Aprire il record collegato

Se il nodo è collegato a:

- un luogo
- un personaggio

puoi aprire direttamente il relativo form.

Se invece il nodo è collegato a un’altra **mappa concettuale**, il pulsante apre quella mappa e mantiene anche una piccola cronologia di navigazione tra mappe.

### Descrizione contestuale del nodo

Per alcuni tipi di nodo, l’inspector mostra anche una descrizione reale già esistente nell’app:

- per un **luogo** mostra la `Descrizione DM`
- per un **personaggio** mostra la descrizione del personaggio

### Note del nodo

Ogni nodo ha anche note proprie, separate dal record sorgente.

## Se selezioni un riquadro

Quando selezioni un riquadro, l’inspector mostra:

- titolo del riquadro
- numero di elementi contenuti
- note del riquadro
- pulsante per eliminare il riquadro

## Se selezioni un collegamento

Quando selezioni una freccia, l’inspector mostra:

- riepilogo del collegamento
- nota della freccia
- pulsante per eliminare il collegamento

Le note sui collegamenti sono molto utili quando vuoi dare un significato più preciso alla relazione, ad esempio:

- alleanza
- dipendenza
- parentela
- passaggio
- causa-effetto

## Se non selezioni nulla

Quando non c’è nessun elemento selezionato, l’inspector mostra un riepilogo della mappa:

- nome della mappa
- numero nodi
- numero collegamenti

## Zoom e navigazione

La schermata supporta:

- zoom
- pan del canvas
- gesture di pinch
- uso rapido di scorciatoie con mouse e trackpad

## Immagini nei nodi

I nodi collegati a luoghi o personaggi possono usare anche l’immagine di copertina del record collegato come sfondo visivo.

## Mappe concettuali collegate tra loro

Uno degli usi più potenti del sistema è la possibilità di collegare una mappa concettuale a un’altra.

Questo permette di costruire:

- una mappa generale dell’avventura
- mappe secondarie per aree specifiche
- mappe specialistiche per personaggi, fazioni o sottotrame

## Quando conviene usarle

Le mappe concettuali sono particolarmente utili quando vuoi:

- pianificare una campagna lunga
- visualizzare relazioni complesse
- organizzare personaggi e luoghi in blocchi
- preparare sottotrame
- avere una vista strategica che non dipende da testi lunghi

## Differenza rispetto ai Luoghi

La sezione `Luoghi` organizza l’avventura sul piano spaziale e contenutistico.

Le **mappe concettuali** invece organizzano la campagna sul piano relazionale.

In breve:

- `Luoghi` = struttura del mondo e contenuti contestuali
- `Mappe concettuali` = struttura logica, narrativa e relazionale

## Differenza rispetto alle mappe interattive

Le **mappe interattive** servono a navigare luoghi reali con marker su una mappa grafica.

Le **mappe concettuali** servono invece a collegare concetti, personaggi, luoghi e idee.

## Buone pratiche

Per usare bene le mappe concettuali conviene:

- tenere una mappa generale dell’avventura
- creare mappe più piccole per aree o capitoli
- usare i riquadri per separare i gruppi di nodi
- usare i nodi liberi per idee che non hanno ancora una scheda reale
- annotare nodi e frecce con note brevi ma utili

## In sintesi

Le mappe concettuali di DnDino sono uno strumento di organizzazione avanzata.

Permettono di costruire una vista visiva e navigabile della campagna, collegando:

- luoghi
- personaggi
- altre mappe
- note libere
- relazioni espresse con frecce

!!! tip
    Se una campagna diventa complessa, prova a usare una mappa concettuale generale per la vista d’insieme e mappe più piccole per singole città, fazioni o sottotrame. È uno dei modi più efficaci per non perdere il filo.
