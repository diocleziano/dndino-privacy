# DnDino Docs

Base guida separata dal progetto app, pensata per essere pubblicata in HTML con:

- ricerca
- indice laterale
- immagini
- pagine in Markdown

## Dove si trova

La cartella della guida e:

```text
/Users/dno/Documents/XCode/DnDino-Docs
```

## Come avviare la guida in locale

Apri il Terminale e vai nella cartella della guida:

```bash
cd /Users/dno/Documents/XCode/DnDino-Docs
```

Avvia MkDocs:

```bash
python3 -m mkdocs serve
```

Poi apri nel browser:

```text
http://127.0.0.1:8000
```

## Come generare l'HTML statico

Sempre dalla cartella della guida:

```bash
python3 -m mkdocs build
```

L'output finale viene creato in:

```text
/Users/dno/Documents/XCode/DnDino-Docs/site
```

## Dove scrivere i contenuti

Le pagine della guida stanno dentro:

```text
/Users/dno/Documents/XCode/DnDino-Docs/docs
```

Esempi:

- `docs/index.md`
- `docs/funzioni/combattimento-flat.md`
- `docs/sections/places.en.md`

## Editor consigliato

Ti consiglio **Visual Studio Code**.

Funziona bene perche ha:

- supporto ottimo al Markdown
- anteprima integrata
- gestione semplice delle immagini

Per vedere l'anteprima Markdown in VS Code:

- `Cmd+Shift+V`

## Mini guida Markdown

Titoli:

```md
# Titolo principale
## Titolo sezione
### Sottosezione
```

Grassetto, corsivo e codice:

```md
**Grassetto**
*Corsivo*
`codice`
```

Liste:

```md
- Primo punto
- Secondo punto
- Terzo punto
```

Liste numerate:

```md
1. Primo passo
2. Secondo passo
3. Terzo passo
```

Link:

```md
[Apri il sito](https://www.example.com)
```

Blocchi codice:

````md
```bash
python3 -m mkdocs serve
```
````

Nota evidenziata:

```md
!!! note
    Questa e una nota.
```

## Come inserire immagini

Le immagini vanno dentro:

```text
/Users/dno/Documents/XCode/DnDino-Docs/docs/images
```

Puoi organizzarle in sottocartelle, per esempio:

- `docs/images/personaggi/`
- `docs/images/luoghi/`
- `docs/images/combattimento/`

Se stai scrivendo in:

```text
docs/funzioni/combattimento-flat.md
```

e l'immagine si trova in:

```text
docs/images/combattimento/flat-overview.png
```

usa:

```md
![Panoramica combattimento flat](../images/combattimento/flat-overview.png)
```

## Consigli pratici per le immagini

- usa nomi semplici come `flat-overview.png`
- evita spazi nei nomi file
- preferisci minuscole e trattini
- tieni una cartella immagini per ogni area dell'app

## Convenzione immagini

Per mantenere la guida coerente, usa queste classi CSS già pronte nei file Markdown.

### Logo

Usa `img-logo` per il logo o l'icona principale di una pagina.

```md
![DnDino](images/icons/appicon.png){ .img-logo }
```

### Hero

Usa `img-hero` per l'immagine principale in alto nella pagina.  
È grande, centrata e pensata per screenshot panoramici.

```md
![HomePage](../images/homepage/it_home.png){ .img-hero }
```

### Screenshot standard

Usa `img-shot` per gli screenshot principali dentro il corpo della guida.

```md
![Combattimento Flat](../images/combattimento/flat-overview.png){ .img-shot }
```

### Dettaglio

Usa `img-detail` per popover, pulsanti, piccoli pannelli o zoom su una singola parte dell'interfaccia.

```md
![Dettaglio pulsante](../images/homepage/detail-button.png){ .img-detail }
```

### Classi legacy

Restano disponibili anche:

- `img-small`
- `img-medium`
- `img-large`

### Regola pratica

- usa `img-hero` una sola volta all'inizio della pagina
- usa `img-shot` per gli screenshot principali
- usa `img-detail` per i particolari dell'interfaccia
- usa `img-logo` per logo e icone introduttive

## Immagine affiancata al testo

Se vuoi restare in **solo Markdown**, puoi usare le classi `img-left` e `img-right` direttamente sulla riga dell'immagine.

### Immagine a sinistra, testo affiancato

```md
![HomePage](../images/homepage/it_home.png){ .img-left }

Qui puoi scrivere il testo della sezione. L'immagine resta affiancata al contenuto finché c'è abbastanza spazio.

- punto importante
- altro punto importante

Questo testo continuerà a scorrere accanto all'immagine.

<div class="img-clear"></div>
```

### Immagine a destra, testo affiancato

```md
![HomePage](../images/homepage/it_home.png){ .img-right }

Qui il testo resta a sinistra e l'immagine va a destra.

Quando hai finito il blocco di testo, aggiungi:

<div class="img-clear"></div>
```

### Regola pratica

- `img-left`: immagine a sinistra
- `img-right`: immagine a destra
- `img-clear`: chiude il testo affiancato e fa ripartire il layout normale sotto
- `img-left-small`, `img-left-medium`, `img-left-large`: immagine a sinistra con dimensione fissa
- `img-right-small`, `img-right-medium`, `img-right-large`: immagine a destra con dimensione fissa
- `img-center-small`, `img-center-medium`, `img-center-large`: immagine centrata con dimensione fissa

Su schermi più piccoli le immagini tornano automaticamente centrate e in verticale.

### Cosa fa `img-clear`

Quando usi un'immagine a sinistra o a destra, il testo normale che scrivi subito sotto tende a scorrere accanto all'immagine.

Questo è utile finché vuoi davvero il testo affiancato.

Quando invece vuoi che il contenuto successivo torni **sotto** l'immagine, devi chiudere il float con:

```md
<div class="img-clear"></div>
```

In pratica:

- senza `img-clear`, anche il testo successivo può continuare a stare accanto all'immagine
- con `img-clear`, da quel punto in poi il layout torna normale e riparte sotto

Esempio:

```md
![Dettaglio](../images/homepage/detail-button.png){ .img-right-small }

Questo paragrafo resta accanto all'immagine.
Anche questo resta accanto all'immagine.

<div class="img-clear"></div>

Da qui in poi il contenuto torna sotto l'immagine.
```

Se l'immagine è centrale, `img-clear` non serve.

### Esempi rapidi

Immagine a sinistra piccola:

```md
![Dettaglio](../images/homepage/detail-button.png){ .img-left-small }

Testo della sezione.

<div class="img-clear"></div>
```

Immagine a destra media:

```md
![HomePage](../images/homepage/it_home.png){ .img-right-medium }

Testo della sezione.

<div class="img-clear"></div>
```

Immagine centrale grande:

```md
![HomePage](../images/homepage/it_home.png){ .img-center-large }
```

## Flusso consigliato

1. apri VS Code sulla cartella `DnDino-Docs`
2. avvia `python3 -m mkdocs serve`
3. apri `http://127.0.0.1:8000`
4. modifica i file `.md`
5. trascina le immagini in `docs/images`
6. controlla subito il risultato nel browser
