# Specula Handbook

Il manuale di riferimento del metodo **Specula**: come portare un'organizzazione attraverso un cambiamento identitario, togliendo quello che copre, non aggiungendo quello che manca.

**📖 Leggi il manuale:** [speculafuturecrafting.mintlify.app](https://speculafuturecrafting.mintlify.app)

## Cosa c'è qui

Questo repository contiene i sorgenti del manuale, pubblicato con [Mintlify](https://mintlify.com). Il manuale documenta:

- i **fondamenti** del metodo (tesi sottrattiva, quattro tappe, condizioni della soglia);
- il **Brand Operating System**: l'architettura a 7 layer con Ethical Frame e Memory Architecture;
- i **modelli di ingaggio** (Audit, Full Journey, Brand Nuovo, Guardian Loop);
- i **dieci workshop** in forma di protocolli replicabili;
- la **governance** (Brand Governance Playbook, Refusal Register, Definition of Done).

## Ecosistema Specula

| Repository | Ruolo | Licenza |
|---|---|---|
| `specula-handbook` (questo repo) | Il manuale di riferimento | CC BY-NC-SA 4.0 |
| [`specula-method`](https://github.com/oddtitoreal/specula-method) | Il processo: metodo in sei fasi, facilitazione, etica | CC BY-SA 4.0 |
| [`specula-bos`](https://github.com/oddtitoreal/specula-bos) | Il prodotto: architettura dei 7 layer | CC BY-NC-SA 4.0 |
| [`specula-framework`](https://github.com/oddtitoreal/specula-framework) | La specifica runtime: schemi, contratti, validazione | CC BY-SA 4.0 |
| [`specula-skill`](https://github.com/oddtitoreal/specula-skill) | L'implementazione: constitution, state machine | MIT |

La mappa completa è nella pagina [Ecosistema](https://speculafuturecrafting.mintlify.app/ecosistema) del manuale.

## Struttura del repo

```
specula-handbook/
├── docs.json            · configurazione Mintlify (navigazione, tema)
├── index.mdx            · homepage
├── introduction.md      · cos'è Specula
├── quickstart.md        · percorsi di lettura
├── ecosistema.md        · mappa dei repository
├── foundations/         · fondamenti del metodo
├── bos/                 · Brand Operating System (7 layer + trasversali)
├── engagement/          · modelli di ingaggio + caso studio
├── workshops/           · i 10 protocolli operativi
├── governance/          · Playbook, Refusal Register, Definition of Done
├── risorse.md           · autore, libro, licenza, versioning
├── glossario.md         · terminologia canonica IT/EN
└── 00_Meta/             · materiali di lavoro interni (non pubblicati in navigazione)
```

## Contribuire

I contributi sono benvenuti: correzioni, chiarimenti, traduzioni, note dal campo. Leggi [CONTRIBUTING.md](CONTRIBUTING.md). Le modifiche al metodo in sé evolvono nei repo `specula-method` e `specula-bos`, non qui.

## Sviluppo locale

```bash
npm i -g mint
mint dev
```

Anteprima su `http://localhost:3000`.

## Versioning

Versioning basato sulla data: `YYYY.MM`. Versione corrente: **2026.06**. Le modifiche sono documentate nel [CHANGELOG](CHANGELOG.md). Le versioni dei repo documentate da questa edizione del manuale sono indicate nella pagina [Ecosistema](https://speculafuturecrafting.mintlify.app/ecosistema).

## Licenza

[CC BY-NC-SA 4.0](LICENSE.md), © Marco Livi / Specula Future Crafting.
Il libro *Fantasticare il futuro* è il mito fondativo del metodo; questo manuale è il filtro operativo.
