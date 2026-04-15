# Energia SSOT, index operativo

Snapshot strutturale: 2026-04-15

## Navigazione rapida
- [README.md](README.md)
- [ROADMAP-DOMESTICO-LUCE-2026-04-15.md](ROADMAP-DOMESTICO-LUCE-2026-04-15.md)
- [COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md](COMPLETION-PACKAGE-DOMESTICO-LUCE-2026-04-15.md)
- [OPEN-QUESTIONS.md](OPEN-QUESTIONS.md)
- [GLOSSARIO.md](GLOSSARIO.md)
- [SOURCE-REGISTRY.md](SOURCE-REGISTRY.md)
- [WORKFLOW.md](WORKFLOW.md)

## Macro docs leggibili, domestico luce
- [MACRO/README.md](MACRO/README.md)
- [MACRO/domestico-luce-master-2026-04-15.md](MACRO/domestico-luce-master-2026-04-15.md)
- [MACRO/domestico-luce-capability-map.md](MACRO/domestico-luce-capability-map.md)
- [MACRO/domestico-luce-handoff-fatturazione-ai-dev.md](MACRO/domestico-luce-handoff-fatturazione-ai-dev.md)
- [MACRO/domestico-luce-prezzi.md](MACRO/domestico-luce-prezzi.md)
- [MACRO/domestico-luce-fiscalita.md](MACRO/domestico-luce-fiscalita.md)
- [MACRO/domestico-luce-bonus-vulnerabili.md](MACRO/domestico-luce-bonus-vulnerabili.md)
- [MACRO/domestico-luce-segmentazione-regimi.md](MACRO/domestico-luce-segmentazione-regimi.md)
- [MACRO/domestico-luce-switching-voltura.md](MACRO/domestico-luce-switching-voltura.md)
- [MACRO/domestico-luce-pod-accessi-reporting.md](MACRO/domestico-luce-pod-accessi-reporting.md)
- [MACRO/domestico-luce-reporting-regolatorio.md](MACRO/domestico-luce-reporting-regolatorio.md)
- [MACRO/domestico-luce-billing-misure.md](MACRO/domestico-luce-billing-misure.md)
- [MACRO/domestico-luce-morosita-pagamenti.md](MACRO/domestico-luce-morosita-pagamenti.md)

## Stato del perimetro domestico luce

