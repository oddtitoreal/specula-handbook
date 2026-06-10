# Contribuire al Specula Handbook

Grazie dell'interesse. Questo manuale è open source e i contributi sono benvenuti, con una distinzione importante tra ciò che può essere contribuito qui e ciò che appartiene all'evoluzione del metodo.

## Cosa accettiamo

**Correzioni e chiarimenti** — Errori tipografici, link rotti, imprecisioni fattuali rispetto ai repo di riferimento, formulazioni ambigue. Apri una [issue](https://github.com/oddtitoreal/specula-handbook/issues) con il template *Bug / Errore* o *Chiarimento*, oppure direttamente una PR per le correzioni banali.

**Traduzioni** — Il manuale è in italiano per scelta; le versioni in altre lingue sono benvenute. Apri prima una issue con il template *Traduzione* per coordinarti ed evitare lavoro duplicato.

**Note dal campo** — Hai usato un workshop Specula e hai osservazioni sull'applicazione pratica? È il contributo più prezioso. Una PR che aggiunge una sezione "Note dal campo" alla fine della pagina del workshop: cosa ha funzionato, cosa va calibrato, in quale contesto.

## Cosa non accettiamo

**Modifiche al metodo** — La struttura del BOS, la sequenza dei layer, i principi etici, il funzionamento del Circolo di Sintesi evolvono nei repo [`specula-method`](https://github.com/oddtitoreal/specula-method) e [`specula-bos`](https://github.com/oddtitoreal/specula-bos), non in questo manuale. Una PR che cambia come funziona il metodo verrà chiusa con un reindirizzo al repo appropriato.

**Contenuti commerciali** — La licenza BY-NC-SA non permette usi commerciali. Non accettiamo link, riferimenti o endorsement commerciali.

## Come proporre una modifica

1. Apri una issue con il template appropriato (o verifica che non esista già).
2. Per le PR: fork → branch → modifica → PR con descrizione di cosa cambia e perché.
3. Una pagina = una PR, dove possibile. Le PR piccole vengono riviste prima.

## Convenzioni redazionali

- Ogni pagina ha frontmatter con `title` e `description`; il body **non** ripete il titolo come H1.
- I link interni sono percorsi assoluti senza estensione: `/workshops/archeologia-brand`, non `../06_Workshop/03_archeologia-brand.md`.
- I termini canonici seguono il [glossario](https://speculafuturecrafting.mintlify.app/glossario); in caso di dubbio fa fede `specula-framework/specs/terminology.md`.
- Le pagine workshop seguono la struttura comune: Obiettivo, Quando si usa, Partecipanti e ruoli, Preparazione, Svolgimento, Criteri di riuscita, Errori comuni, Output e destinazione.
- Prosa in italiano, termini tecnici del metodo in inglese dove canonici (Refusal Register, Ethical Gate…).

## Anteprima locale

```bash
npm i -g mint
mint dev
```

## Codice di condotta

Partecipando accetti il [Codice di Condotta](CODE_OF_CONDUCT.md).
