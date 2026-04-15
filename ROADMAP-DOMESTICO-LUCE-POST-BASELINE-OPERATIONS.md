# Roadmap post-baseline, domestico luce, operational depth

Data di riferimento: 2026-04-15

## Scopo
Questa roadmap non riapre il baseline `domestico luce` già chiuso al boundary SSOT.

Serve a registrare in modo esplicito il layer successivo di lavoro che manca ancora per passare da:
- `baseline normativa-operativa minima chiusa`

al livello:
- `process architecture / operational depth / ERP-ready`

In altre parole, questo file elenca i gap residui seri che non negano la chiusura del baseline, ma impediscono di considerare il repo una mappa industriale completa del dominio.

## Regola di lettura
- Se un punto qui sotto manca, non significa automaticamente che il SSOT sia falso o incoerente.
- Significa che il repo non ha ancora trasformato il SSOT in un layer completo di flussi, stati, tracciati, eccezioni o artefatti implementativi.
- Le nuove aggiunte a questo layer devono sempre referenziare `DOMAINS/`, `RULES/`, `EXTRACTED/` e `CITATIONS/`, senza reinventare le regole.

## Regole metodologiche critiche per il layer SII / processi
- Non basta prendere un PDF utile o parseabile: per ogni processo va cercata prima la sezione `Documenti in vigore` della pagina ufficiale SII o AU pertinente.
- La selezione della fonte deve privilegiare la **versione vigente più recente** della famiglia documentale corretta, non una versione storica solo perché facile da estrarre.
- La regola non è `PDF-first` in senso dogmatico ma `official-source-first`: usare PDF, HTML o pagina normativa ufficiale a seconda di quale sia la fonte migliore e più aggiornata per quel fatto.
- Su una singola pagina SII spesso esistono più documenti utili nello stesso tempo: documento di funzionamento del processo, specifiche tecniche, allegati `All.A` o `All.B`, guida `PdC`, OpenAPI o WSDL, errata o EC. Non va scelto un singolo file a caso.
- Per ogni processo SII va modellato un **document set** minimo, distinguendo almeno tra: documento core di processo, allegati strutturali o codifiche, interfacce o tracciati, supporti operativi o di utilizzo.
- Le versioni precedenti vanno trattate come storico o superseded, non come baseline attiva, salvo uso esplicito per diff o retrospettiva.
- Ogni ingestione deve registrare almeno: famiglia documentale, ruolo del file nel processo, versione, data, URL, motivo della scelta e verifica che sia o meno l'ultima versione vigente visibile.

## Stato complessivo
- baseline `domestico luce`: **chiuso al boundary SSOT**
- operational depth / flows layer: **non ancora coperto in modo completo**

## Macro-gap residui prioritari

| Priorità | Area | Stato | Perché conta | Deliverable atteso |
| --- | --- | --- | --- | --- |
| P0 | flow catalog end-to-end | aperto | oggi il repo chiude verità e boundary, ma non una mappa completa `attore -> trigger -> input -> output -> SLA -> eccezioni` | catalogo flussi per use case domestico luce |
| P0 | state machine processi core | aperto | senza stati e transizioni esplicite è difficile costruire automazioni o ERP robusti | state machine per switching, voltura, subentro, disattivazione, morosità, billing |
| P0 | mapping profondo specifiche SII | aperto | il repo copre i processi minimi e diversi punti SII, ma non un mapping sistematico di messaggi, esiti, precedenze, controlli e scarti | package `SII deep operations` |
| P1 | PDO / anagrafica tecnica estesa | aperto | oggi è chiuso solo il set minimo customer-facing e operator-facing ordinario, non la mappa estesa di campi, eventi e uso applicativo | catalogo attributi POD/PDO con source boundary |
| P1 | 2G / PDO2G / misura avanzata | aperto | il repo chiude il boundary retail minimo, ma non il layer profondo di rollout, capability metering e impatto applicativo | slice dedicato `2G / metering depth` |
| P1 | ERP handoff completo | aperto | esiste un handoff billing, ma non ancora un handoff completo per tutti i cluster di processo | pacchetti handoff per processi core |
| P1 | decision tables prodotto/ops | aperto | senza tabelle decisionali resta troppo implicito il ponte tra regola e comportamento software | decision tables per intake, routing, eccezioni |
| P2 | BPMN o flow diagrams | aperto | utile per onboarding team e governance, ma viene dopo il flow catalog testuale | diagrammi o BPMN derivati dal flow catalog |
| P2 | inventory completo edge cases | aperto | diversi edge cases sono già nei domini, ma non esiste ancora una raccolta unica per implementazione | matrice edge cases domestico luce |