| Area | Asset SSOT attuali | Stato | Note |
| --- | --- | --- | --- |
| attori e ruoli di mercato | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md) | **chiuso al boundary SSOT** | coperti SII, RCU, UdD, vulnerabili, AU e ruoli base dei processi switching/voltura; restano solo rifiniture glossario e monitoraggio di futuri consolidati ufficiali |
| regimi di servizio, vulnerabili, STG | [DOMAINS/tutele-graduali.md](DOMAINS/tutele-graduali.md) | **chiuso al boundary SSOT** | chiusi perimetro STG e vulnerabili; baseline composita TIV/TIT/TIDE armonizzata nel repo e vista editoriale unica disponibile in [MACRO/domestico-luce-segmentazione-regimi.md](MACRO/domestico-luce-segmentazione-regimi.md) |
| switching | [DOMAINS/switching.md](DOMAINS/switching.md) | **chiuso al boundary SSOT** | chiuso il baseline vigente ARERA 487/2015 + perimetro SII; la riforma reseller a 24 ore resta solo monitoraggio futuro perché non efficace al 2026-04-15 |
| voltura, subentro, cessazione | [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md) | **chiuso al boundary SSOT** | voltura, subentro, cessazione/disattivazione e slice domestico BT di nuova connessione/prima attivazione con lavori o preventivi sono chiusi; eventuali estensioni A→Z su connessioni più ampie o particolari restano solo roadmap futura |
| anagrafica tecnica POD, accessi e reporting | [DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md](DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md) | **chiuso al boundary SSOT** | dominio chiuso al boundary SSOT: separati in modo source-backed Portale Consumi data-centric, minimo TIQV di area personale, documenti su supporto durevole e retention lato venditore; il set customer-facing ordinario del POD resta quello minimo già chiuso da bolletta, senza ulteriori campi uniformi verificati |
| misure | [DOMAINS/misure.md](DOMAINS/misure.md) | **chiuso al boundary SSOT** | chiuso il pacchetto customer-facing `TIME/TIF + Portale Consumi`; restano fuori solo sviluppi extra-slice su 2G, mentre la rateizzazione dei maxiconguagli non è più un gap normativo aperto del repo |
| fatturazione | [DOMAINS/fatturazione.md](DOMAINS/fatturazione.md) | **chiuso al boundary SSOT** | chiusi periodicità, emissione, chiusura, `Elementi di dettaglio`, reclami TIQV sugli importi fatturati, archivio bollette minimo post-cessazione, coordinamento minimo post-sentenze, disclosure contrattuale minima e rinvio retail uniforme del libero a rateizzazione per periodicità mancata o importi anomali |
| prezzi, componenti e formule economiche | [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md) | **chiuso al boundary SSOT** | coperti bucket bolletta, dispacciamento, maggior tutela, STG e boundary strutturale del libero, incluse promozioni automatiche vs detail-only e trattamento Portale dell'onere di recesso; restano soprattutto manutenzione editoriale e futuri aggiornamenti |
| fiscalità | [DOMAINS/fiscalita.md](DOMAINS/fiscalita.md) | **chiuso al boundary SSOT** | dominio autonomo su accisa abitazioni, agevolazione residente, IVA uso domestico e principali esclusioni, con boundary fiscale domestico di base già separato dal dominio prezzi |
| bonus sociale | [DOMAINS/bonus-sociale.md](DOMAINS/bonus-sociale.md) | **chiuso al boundary SSOT** | chiusi requisiti, durata, flusso INPS-SII-venditore, importi ordinari 2026, esposizione minima in bolletta e raccordo base con vulnerabilità |
| contratti, offerte e trasparenza commerciale | [DOMAINS/contratti-offerte-trasparenza.md](DOMAINS/contratti-offerte-trasparenza.md) | **chiuso al boundary SSOT** | chiuso il baseline su CCC24, PLACET, Portale, disclosure 2026, non generalizzate fuori-Portal ma non fuori-disclosure, promozioni automatiche vs detail-only e boundary completo del recesso anticipato, incluso il layer attuativo ARERA 250/2023 |
| pagamenti, garanzie e rateizzazioni | [DOMAINS/pagamenti-garanzie-rateizzazioni.md](DOMAINS/pagamenti-garanzie-rateizzazioni.md) | **chiuso al boundary SSOT** | chiuso il baseline CCC24 + PLACET + TIV/TIF, il minimo TIQV su accrediti da reclamo, il boundary post-sentenze e il rinvio uniforme del libero alla rateizzazione per periodicità mancata o importi anomali; le pattuizioni ulteriori restano contrattuali, non gap normativo SSOT |
| morosità e CMOR | [DOMAINS/morosita-cmor.md](DOMAINS/morosita-cmor.md) | **chiuso al boundary SSOT** | dominio chiuso al boundary SSOT: coordinamento TIMOE/TIV per non disalimentabili domestici non vulnerabili chiuso dal TIV 2026 (RULE-EE-TIMOE-008), costi ex articolo 9 definiti come costi effettivi senza tariffario numerico uniforme (RULE-EE-TIMOE-009) |
| qualità commerciale e reclami | [DOMAINS/qualita-commerciale-reclami.md](DOMAINS/qualita-commerciale-reclami.md) | **chiuso al boundary SSOT** | dominio chiuso al boundary SSOT: le determinazioni ARERA ex articoli 31, 33, 38 e 39 TIQV sono operative e procedurali, non estensioni materiali del baseline (RULE-EE-TIQV-029) |
| reporting regolatorio, comunicazioni e registri | [DOMAINS/reporting-regolatorio.md](DOMAINS/reporting-regolatorio.md) | **chiuso al boundary SSOT** | package dedicato che unifica il layer end-to-end su intake, registri, call center, comunicazioni ad ARERA, pubblicazioni annuali e reporting di misura già source-backed nel repo |
| glossario | [GLOSSARIO.md](GLOSSARIO.md) | parziale | normalizzato come mappa di copertura terminologica, ma ancora senza voci definitorie complete |
| decisioni prodotto SUPER | [DECISIONS/](DECISIONS/) | non avviato | nessuna decisione applicativa ancora registrata |

