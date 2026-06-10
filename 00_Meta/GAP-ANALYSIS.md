# Gap Analysis — Specula Handbook

Analisi del manuale (sito Mintlify + repo `specula-handbook`) rispetto all'ecosistema GitHub: `specula-framework` (v1.2.0), `specula-method` (v1.0), `specula-skill` (v0.1.2), `specula-bos` (v2.0).
Obiettivo: cosa manca perché il manuale sia leggibile e gestibile da tutti come riferimento del metodo open source.

Data: 2026-06-10

---

## Sintesi

Il manuale è ben scritto ma oggi documenta **solo il BOS**, non l'intero metodo. I quattro repo raccontano un ecosistema a tre/quattro strati (framework → method → skill → bos) che il manuale non mappa, e in più punti lo **contraddice** (numero di fasi, licenze, modelli di ingaggio, versioni). Sul piano tecnico, il sito pubblicato ha homepage rotta, link interni rotti e pagine orfane; il repo non ha README, LICENSE né infrastruttura di contribuzione, pur dichiarando di averla.

Tre categorie di lavoro, in ordine di gravità: **A. Allineamento con i repo** (sostanza), **B. Bug di pubblicazione** (leggibilità), **C. Igiene open source** (gestibilità).

---

## ✅ Risolto — Sicurezza (2026-06-10)

Il remote git locale conteneva un **GitHub Personal Access Token in chiaro** nell'URL. Token revocato dall'autore e remote ripulito (`https://github.com/oddtitoreal/specula-handbook.git`). Per i prossimi push: usare un credential manager, SSH o un fine-grained PAT con scope limitato a questo repo.

---

## A. Allineamento manuale ↔ ecosistema repo (il gap più grave)

### A1. Sei fasi vs sette layer — mai riconciliati
`specula-method` definisce il metodo in **6 fasi** (1 Scenario Generation, 1.5 Competitive Futures Mapping, 2 Brand Archeology, 3 Future Prototyping & Ethical Gate, 4 Narrative Synthesis, 5 Co-creation, 6 Activation & Guardian). `specula-framework` ha contratti JSON "for all 6 phases". Il manuale parla solo di **7 layer** (WORLD → … → INTERFACE).
Un lettore che arriva dai repo e poi apre il manuale crede di leggere due metodi diversi. **Manca una pagina di mappatura fasi ↔ layer** (e la Fase 1.5 — Competitive Futures Mapping — non esiste da nessuna parte nel manuale).

