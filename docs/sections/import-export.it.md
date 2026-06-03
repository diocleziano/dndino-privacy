# Importazione ed esportazione

DnDino permette di esportare e importare contenuti per spostarli tra installazioni, creare copie di lavoro o condividere materiale con altri Dungeon Master.

Le importazioni non sovrascrivono automaticamente i dati esistenti: prima di salvare puoi controllare cosa verrà aggiunto, sostituito o ignorato.

## Incantesimi

Gli incantesimi possono essere esportati in un file JSON.

Durante l'importazione DnDino distingue:

- incantesimi nuovi
- incantesimi con lo stesso nome già presenti nel database

Per ogni incantesimo puoi scegliere se:

- importarlo come nuovo record
- sovrascrivere un record esistente
- ignorarlo

Quando esiste già un incantesimo con lo stesso nome, la schermata di revisione mostra il confronto tra il record presente e quello importato. In questo modo puoi controllare livello, scuola, manuale, classi, tempo di lancio e durata prima di decidere.

Sono disponibili anche azioni rapide per gestire più conflitti insieme, ad esempio saltare tutti gli incantesimi già presenti o importarli tutti come nuovi.

## Personaggi

I personaggi vengono esportati in un pacchetto ZIP che può includere:

- scheda del personaggio
- immagini collegate
- collegamenti agli incantesimi
- dati utili per ricostruire il record nell'altra installazione

Durante l'importazione, i personaggi con lo stesso nome non vengono sostituiti automaticamente. Puoi importarli come nuovi, sovrascrivere un record esistente o ignorarli.

Se il personaggio importato ha incantesimi collegati, DnDino prova ad associarli agli incantesimi già presenti usando il nome. Se trova più incantesimi compatibili, ti chiede quale usare.

Quando importi personaggi in un database già ricco, controlla sempre i collegamenti agli incantesimi: due incantesimi possono avere lo stesso nome ma provenire da manuali o versioni diverse.

## Avventure

Le avventure vengono esportate in un pacchetto ZIP con i dati necessari a ricostruire l'avventura.

Un'importazione di avventura viene sempre creata come **nuova avventura**. DnDino non sovrascrive un'avventura già esistente, così non rischi di perdere luoghi, personaggi o sessioni della tua campagna attiva.

Il flusso consigliato è a step:

1. importa o collega gli incantesimi
2. importa o collega i personaggi
3. importa l'avventura

Nella revisione dell'avventura DnDino separa le parti principali:

- incantesimi inclusi nel pacchetto
- personaggi inclusi nel pacchetto
- struttura dell'avventura

Per incantesimi e personaggi puoi decidere come gestire i record già presenti. Dopo questa scelta, l'avventura viene importata collegando i personaggi corretti ai luoghi, alle presenze e agli altri contenuti del pacchetto.

## Equipaggiamento, talenti e glossario

Anche equipaggiamento, talenti e glossario possono essere esportati e importati separatamente.

L'esportazione crea file JSON dedicati, utili per condividere solo una parte del materiale senza dover esportare un'intera avventura.

Durante l'importazione DnDino separa i record nuovi da quelli che hanno già una corrispondenza nel database. Per ogni record puoi scegliere se importarlo come nuovo, sovrascrivere quello esistente o ignorarlo.

Per l'equipaggiamento il confronto considera nome e categoria, così armi, armature, strumenti e dotazione restano distinti. Per i talenti viene considerato anche il tipo di talento. Per il glossario il riferimento principale è il nome della voce.

Quando esiste già un record simile, la schermata di revisione mostra il confronto tra il contenuto presente e quello importato. Usa le azioni massive per saltare, importare o sovrascrivere più record insieme quando il file contiene molti elementi.

## Controlli prima dell'importazione

Prima di importare pacchetti con immagini, DnDino verifica che il file sia leggibile e che ci sia spazio sufficiente per copiare i media nel contenitore dell'app.

Se il file è danneggiato, incompleto o non compatibile, l'importazione viene interrotta con un messaggio di errore invece di creare dati parziali.

## Buone pratiche

Prima di importare contenuti importanti:

- crea un backup dell'app
- importa prima gli incantesimi se sai che verranno usati da molti personaggi
- controlla i record con lo stesso nome prima di sovrascriverli
- usa il confronto tra vecchio e nuovo record quando non sei sicuro
- importa le avventure come nuove e poi verifica collegamenti, luoghi e immagini

L'importazione è pensata per proteggere il database: in caso di dubbio, scegli `Importa come nuovo` o `Ignora` invece di sovrascrivere.