## Domini già presenti nel repo
- [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md)
- [DOMAINS/tutele-graduali.md](DOMAINS/tutele-graduali.md)
- [DOMAINS/switching.md](DOMAINS/switching.md)
- [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md)
- [DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md](DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md)
- [DOMAINS/misure.md](DOMAINS/misure.md)
- [DOMAINS/fatturazione.md](DOMAINS/fatturazione.md)
- [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md)
- [DOMAINS/fiscalita.md](DOMAINS/fiscalita.md)
- [DOMAINS/bonus-sociale.md](DOMAINS/bonus-sociale.md)
- [DOMAINS/contratti-offerte-trasparenza.md](DOMAINS/contratti-offerte-trasparenza.md)
- [DOMAINS/pagamenti-garanzie-rateizzazioni.md](DOMAINS/pagamenti-garanzie-rateizzazioni.md)
- [DOMAINS/morosita-cmor.md](DOMAINS/morosita-cmor.md)
- [DOMAINS/qualita-commerciale-reclami.md](DOMAINS/qualita-commerciale-reclami.md)
- [DOMAINS/reporting-regolatorio.md](DOMAINS/reporting-regolatorio.md)

## Aree A→Z ancora senza dominio autonomo completo
- nessuna sul baseline domestico luce al `2026-04-15`: il package `reporting-regolatorio` chiude anche l'ultimo gap strutturale-editoriale residuo

## Questioni aperte da seguire subito
- nessuna open question SSOT prioritaria residua sul baseline domestico luce al `2026-04-15`; restano solo monitoraggio ordinario di futuri atti, consolidati ufficiali e manutenzioni editoriali del repo

## Chiusure recenti rilevanti
- Il boundary minimo del dispacciamento nel libero domestico lato cliente è ora chiuso tramite `RULE-EE-DISP-004`, `RULE-EE-PRC-011` e `RULE-EE-PRC-012`.
- La deliberazione `ARERA 250/2023/R/com` chiude ora anche il residuo attuativo sugli oneri di recesso anticipato domestici, inclusi perimetro ammesso, massimale ex ante, ricalcolo alla perdita economica diretta, decadenza per variazione unilaterale e trattamento nel Portale Offerte.
- Il dominio `contratti-offerte-trasparenza` chiude ora anche gli edge su `sconti automatici primi 12 mesi` vs promozioni detail-only e sul fatto che pacchetti o servizi già erogati possono rilevare solo come perdita economica diretta nel ristretto perimetro del recesso anticipato.
- Il dominio `anagrafica-tecnica-pod-accessi-reporting` chiude ora anche il boundary su disponibilità online data-centric del Portale Consumi, documenti customer-facing ulteriori su supporto durevole e assenza di ulteriori campi tecnici customer-facing uniformi oltre il minimo già verificato.
- Il dominio `qualita-commerciale-reclami` chiude ora anche classificazione prudenziale TIQV, tassonomia tabella A, causalizzazione dei mancati rispetto, registri verificabili, comunicazioni annuali ad ARERA e pubblicazioni annuali lato venditore o lato ARERA; le determinazioni ARERA ex articoli 31, 33, 38 e 39 sono procedurali, non estensioni del baseline (RULE-EE-TIQV-029).
- Il dominio `morosita-cmor` chiude ora anche il coordinamento TIMOE/TIV per i non disalimentabili domestici non vulnerabili (RULE-EE-TIMOE-008) e conferma che i costi ex articolo 9 sono definiti come costi effettivi senza tariffario numerico uniforme (RULE-EE-TIMOE-009).
- Il dominio `voltura-subentro-cessazione` chiude ora anche l'intero slice domestico BT di nuova connessione o prima attivazione con lavori o preventivi tramite `RULE-EE-VOL-019..026`, fonti Atlante ARERA su allacciamento o attivazione, integrazione mirata delle fonti primarie `SRC-ARERA-617-23` e `SRC-ARERA-616-23` e quantificazione corrente dei costi tramite `SRC-ARERA-TIC-VIGENTE-2026-PDF`.
- Il dominio `fatturazione` chiude ora anche il minimo su `Elementi di dettaglio`, allegati TIQV ai reclami sugli importi fatturati e archivio bollette/notifiche per almeno 6 mesi post-cessazione se il venditore offre area personale.
- Il dominio `fatturazione` chiude ora anche il coordinamento minimo post-sentenze sul lato bolletta, con distinzione tra prescrizione maturata, cause ostative e layer upstream di compensazione.
- I domini `fatturazione` e `pagamenti-garanzie-rateizzazioni` chiudono ora anche il residuo retail uniforme del libero non-PLACET tramite `SRC-ARERA-63-2025-R-COM` e `RULE-EE-LIB-001`: la rateizzazione ARERA verificata resta limitata a periodicità mancata e importi anomali, senza ulteriori diritti uniformi su rimborsi extra-standard.

