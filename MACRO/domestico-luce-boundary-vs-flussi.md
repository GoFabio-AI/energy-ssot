# Macro, boundary SSOT vs layer flussi

Snapshot SSOT: 2026-04-15

## Perché esiste questa nota
Il package `domestico luce` è chiuso al boundary SSOT, ma questo non significa che il repo contenga già una process architecture completa del settore o un catalogo esaustivo di tutti i flussi implementativi.

Questa nota serve a separare due cose diverse:
- `baseline SSOT chiuso`
- `layer flussi/processi/ERP` ancora costruibile sopra il baseline

## Cosa è già chiuso nel repo
Il repo chiude il tratto minimo normativo-operativo riusabile per il domestico luce al `2026-04-15`.

In pratica sono già chiusi:
- regimi e segmentazione (`vulnerabili`, `non vulnerabili`, `MT`, `STG`, `mercato libero`)
- attori e ruoli minimi (`SII`, `RCU`, `AU`, venditore, distributore, UdD, controparte commerciale)
- processi customer-facing principali (`switching`, `voltura`, `subentro`, `disattivazione`, `allacciamento/attivazione` nel boundary coperto)
- misure, autoletture, stime, ricostruzioni e visibilità cliente dei dati
- fatturazione, bolletta 2025, `Elementi di dettaglio`, prescrizione, reclami importi fatturati
- pagamenti, garanzie, deposito, rateizzazione regolata
- morosità, sospensione, riattivazione, `CMOR`, clienti non disalimentabili e ultima istanza
- reporting regolatorio, intake, registri, call center, pubblicazioni e reporting di misura
- bonus sociale, fiscalità domestica di base, contratti e trasparenza commerciale

## Cosa NON significa la chiusura del baseline
La chiusura del baseline non implica che il repo contenga già, in forma esaustiva:
- una mappa completa `attore -> trigger -> input -> output -> SLA -> esito -> eccezioni`
- BPMN o state machine complete di tutti i processi di settore
- un catalogo completo di tutti i messaggi o tracciati operativi `SII`
- scraping esaustivo di ogni pagina secondaria, FAQ o specifica tecnica esistente
- una process architecture ERP-ready completa per tutti i use case
- decision table applicative complete per ogni edge case implementativo

In altre parole, il repo oggi è forte sul `cosa è vero`, `cosa è consentito affermare`, `quale boundary è chiuso`, più che sul `come modellare ogni processo software end-to-end`.

## Cosa esiste già come ponte verso quel livello
Il repo però non parte da zero sul layer operativo:
- `MACRO/domestico-luce-capability-map.md` traduce il baseline in `sapere / fare / decidere`
- `MACRO/domestico-luce-handoff-fatturazione-ai-dev.md` prepara un handoff diretto verso coding agent sul tratto billing
- i domini `switching`, `voltura-subentro-cessazione`, `anagrafica-tecnica-pod-accessi-reporting`, `misure`, `fatturazione`, `morosita-cmor` e `reporting-regolatorio` contengono già gran parte dei trigger e boundary minimi necessari per costruire flussi applicativi sopra il SSOT

## Prossimo layer naturale sopra il repo attuale
Se si vuole andare oltre il baseline SSOT, il next step sensato non è “aggiungere altri fatti casuali”, ma costruire un layer dedicato ai flussi.

### Possibile workstream successivo
`domestico-luce-flussi-operativi`

### Deliverable tipici di quel layer
- flow catalog per use case
- matrice `attore / trigger / prerequisiti / input / output / SLA / eccezioni`
- state machine dei processi principali
- mapping più profondo delle specifiche `SII`
- decision table ERP o product-ready
- distinzione esplicita tra `regola SSOT`, `assunzione tecnica`, `decisione prodotto`

## Regola da tenere ferma
Quel layer successivo deve riusare il repo come base, non sostituirlo.

Quindi:
- il `SSOT` continua a stare in `DOMAINS/`, `RULES/`, `EXTRACTED/`, `CITATIONS/`
- i flussi applicativi devono referenziare il SSOT, non reinventarlo
- se un flusso richiede una scelta non chiusa dal SSOT, la scelta va in `DECISIONS/`

## Dove leggere per capire il confine
- [../README.md](../README.md)
- [../INDEX.md](../INDEX.md)
- [../COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md](../COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md)
- [domestico-luce-capability-map.md](domestico-luce-capability-map.md)
- [domestico-luce-handoff-fatturazione-ai-dev.md](domestico-luce-handoff-fatturazione-ai-dev.md)
