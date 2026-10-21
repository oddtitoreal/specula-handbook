---
title: "Decision Log"
description: "Il registro delle decisioni con il criterio applicato, l'effetto atteso e la data di revisione: i valori restano fermi, i criteri si mettono alla prova."
---
I valori del DNA restano fermi. I criteri che li traducono in decisioni sono ipotesi: possono essere sbagliati, e il sistema deve poterlo scoprire. Il Decision Log è lo strumento con cui lo scopre.

Si apre nel workshop [Dal Prototipo al Protocollo](/workshops/dal-prototipo-al-protocollo), insieme al Protocollo Strategico, e vive nella **Decision Memory** della [Memory Architecture](/bos/memory-architecture).

## Struttura di una voce

| Data | Decisione | Criterio applicato | Effetto atteso | Data di revisione | Effetto osservato |
|---|---|---|---|---|---|
| | | | | | |

L'effetto atteso si scrive prima della decisione: senza quel termine di confronto, l'effetto osservato non permette di correggere il criterio.

Le posizioni di minoranza emerse nella delibera restano visibili accanto alla voce.

## La revisione

Alla data di revisione il Circolo confronta effetto atteso ed effetto osservato. Il criterio viene **confermato**, **rivisto** o **ritirato**. L'[Audit della Memoria](/workshops/audit-memoria) trimestrale verifica che nessuna revisione sia rimasta indietro.

I criteri nuovi si provano con esperimenti progettati per poter fallire senza danni.

## Classificazione delle derive

Il Guardian legge le derive anche attraverso il Decision Log. Ogni deriva riceve una classe, con la regola che l'ha prodotta:

| Classe | Regola | Azione |
|---|---|---|
| **Errore** | La deriva viola una red line | Correzione |
| **Modello superato** | Il mondo osservato esce da tutti gli scenari | [Re-Speculation](/engagement/guardian-loop) |
| **Apprendimento** | La deriva è ripetuta, spontanea e diffusa, e non viola red line | Il Circolo delibera se il criterio che la contraddice va cambiato |

La classe "apprendimento" permette a un'identità di restare coerente senza irrigidirsi: le etichette dei valori restano, il modo di tradurle in decisioni impara dall'esperienza.

## Le metriche che ne derivano

- **Brand Coherence Index**: ogni trimestre si estrae un campione di decisioni dal Decision Log; due valutatori indipendenti le collocano nella [Matrice Comportamentale](/workshops/matrice-comportamentale). L'indice è la quota di decisioni che entrambi collocano come Ammesse, riportata insieme al grado di accordo tra i valutatori: se l'accordo è basso, va prima rivista la matrice.
- **Learning Velocity**: criteri rivisti nel trimestre, con effetto atteso e osservato confrontati.

---

*Fonti canoniche: [`specula-bos/docs/05_memory-architecture.md`](https://github.com/oddtitoreal/specula-bos/blob/main/docs/05_memory-architecture.md) · [`specula-method/docs/method-overview.md`](https://github.com/oddtitoreal/specula-method/blob/main/docs/method-overview.md) · [`specula-framework/schemas/decision_log.schema.json`](https://github.com/oddtitoreal/specula-framework/blob/main/schemas/decision_log.schema.json)*