## Consistenza interna del repo
- il dominio `tutele-graduali` ora ha un file dedicato, coerente con `RULE-EE-STG-001`
- il dominio `fiscalita` ha ora un file dedicato e separa il baseline fiscale domestico da `prezzi-oneri-componenti`
- il dominio `anagrafica-tecnica-pod-accessi-reporting` è ora chiuso al boundary SSOT come dominio autonomo su punto, accessi, privacy minima e document availability di base
- il dominio `reporting-regolatorio` unifica ora in un package dedicato il layer end-to-end su comunicazioni, registri, call center, comunicazioni ad ARERA, pubblicazioni annuali e reporting di misura, senza introdurre nuove fonti o nuove regole
- il pacchetto `MACRO/` copre ora anche un master document domestico luce finale al `2026-04-15`, con sintesi trasversale del baseline chiuso e soli follow-up di manutenzione o monitoraggio futuro
- il pacchetto `MACRO/` copre ora anche una capability map domestico luce, con split esplicito tra baseline normativa e layer interpretativo per `SUPER`, senza introdurre nuove decisioni prodotto
- il pacchetto `MACRO/` copre ora anche un handoff `fatturazione -> AI dev`, pronto da passare a un coding agent con file minimi, `RULE-*` rilevanti, invarianti implementative e boundary esplicito tra SSOT e decisioni prodotto
- il pacchetto `MACRO/` copre ora anche una vista editoriale unica di segmentazione cliente e routing minimo di regime tramite `domestico-luce-segmentazione-regimi.md`
- il pacchetto `MACRO/` copre ora anche una sintesi leggibile su POD, accessi e reporting minimo, senza uscire dal boundary SSOT già chiuso
- i domini `contratti-offerte-trasparenza` e `pagamenti-garanzie-rateizzazioni` hanno ora file dedicati e chiudono due gap A→Z del repo
- la baseline composita `TIV + DL 19/2025 + ARERA 110/2025 + ARERA 96/2026 + TIT + TIDE` è ora armonizzata come riferimento trasversale sufficiente del repo al 2026-04-15
- il glossario è stato normalizzato come mappa di copertura, ma le singole voci definitorie restano da scrivere solo dopo chiusura con fonte ufficiale
- [DOMAINS/misure.md](DOMAINS/misure.md) ha ora regole atomiche dedicate del pacchetto `TIME/TIF` e raccordo esplicito con Portale Consumi
- [DOMAINS/fatturazione.md](DOMAINS/fatturazione.md) copre ora periodicità, emissione, chiusura, `Elementi di dettaglio`, reclami importi fatturati, archivio bollette minimo post-cessazione, coordinamento minimo post-sentenze e rinvio retail uniforme del libero alla rateizzazione; fuori restano solo clausole commerciali extra-standard non generalizzabili come SSOT
- [DOMAINS/morosita-cmor.md](DOMAINS/morosita-cmor.md) non è più un buco rosso: ha ora fonti primarie e regole atomiche anche sulla coda residuale di interruzione fisica, nuove attivazioni post-articolo 9, non disalimentabili e ultima istanza domestica
- [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md) non lascia più aperta una open question attiva sul slice domestico BT della prima attivazione: separa ora in modo verificato subentro, attivazione standard su punto già allacciato e nuova connessione con preventivo o lavori, inclusi computo corretto dei tempi, indennizzi ed economics TIC correnti
- `SRC-ARERA-FINE-TUTELA-ELE` ha ora `EXTRACTED/` e `CITATIONS/`, quindi la distinzione operativa ARERA tra vulnerabili e non vulnerabili è riusabile come evidenza di supporto
- `SRC-ARERA-TIV-2020-PDF` ha ora citazioni riusabili ricavate dal `full-extract`, restando materiale storico di confronto e non baseline vigente
