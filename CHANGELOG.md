# Changelog

Tutte le modifiche rilevanti al Manuale Specula sono documentate qui.

Il formato segue [Keep a Changelog](https://keepachangelog.com/it/1.0.0/).
Il versioning usa il formato `YYYY.MM`.

---

## [2026.11] · da rilasciare

### Revisione metodologica · 2026-10-21

Allinea il manuale a `specula-method` 2.0, `specula-bos` 2.2, `specula-framework` 1.3 e `specula-skill` 0.3.

**Aggiunto**
- `governance/decision-log.md`: Decision Log, revisione dei criteri, classificazione delle derive, procedimento di calcolo di Brand Coherence Index e Learning Velocity. In navigazione (`docs.json`) e in `INDICE.md`
- `engagement/full-journey.md`: sezione "Tempi e compressione"
- `foundations/subtractive-thesis.md`: sezione "L'ambito della tesi"
- `foundations/threshold-conditions.md`: evidenza da registrare per ogni condizione e sezione "La scheda di soglia"
- `bos/circolo-di-sintesi.md`: funzioni, regole di voto e regole per il disaccordo sui valori, con il Governance Charter di `specula-framework` come fonte canonica
- `glossario.md`: Backcasting, Classificazione delle derive, Decision Log, Futuri generici, Futuro preferibile, Scheda di soglia

**Modificato**
- `workshops/worldbuilding-collaborativo.md`: quattro scenari con regola di costruzione (futuri generici, megatrend chiusi, uno scenario contro il valore più forte, uno inverosimile alla prima lettura, orizzonte a 10–15 anni), quattro team con partecipanti esterni, white spaces etichettati come trend o controtrend
- `workshops/archeologia-brand.md`: corpus da documenti, interviste strategiche, futuri ufficiali, controesempi, misura del cambiamento; Value Stress Test sulla forma operativa, giudicato da chi non ha costruito gli scenari, con Causal Layered Analysis come secondo metodo
- `workshops/brief-sotto-stress.md`: incontri preliminari con scheda di soglia, esercizio d'apertura e regole di parola; chiusura con consenso scritto su domanda di ricerca, finestra temporale e regole di lavoro
- `workshops/mappa-segnali-deboli.md`: griglia dichiarata con la domanda di ricerca al centro; raccolta umana, AI sulle correlazioni
- `workshops/dal-prototipo-al-protocollo.md` (ora 4 ore): futuro preferibile e backcasting prima del protocollo; criteri come ipotesi con effetto atteso e data di revisione
- `workshops/calibrazione-radar.md`: soglie che pendono verso la riapertura, combinazioni di indicatori, tempi di escalation legati alla velocità dei segnali, classificazione delle derive
- `workshops/audit-memoria.md`, `workshops/confrontation-brand-nei-futuri.md`, `workshops/overview.md`: allineati a quattro scenari, Decision Log e nuove durate
- `bos/02_futures.md`, `bos/03_identity.md`, `bos/05_strategy.md`, `bos/06_governance.md`, `bos/memory-architecture.md`: allineati ai workshop
- `foundations/metodo-e-bos.md`: tabella su `specula-method` 2.0, durate aggiornate (circa 27 ore), nota sull'ordine delle fasi
- `bos/04_exploration.md`, `foundations/lignaggio.md`: quattro scenari
- `foundations/four-stages.md`, `engagement/brand-nuovo.md`, `engagement/guardian-loop.md`, `governance/definition-of-done.md`, `governance/brand-governance-playbook.md`: quattro scenari, sottrazione tra identità possibili in Brand Nuovo, Guardian come revisione esterna che presuppone l'autonomia, classificazione delle derive
- `ecosistema.md`, `risorse.md`: versioni di riferimento e versione del manuale

**Corretto**
- `governance/definition-of-done.md`: il link al modello Guardian puntava a un percorso dell'archivio
- `bos/05_strategy.md`: refuso

**Note**
- Il Workshop Kit su FigJam va aggiornato su questa versione: regola di costruzione nel WS2, giudice esterno e forma operativa nel WS3, consenso scritto nel WS0, futuro preferibile e criteri come ipotesi nel WS5

### Workshop pilota Carta di Allineamento e porta specula.design · 2026-09-26

**Aggiunto**
- `workshops/carta-allineamento.md`: undicesimo workshop, pilota, binario AX. Documenta il protocollo con cui il Layer 08 · Agent Experience costruisce le sue Brand Policy, Skills e Contracts. Non fa parte del metodo in sei fasi
- `ecosistema.md`: riga su specula.design come porta per chi decide e acquista, con rimando al manuale per chi facilita e integra

**Modificato**
- `workshops/overview.md`: la tabella e l'introduzione registrano l'undicesimo workshop pilota
- `bos/08_agent-experience.md`: rimando al nuovo workshop
- `docs.json`: `workshops/carta-allineamento` in navigazione

### Allineamento fasi, workshop e sito · 2026-09-26

**Modificato**
- `foundations/metodo-e-bos.md`: la mappatura canonica aggiunge la colonna dei workshop con le durate, per ogni fase. La fase 5 comprende Calibrazione del Radar (con la configurazione del Guardian Loop) e Matrice Comportamentale; la fase 6 comprende Onboarding dell'Agent
- `foundations/metodo-e-bos.md`: nuova sezione "Ordine dei workshop e ordine delle fasi". Chiarisce che la prima Matrice Comportamentale si svolge a chiusura del Full Journey e appartiene alla fase 5; Audit della Memoria e Matrice diventano poi ricorrenti nel Guardian Loop
- `foundations/metodo-e-bos.md`: le componenti trasversali sono tre (Ethical Frame, Memory Architecture, Circolo di Sintesi), allineate a `bos/overview`. La versione precedente ne elencava due

**Note**
- Il sito di Specula (oggi marcolivi.it/specula; pagine Metodo, Servizi, Casi, Test della tensione) è allineato a questa versione: sei fasi con i workshop corrispondenti, Refusal Register come termine unico
- Il Workshop Kit su FigJam (undici canvas, stato pilota, testato a ritroso su due progetti reali) implementa i protocolli dei workshop 0–9 e il WS10, Carta di Allineamento (binario AX, 3 h), documentato nella voce successiva di questo changelog. Il kit resta un materiale di lavoro: le modifiche ai protocolli passano prima da questo manuale

### Revisione strutturale ed editoriale · 2026-06-10

**Aggiunto**
- `quickstart.md`: percorsi di lettura per decisori, professionisti, integratori
- `ecosistema.md`: mappa dei cinque repository, licenze, versioni documentate
- `foundations/metodo-e-bos.md`: mappatura canonica 6 fasi del metodo ↔ 7 layer del BOS, equivalenze terminologiche
- `glossario.md`: terminologia canonica IT/EN allineata a `specula-framework/specs/terminology.md`
- `engagement/caso-studio.md`: Il posto delle fragole (da `specula-method`)
- README.md, LICENSE.md, CONTRIBUTING.md, CODE_OF_CONDUCT.md, SECURITY.md, template issue (.github)

**Modificato**
- Homepage `index` aggiunta alla navigation (prima il sito serviva il template di default)
- Tutti i link interni riscritti come percorsi assoluti Mintlify (17+ link rotti corretti)
- Rimossi gli H1 duplicati dal body di tutte le pagine; aggiunta `description` al frontmatter di ogni pagina
- I 10 workshop riscritti come protocolli replicabili: preparazione, agenda con tempi, criteri di riuscita, errori comuni, destinazione degli output
- `workshops/overview.md` e `engagement/overview.md` trasformati da stub a pagine di orientamento con tabelle comparative
- `risorse.md`: tabella licenze corretta (method/framework BY-SA, skill MIT), aggiunto `specula-skill`, URL spostato da `09_Risorse/01_risorse` a `risorse`
- Note interne "Da scrivere. Fonte:" convertite in note di fonte canonica a piè di pagina

**Rimosso**
- Doppio albero dei contenuti: le cartelle numerate `01_…08_` spostate in `00_Meta/archive/` (la struttura pubblicata è l'unica fonte)
- `bos/seven-layers.md` (stub orfano, archiviato)

---

## [2026.06] · 2026-06-08

### Prima versione pubblica

**Aggiunto**
- Struttura completa del manuale in 9 sezioni
- `01_Introduzione`: Cos'è Specula, mito e filtro, a chi serve, come usare il manuale
- `02_Fondamenti`: Tesi sottrattiva, movimento in quattro tappe, condizioni della soglia
- `03_BOS`: Overview del Brand Operating System, architettura 7 layer, VEDERE·SCEGLIERE·RESTARE
- `04_I_Sette_Layer`: Tutti e 7 i layer in prosa operativa completa + Layer 08 Agent Experience
- `05_Ethical_Frame_e_Memoria`: Ethical Frame, Refusal Register, Memory Architecture, Circolo di Sintesi, Brand Governance Playbook
- `06_Workshop`: 10 protocolli completi (Brief sotto stress + uno per layer + Audit Memoria + Matrice Comportamentale)
- `07_Modelli_di_Ingaggio`: Full Journey, Specula Audit, Brand Nuovo, Specula Guardian
- `08_Definition_of_Done`: Criteri di completamento del mandato
- `09_Risorse`: Bio autore, repository GitHub, contributing, licenza CC BY-NC-SA 4.0, versioning
- `index.mdx`: Homepage italiana del sito Mintlify

**Note**
- Lingua: italiano (versione inglese pianificata per versione successiva)
- Hosting: [speculafuturecrafting.mintlify.app](https://speculafuturecrafting.mintlify.app)
- Repository: [oddtitoreal/specula-handbook](https://github.com/oddtitoreal/specula-handbook)
