---
title: "Onboarding dell'Agent"
description: "2 ore per caricare il DNA del brand nello Specula Agent e testarne il supporto decisionale su casi reali."
---

**Layer:** [07 · INTERFACE](/bos/07_interface)
**Durata:** 2 ore
**Prerequisito:** Brand Radar configurato e Strategic Protocol completato

---

## Obiettivo

Configurare lo Specula Agent con il DNA del brand e testare la qualità del suo supporto decisionale su decisioni reali già prese. L'Agent non decide: segnala coerenza e drift, con motivazione.

## Quando si usa

Alla fine del percorso, quando tutti gli artefatti sono validati. Ripetibile quando il DNA o il Protocollo vengono aggiornati in modo sostanziale.

## Partecipanti e ruoli

Il Circolo di Sintesi. **Sessione tecnica: richiede accesso al sistema** e una figura in grado di modificare prompt e memoria dell'Agent in sessione.

## Preparazione

- Gli artefatti da caricare: Speculative Brand DNA, Refusal Register (prime voci), Strategic Protocol, scenari divergenti di riferimento.
- **Cinque decisioni reali** affrontate dall'organizzazione negli ultimi sei mesi, documentate con il contesto che c'era al momento della scelta.
- Ambiente di test dell'Agent separato da quello operativo.

## Svolgimento

**1 · Caricamento** (30 min) — Il Brand Alchemist carica nella memoria dell'Agent i quattro artefatti. Ogni caricamento viene verificato con una domanda di controllo ("quali sono le red lines?").

**2 · Test su casi reali** (60 min) — Il team presenta all'Agent le cinque decisioni reali. Per ciascuna si valuta:
   - l'Agent avrebbe segnalato coerenza o drift?
   - con quale motivazione?

   Le risposte vengono confrontate con le decisioni effettivamente prese e con il giudizio retrospettivo del Circolo.

**3 · Affinamento** (20 min) — Le divergenze diventano materiale per correggere prompt e memoria: una divergenza può rivelare un errore dell'Agent, ma anche un drift reale che il Circolo non aveva visto. Entrambi i casi vanno verbalizzati.

**4 · Approvazione** (10 min) — Il Circolo approva formalmente la configurazione prima che l'Agent diventi operativo. Senza approvazione esplicita, l'Agent resta in test.

## Criteri di riuscita

- L'Agent motiva ogni segnalazione risalendo a un valore, una red line o un criterio del Protocollo: mai "non è in linea col brand" senza riferimento.
- Almeno una divergenza è stata analizzata fino alla causa (errore di configurazione o drift reale).
- La prompt architecture è documentata: un terzo potrebbe ricostruire la configurazione.

## Errori comuni

- Testare l'Agent su casi ipotetici invece che su decisioni reali già prese: solo il confronto con la storia rivela la qualità del giudizio.
- Trattare ogni divergenza come errore dell'Agent: a volte ha ragione lui.
- Renderlo operativo senza approvazione formale del Circolo.

## Output e destinazione

**Specula Agent operativo**, testato su casi reali e approvato, con **prompt architecture documentata**. È l'interfaccia quotidiana del BOS; le sue segnalazioni alimentano la **Decision Memory** e il [Brand Radar](/bos/06_governance).