## Workstream suggeriti

### WS1. Flow catalog domestico luce
#### Obiettivo
Costruire il catalogo dei flussi end-to-end minimi per i casi principali.

#### Use case minimi da coprire
- switching su POD attivo
- voltura su POD attivo
- subentro su POD disattivo
- disattivazione/cessazione
- allacciamento + attivazione nel boundary BT coperto
- ciclo misura -> fattura -> pagamento -> reclamo billing
- mora -> riduzione potenza -> sospensione -> riattivazione -> CMOR
- bonus sociale economico da DSU a sconto in fattura
- intake reclami / richieste informazioni -> registro -> reporting TIQV

#### Deliverable atteso
Per ogni flusso:
- trigger
- attori coinvolti
- prerequisiti
- input minimi
- passaggi
- output
- SLA / tempi
- eccezioni e blocchi
- regole SSOT richiamate

### WS2. SII deep operations
#### Obiettivo
Approfondire il layer processuale e tecnico `SII` oltre il boundary già chiuso nel baseline.

#### Target principali
- messaggi/processi `SE`, `RC`, `UI`, `VS`, `AV`, `DS`, `PK`, `CDT`
- esiti e precedenze
- compatibilità/incompatibilità tra pratiche
- eventi di aggiornamento `RCU`
- mapping riusabile per ERP e automazioni
- ricostruzione del `document set` vigente per ciascun processo, non solo del PDF principale

#### Deliverable atteso
- matrice processi `SII`
- matrice esiti/scarti/precedenze
- note operative separate dal SSOT normativo
- registro per processo di `documenti in vigore` con classificazione `core / allegato / interfaccia / supporto operativo`

### WS3. POD / PDO / 2G / metering depth
#### Obiettivo
Colmare il layer profondo sugli oggetti tecnici del punto e sui dati di misura evoluti, che oggi nel repo sono chiusi solo nel minimo riusabile customer-facing o operator-facing.

#### Target principali
- distinzione tra set minimo già chiuso e anagrafica tecnica estesa
- campi tecnici addizionali del punto quando verificabili da fonte ammessa
- eventi e stati rilevanti per `2G`
- impatti applicativi del dato giornaliero o quartorario
- boundary tra conoscenza tecnica utile e dettaglio non ancora stabile o non retail

#### Deliverable atteso
- dominio o package dedicato `pod-pdo-2g-depth`
- glossario tecnico minimo esteso
- inventario attributi/stati/eventi con fonte

### WS4. ERP-ready handoff layer
#### Obiettivo
Tradurre i domini chiusi in pacchetti implementativi realmente riusabili da coding agent o team prodotto.

#### Deliverable atteso
- handoff per processi `switching/voltura/subentro`
- handoff morosità/CMOR
- handoff bonus/vulnerabili
- handoff reporting/compliance
- decision table separate in `DECISIONS/` quando il SSOT non chiude il comportamento applicativo

## Criteri di completamento di questo layer
Un workstream di `operational depth` si considera davvero chiuso solo quando esistono:
1. mappa del flusso end-to-end
2. attori e responsabilità esplicite
3. trigger/input/output documentati
4. SLA e tempi ricondotti alle regole SSOT
5. eccezioni principali e precedenze
6. decisioni prodotto separate dai fatti normativi
7. artefatti leggibili da team tecnico o coding agent

## Rischio se non si apre questo layer
Se ci si ferma al baseline SSOT, il repo resta forte come fonte di verità normativa minima, ma rimane debole su:
- progettazione di automazioni robuste
- orchestrazione processi ERP
- implementazione sistematica degli edge cases
- auditing applicativo dei flussi operativi reali

## Punto fermo
Questo file non declassa il lavoro già fatto.

Lo rende più onesto:
- `baseline chiuso` non vuol dire `settore completamente modellato`
- i gap residui seri esistono ancora, e sono soprattutto nel layer `flows / SII depth / PDO-2G / ERP-ready`

## Vedi anche
- [README.md](README.md)
- [INDEX.md](INDEX.md)
- [COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md](COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md)
- [MACRO/domestico-luce-boundary-vs-flussi.md](MACRO/domestico-luce-boundary-vs-flussi.md)
- [MACRO/domestico-luce-capability-map.md](MACRO/domestico-luce-capability-map.md)
- [MACRO/domestico-luce-handoff-fatturazione-ai-dev.md](MACRO/domestico-luce-handoff-fatturazione-ai-dev.md)
