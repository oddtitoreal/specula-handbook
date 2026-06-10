---
title: "Ecosistema Specula"
description: "I quattro repository GitHub e questo manuale: chi fa cosa, con quale licenza, da dove entrare."
---

Specula è distribuito su quattro repository pubblici più questo manuale. Ogni oggetto ha un ruolo preciso: confonderli è il modo più rapido per perdersi.

## La mappa

| Oggetto | Ruolo | Per chi | Licenza |
|---|---|---|---|
| [**Specula Handbook**](https://github.com/oddtitoreal/specula-handbook) (questo sito) | Il manuale di riferimento: filosofia, architettura, protocolli, governance in forma leggibile | Tutti: decisori, professionisti, studenti | CC BY-NC-SA 4.0 |
| [`specula-method`](https://github.com/oddtitoreal/specula-method) | **Il processo**: il metodo in sei fasi, il framework etico, la facilitazione, i template, il case study | Strategist, designer, facilitatori | CC BY-SA 4.0 |
| [`specula-bos`](https://github.com/oddtitoreal/specula-bos) | **Il prodotto**: l'architettura dei 7 layer che il metodo costruisce, i workshop, la Memory Architecture | Chi progetta o governa un BOS | CC BY-NC-SA 4.0 (dichiarata) |
| [`specula-framework`](https://github.com/oddtitoreal/specula-framework) | **La specifica runtime**: schemi JSON delle sei fasi, contratti, agente eseguibile, terminologia canonica | Integratori, architetti di governance | CC BY-SA 4.0 |
| [`specula-skill`](https://github.com/oddtitoreal/specula-skill) | **L'implementazione**: constitution, state machine, validatore di artefatti di governance | AI engineer, implementatori | MIT |

In una frase: il **method** è come si lavora, il **BOS** è cosa si costruisce, il **framework** è come funziona a runtime, la **skill** è come lo si implementa in codice. Il manuale è la porta d'ingresso di tutto.

## Da dove entrare

- *Devo capire il metodo* → resta qui nel manuale, poi [`specula-method`](https://github.com/oddtitoreal/specula-method) per i materiali operativi.
- *Devo facilitare una sessione* → [Workshop](/workshops/overview) qui + i template e l'agent di facilitazione in `specula-method`.
- *Devo integrare Specula in un sistema* → [`specula-framework`](https://github.com/oddtitoreal/specula-framework), partendo dal suo Quick Start.
- *Devo implementare regole di governance in codice* → [`specula-skill`](https://github.com/oddtitoreal/specula-skill), con i contratti canonici del framework.

## Versioni documentate

Questo manuale (versione **2026.06**) documenta:

| Repo | Versione di riferimento |
|---|---|
| `specula-method` | v1.0 |
| `specula-framework` | v1.2.x |
| `specula-skill` | v0.1.x |
| `specula-bos` | v2.0 |

L'allineamento tra i repo è governato da `VERSIONS.md` e `ALIGNMENT.md` in `specula-framework`. Quando una versione di riferimento cambia, questo manuale lo registra nel [CHANGELOG](https://github.com/oddtitoreal/specula-handbook/blob/main/CHANGELOG.md).

## Nota sulle licenze

Le licenze sono deliberatamente diverse. Il manuale e il BOS usano **BY-NC-SA** perché descrivono il metodo come pratica professionale. Il framework e il method usano **BY-SA** (senza clausola non commerciale) per permettere l'integrazione tecnica e l'adozione del processo anche in contesti commerciali. La skill usa **MIT** perché è codice destinato a essere incorporato. Se trovi una discrepanza tra quanto dichiarato qui e i file LICENSE nei repo, fanno fede i repo: segnalala con una [issue](https://github.com/oddtitoreal/specula-handbook/issues).

## Cosa è aperto, cosa è proprietario

Aperto: l'architettura dei 7 layer, l'Ethical Frame, i protocolli workshop, la struttura della Memory Architecture, il Brand Governance Playbook, gli schemi e i validatori.

Proprietario: configurazioni AI e librerie di prompt, librerie di scenari, strumenti operativi di facilitazione, lavoro sui clienti.

Questa distinzione non è una riserva commerciale travestita: è ciò che rende il metodo verificabile senza renderlo banalizzabile. Chiunque può controllare *come* funziona Specula; applicarlo bene richiede il percorso, non il download.

→ Come le sei fasi del metodo costruiscono i sette layer: [Il Metodo e il BOS](/foundations/metodo-e-bos)
