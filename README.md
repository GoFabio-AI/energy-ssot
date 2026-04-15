# Energia SSOT

Repository di knowledge engineering per il dominio energia, costruito a partire da fonti ufficiali e pensato per trasformare normativa, regolazione e materiali quasi-ufficiali in regole riusabili per prodotto, ERP, operations e sviluppo software.

## Scopo
Essere la fonte di verità per domande normative, interpretazioni operative minime e decisioni applicative tracciabili.

## Stato rapido, luce domestica
Al `2026-04-15` il pacchetto `domestico luce` è chiuso al boundary SSOT.

Entry point consigliati:
- [INDEX.md](INDEX.md)
- [COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md](COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md)
- [ROADMAP-DOMESTICO-LUCE-POST-BASELINE-OPERATIONS.md](ROADMAP-DOMESTICO-LUCE-POST-BASELINE-OPERATIONS.md)
- [MACRO/domestico-luce-master-2026-04-15.md](MACRO/domestico-luce-master-2026-04-15.md)
- [MACRO/domestico-luce-capability-map.md](MACRO/domestico-luce-capability-map.md)
- [MACRO/domestico-luce-boundary-vs-flussi.md](MACRO/domestico-luce-boundary-vs-flussi.md)
- [MACRO/domestico-luce-handoff-fatturazione-ai-dev.md](MACRO/domestico-luce-handoff-fatturazione-ai-dev.md)

## Come leggere la repo
- Parti da `INDEX.md` per capire copertura, domini e stato del package.
- Usa `COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md` come manifest finale di chiusura e handoff.
- Leggi i file in `MACRO/` se vuoi una vista umana e compatta.
- Scendi nei `DOMAINS/` quando ti serve il boundary SSOT operativo.
- Usa `RULES/`, `EXTRACTED/` e `CITATIONS/` quando devi verificare o implementare il dettaglio atomico.

## Struttura del repo
- `DOMAINS/`: package di dominio SSOT
- `RULES/`: regole atomiche riusabili
- `EXTRACTED/`: estrazioni normalizzate dalle fonti
- `CITATIONS/`: citazioni verificabili e riferimenti puntuali
- `MACRO/`: documenti leggibili, master docs e handoff
- `DECISIONS/`: decisioni prodotto o applicative separate dal SSOT
- `RAW/`: materiale grezzo conservato dove serve

## Regole base
- usare solo fonti ammesse
- non scrivere fatti senza citazione
- non trattare bozze o dubbi come verità
- tenere separate regole e decisioni
- se un caso non è coperto, lasciarlo come gap esplicito o decisione separata

## A cosa serve bene
- supportare agenti o team che devono implementare logica regolatoria senza inventare regole
- fare handoff verso coding agent con file e vincoli chiari
- mantenere separati fatti normativi, interpretazione minima e decisioni prodotto
- creare una base verificabile per billing, care, operations, pricing e compliance

## Cosa il repo non pretende ancora di essere
- non è ancora un catalogo esaustivo di tutti i flussi operativi di settore
- non è ancora una process architecture completa `ERP-ready`
- non è ancora una raccolta completa di BPMN, state machine o mapping profondo di tutti i messaggi `SII`
- per questo confine vedi `MACRO/domestico-luce-boundary-vs-flussi.md`
- per il backlog operativo successivo vedi `ROADMAP-DOMESTICO-LUCE-POST-BASELINE-OPERATIONS.md`

## Standard modello
Per questo workstream usare GPT-5.4 con reasoning xhigh.
