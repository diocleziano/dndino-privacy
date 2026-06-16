# Librerie riutilizzabili

DnDino Hero separa il personaggio dai contenuti riutilizzabili.

Questa scelta evita di reinserire ogni volta le stesse informazioni e permette di mantenere coerenza tra più personaggi.

## Classi

Le classi sono contenuti condivisi.

Una classe può contenere:

- nome
- descrizione
- dado vita
- caratteristiche primarie
- competenze nei tiri salvezza
- competenze nelle abilità
- competenze in armi, armature e strumenti
- equipaggiamento iniziale
- privilegi di classe
- progressioni
- sottoclassi
- incantesimi
- liste libere personalizzate

Quando modifichi una classe, i personaggi associati leggono la definizione aggiornata.

## Sottoclassi

Le sottoclassi appartengono a una classe.

Ogni sottoclasse può avere:

- nome
- privilegi della sottoclasse
- liste libere
- incantesimi, se previsti
- caratteristica da incantatore, se la sottoclasse usa magia

Nel personaggio la sottoclasse viene scelta per ogni classe, solo quando quella classe raggiunge il livello richiesto.

## Progressioni

Le progressioni servono per rappresentare valori che cambiano con il livello.

Possono essere usate per:

- risorse consumabili
- bonus
- valori numerici
- dadi
- valori descrittivi

Le progressioni di tipo risorsa possono mostrare residui e totale, con pulsanti per consumare o ripristinare.

!!! note
    I bonus dichiarati nelle progressioni non vengono applicati automaticamente a caratteristiche, attacchi o altre statistiche. Vanno aggiunti manualmente dove devono incidere.

Le progressioni di tipo dado o bonus possono essere richiamate anche negli attacchi, per costruire danni aggiuntivi o modificatori legati alla classe.

## Bonus dei privilegi

I privilegi di classe e alcune liste libere possono mostrare un bonus costruito da più parti.

Un bonus può includere:

- tiro di dado
- livello della classe
- bonus di competenza
- modificatore di caratteristica
- valore libero
- progressione di classe di tipo dado o bonus

Puoi anche assegnare un nome al totale del bonus, utile quando vuoi mostrare in scheda una formula compatta come `1d10 + 5`.

## Specie

Le specie sono riutilizzabili e possono contenere:

- nome della specie
- tipo di creatura
- taglia
- altezza
- velocità base
- descrizione
- tratti della specie

I tratti possono dipendere dal livello. Nella scheda generale vengono mostrati solo quelli disponibili al livello attuale.

## Background

I background possono contenere:

- nome
- punteggi caratteristica selezionabili
- talento
- competenze nelle abilità
- competenze negli strumenti
- equipaggiamento
- descrizione

Il nome del background viene condiviso con l'identità del personaggio.

## Talenti, regole e incantesimi

DnDino Hero prevede sezioni generali per:

- talenti
- regole
- incantesimi

Questi elementi possono essere importati, esportati e associati al personaggio quando servono.

Gli incantesimi possono essere associati al personaggio, marcati come preparati o non preparati e mostrati in scheda solo quando sono realmente disponibili.

## Importazione ed esportazione

Le librerie principali possono essere esportate e importate in JSON, così puoi spostare contenuti tra dispositivi o recuperarli da DnDino.

In caso di nome già esistente, l'importazione deve chiedere come procedere, evitando sovrascritture involontarie.

Sono previste importazione ed esportazione per:

- classi
- specie
- background
- incantesimi
- talenti
- regole