### A2. Il manuale non copre tre repo su quattro
- `specula-framework` (runtime, schemi JSON, agente eseguibile `specula-agent`, precedence, versioning): citato solo di sfuggita in Risorse. Manca una sezione "Per chi integra" che spieghi cosa ci si trova e quando serve.
- `specula-method` (le 6 fasi, Speculative Identity Model/Canvas, Resilience Protocol, Alumni Network, Certificazione Practitioner, case study *Il posto delle fragole*): nulla di tutto questo è nel manuale.
- `specula-skill` (constitution, state-machine, validatore): **assente perfino dalla tabella repo in Risorse** (c'è in 00_Meta ma non nella pagina pubblicata).

### A3. Licenze dichiarate ≠ licenze reali
La pagina Risorse dichiara:

| Repo | Manuale dice | Repo dice realmente |
|---|---|---|
| specula-method | CC BY-NC-SA 4.0 | **CC BY-SA 4.0** |
| specula-skill | (non citato) | **MIT** |
| specula-bos | CC BY-NC-SA 4.0 | **nessun file LICENSE nel repo** |
| specula-framework | CC BY-SA 4.0 | CC BY-SA 4.0 ✓ |

Da correggere in Risorse; e `specula-bos` ha bisogno di un LICENSE.

### A4. Versioni incoerenti, manuale fuori dal sistema di allineamento
I repo hanno `VERSIONS.md` e `ALIGNMENT.md` che governano la coerenza reciproca (framework 1.2.0 · method 1.0 · skill 0.1.2) — ma la matrice copre "three repositories": **né `specula-bos` né il manuale ne fanno parte**. Inoltre `specula-bos` dichiara "Framework: Specula v2.4.5" che non corrisponde a nessuna versione pubblicata. Il manuale (2026.06) non dice **quale versione** del metodo/framework documenta. Serve: riga del handbook in VERSIONS.md + nota di versione nel manuale ("documenta method v1.0 / framework v1.2.x / bos v2.0").

### A5. Terminologia divergente
Stesso concetto, nomi diversi a seconda della fonte: *Refusal Register* (manuale/bos) vs *Registry of Refusals* (method); *Guardian Loop* (manuale) vs *Specula Guardian* (method/bos); 4 modelli di ingaggio nel manuale (con **Brand Nuovo**) vs 3 in method e bos (Brand Nuovo non esiste nei repo). `specula-framework` ha `specs/terminology.md` come standard canonico: il manuale dovrebbe dichiararvi conformità e includere un **glossario** bilingue IT/EN.

### A6. Visibilità incrociata assente
Nessuno dei quattro repo linka il manuale (le tabelle "SPECULA Ecosystem" non lo menzionano). Chi parte da GitHub non scoprirà mai il sito. Aggiungere il handbook alle tabelle ecosistema dei repo e, viceversa, una pagina "Ecosistema" nel manuale con la tabella dei 4 repo + ruoli + licenze + entry point.

### A7. Contenuti dei repo che il manuale dovrebbe riusare
- Il **case study reale** (*Il posto delle fragole*, già pubblico in IT e EN in specula-method) — il manuale non ha nemmeno un esempio applicato.
- I **template** (Speculative Identity Canvas, Registry of Refusals, Brand Governance Playbook in specula-bos/templates) — il manuale li descrive ma non li linka né li offre in download.
- I **QUICKSTART** EN/IT dei repo — il manuale non ha un percorso "inizia qui in 10 minuti".

---

## B. Sito pubblicato — bug che bloccano la lettura

1. **Homepage rotta.** `speculafuturecrafting.mintlify.app/` serve il template di default Mintlify ("Product Guide", link a /platform, /analytics inesistenti) invece di `index.mdx`. Probabile causa: la home non è raggiungibile dalla navigation in `docs.json`. È la prima cosa che vede chiunque.
2. **17+ link interni rotti.** Le pagine pubblicate contengono link relativi ai vecchi percorsi numerati (`../06_Workshop/01_mappa-segnali-deboli.md`, `../07_Modelli_di_Ingaggio/...`) che non esistono sul sito. Vanno riscritti come percorsi assoluti Mintlify senza estensione (es. `/workshops/mappa-segnali-deboli`).
3. **Titolo duplicato su ogni pagina.** Frontmatter `title:` + `# Titolo` nel body → l'H1 appare due volte. Rimuovere l'H1 dal body.
4. **Nessuna pagina ha `description` nel frontmatter** → SEO scarsa e descrizioni llms.txt generate automaticamente in inglese su un sito italiano.
5. **Pagine orfane e voci fantasma.** `bos/seven-layers.md` esiste ma non è in navigation (e contiene solo 3 righe); il gruppo Risorse usa il percorso interno `09_Risorse/01_risorse` (URL brutto e incoerente: dovrebbe essere `resources/...` o `risorse`).
6. **URL canonico sbagliato.** Le decisioni chiuse dicono `handbook.specula.design`, ma il canonical in docs.json punta a `.mintlify.app` e il dominio custom non è configurato.
7. **Workshop troppo magri per essere "protocolli".** Le pagine workshop pubblicate sono 150–320 parole: descrivono il workshop ma non lo rendono replicabile (manca agenda passo-passo, materiali, ruoli, template di output, criteri di riuscita). `specula-bos/workshops/` è la fonte dichiarata: o si sincronizza, o si linka.

---

## C. Repo `specula-handbook` — igiene open source

Confronto impietoso con `specula-framework`, che è lo standard di casa:

| Elemento | framework | method | skill | **handbook** |
|---|---|---|---|---|
| README.md alla radice | ✓ | ✓ | ✓ | **✗** (solo INDICE.md, che GitHub non mostra come README) |
| LICENSE | ✓ | ✓ | ✓ | **✗** (la licenza è solo dichiarata in una pagina) |
| CONTRIBUTING.md | ✓ | ✓ | — | **✗** |
| CODE_OF_CONDUCT.md | ✓ | ✓ | — | **✗** |
| SECURITY.md | ✓ | ✓ | — | **✗** |
| Template issue (.github) | ✓ | ✓ | ✓ | **✗** — ma la pagina Risorse **promette** template "Bug / Errore, Chiarimento, Traduzione, Nota dal campo" che non esistono |
| CI (link check, lint) | ✓ | ✓ | — | **✗** |
| Bilingue EN/IT | ✓ | ✓ | ✓ | **✗** (solo IT, ma la decisione chiusa diceva "bilingue dal lancio") |

Altri problemi interni:

- **Doppio albero dei contenuti.** Le cartelle numerate `01_…09_` duplicano le cartelle pubblicate (`foundations/`, `bos/`, `workshops/`…). `bos/` e `04_I_Sette_Layer` sono identiche oggi, ma in `06_Workshop` esistono già **tre versioni** dello stesso workshop (numerata, non numerata, pubblicata). È drift garantito. Decidere un'unica fonte (le cartelle pubblicate), spostare il vecchio albero in `00_Meta/archive/` o eliminarlo.
- **INDICE.md non aggiornato** (segna "da scrivere" sezioni già scritte e pubblicate).
- **`00_Meta/README.md` cita `DECISIONI.md` e `CHANGELOG.md` in 00_Meta** che non esistono lì.
- `.DS_Store` committato nonostante il .gitignore.

---

## D. Cosa manca per i tre pubblici dichiarati

Il manuale dichiara tre lettori (decisori, professionisti, studenti). Per ciascuno manca:

- **Decisori**: un caso reale (riusare Posto delle Fragole), una pagina "quanto costa/quanto dura" consolidata, FAQ.
- **Professionisti/facilitatori**: workshop replicabili (agende, materiali, template scaricabili), quickstart, mappatura fasi↔layer, glossario, certificazione (esiste in method, il manuale non la nomina).
- **Studenti/contributori/integratori**: pagina Ecosistema con i 4 repo, sezione sul runtime (framework + skill), CONTRIBUTING reale con i template promessi, versione inglese.

---

## Piano d'azione prioritizzato

**Subito (ore)**
1. Revocare il PAT e ripulire il remote.
2. Aggiungere `index` alla navigation / sistemare la homepage.
3. Correggere i 17+ link rotti e rimuovere gli H1 duplicati.
4. Correggere la tabella licenze in Risorse e aggiungere `specula-skill`.
5. Creare README.md e LICENSE alla radice del repo.

**Questa settimana**
6. Pagina "Ecosistema Specula" nel manuale (4 repo, ruoli, licenze, entry point) + link al handbook nei README dei repo.
7. Pagina di mappatura 6 fasi ↔ 7 layer + glossario terminologico (conforme a `specs/terminology.md`).
8. Eliminare il doppio albero dei contenuti; aggiornare INDICE.md.
9. CONTRIBUTING.md + template issue promessi in Risorse + CODE_OF_CONDUCT (riusare quelli di specula-method).
10. `description` nel frontmatter di tutte le pagine; URL Risorse pulito.

**Questo mese**
11. Arricchire i 10 workshop fino a protocolli replicabili (sincronizzati con specula-bos).
12. Integrare il case study e i template scaricabili.
13. Versione inglese (i18n Mintlify) — onorare la decisione "bilingue dal lancio".
14. Aggiungere handbook e bos a VERSIONS.md/ALIGNMENT.md; nota di versione nel manuale; chiarire "Brand Nuovo" (aggiungerlo ai repo o segnalarlo come estensione del manuale).
15. Dominio `handbook.specula.design` + canonical corretto; CI con link-checker.
