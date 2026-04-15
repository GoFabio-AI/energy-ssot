# Macro docs, luce domestica

Snapshot: 2026-04-15

Questa cartella raccoglie documenti brevi e leggibili costruiti solo a partire dal materiale SSOT già presente nel repo.

## Regola d'uso
- queste note non sostituiscono `DOMAINS/`, `RULES/`, `EXTRACTED/` o `CITATIONS/`
- servono per lettura umana rapida e packaging tematico
- se serve il dettaglio normativo o la formulazione esatta, la fonte di verità resta nei file dominio e nelle regole collegate

## Pacchetto attuale
- [domestico-luce-master-2026-04-15.md](domestico-luce-master-2026-04-15.md)
- [domestico-luce-capability-map.md](domestico-luce-capability-map.md)
- [domestico-luce-handoff-fatturazione-ai-dev.md](domestico-luce-handoff-fatturazione-ai-dev.md)
- [domestico-luce-prezzi.md](domestico-luce-prezzi.md)
- [domestico-luce-fiscalita.md](domestico-luce-fiscalita.md)
- [domestico-luce-bonus-vulnerabili.md](domestico-luce-bonus-vulnerabili.md)
- [domestico-luce-segmentazione-regimi.md](domestico-luce-segmentazione-regimi.md)
- [domestico-luce-switching-voltura.md](domestico-luce-switching-voltura.md)
- [domestico-luce-pod-accessi-reporting.md](domestico-luce-pod-accessi-reporting.md)
- [domestico-luce-reporting-regolatorio.md](domestico-luce-reporting-regolatorio.md)
- [domestico-luce-billing-misure.md](domestico-luce-billing-misure.md)
- [domestico-luce-morosita-pagamenti.md](domestico-luce-morosita-pagamenti.md)

## Mappa rapida del pacchetto

| Macro doc | Slice SSOT di partenza | Cosa si può leggere con fiducia | Gap principale lasciato fuori |
| --- | --- | --- | --- |
| [domestico-luce-master-2026-04-15.md](domestico-luce-master-2026-04-15.md) | sintesi trasversale del baseline già chiuso su prezzi, fiscalità, bonus/vulnerabili, contratti/trasparenza, switching/voltura/subentro/cessazione/prima attivazione, billing/misure, morosità/pagamenti, dati/accessi/reporting | un unico documento leggibile di settore con baseline domestico finale al `2026-04-15` e sezione finale sui soli follow-up di monitoraggio o manutenzione | nessun gap SSOT attivo sul baseline; restano solo monitoraggio ufficiale ed editorial extension fuori scope |
| [domestico-luce-capability-map.md](domestico-luce-capability-map.md) | roadmap SSOT domestico luce + domini `attori-mercato`, `tutele-graduali`, `contratti-offerte-trasparenza`, `prezzi-oneri-componenti`, `fiscalita`, `fatturazione`, `pagamenti-garanzie-rateizzazioni`, `morosita-cmor`, `switching`, `voltura-subentro-cessazione`, `misure`, `anagrafica-tecnica-pod-accessi-reporting`, `qualita-commerciale-reclami`, `reporting-regolatorio` | capability map per uso prodotto, con split esplicito tra baseline normativa e layer interpretativo `sapere/fare/decidere`, utile come ponte verso `SUPER` senza introdurre decisioni di prodotto | nessun gap SSOT attivo; restano solo limiti strutturali già chiusi nel boundary e l'assenza di decisioni prodotto registrate |
| [domestico-luce-handoff-fatturazione-ai-dev.md](domestico-luce-handoff-fatturazione-ai-dev.md) | `fatturazione`, `misure`, `pagamenti-garanzie-rateizzazioni`, con richiami a `prezzi-oneri-componenti`, `fiscalita`, `bonus-sociale`, `contratti-offerte-trasparenza` e relative `RULE-*` | pacchetto pronto da passare a un coding agent per implementare billing domestico senza inventare regole, con prompt incollabile, invarianti SSOT e boundary su ciò che deve restare `gap` o `decisione prodotto` | non sostituisce le decisioni applicative: se il prodotto richiede scelte non chiuse dal SSOT, vanno registrate in `DECISIONS/` |
| [domestico-luce-prezzi.md](domestico-luce-prezzi.md) | `prezzi-oneri-componenti`, `contratti-offerte-trasparenza`, `RULE-EE-PRC-*`, `RULE-EE-DISP-*`, `RULE-EE-TIV-002..003`, `RULE-EE-STG-002..003`, `RULE-EE-CTR-001..005` | bucket bolletta 2025, componenti regolatorie MT/STG, rete/oneri/dispacciamento lato servizi regolati e boundary strutturale del libero domestico, incluse offerte onnicomprensive, offerte non generalizzate come fuori-Portal ma non fuori-disclosure, promozioni automatiche vs detail-only, eccezione oraria, comparabilità Portale art. 10.8 e boundary completo dell'onere di recesso anticipato anche lato Portale | restano soprattutto futuri aggiornamenti regolatori e casi commerciali extra-corpus non ancora normati |
| [domestico-luce-fiscalita.md](domestico-luce-fiscalita.md) | `DOMAINS/fiscalita.md`, `RULE-EE-FISC-ACCISA-*`, `RULE-EE-FISC-IVA-*` | accisa abitazioni, agevolazione residente, IVA uso domestico e principali esclusioni | restano solo futuri aggiornamenti ADM o fiscali, non gap strutturali del package |
| [domestico-luce-bonus-vulnerabili.md](domestico-luce-bonus-vulnerabili.md) | `bonus-sociale`, `tutele-graduali`, `RULE-EE-BONUS-*`, `RULE-EE-VUL-*` | requisiti bonus economico, importi ordinari 2026, esposizione minima in bolletta, categorie vulnerabili e rapporto con MT/STG | solo manutenzione editoriale di eventuali futuri consolidati ARERA |
| [domestico-luce-segmentazione-regimi.md](domestico-luce-segmentazione-regimi.md) | `attori-mercato`, `tutele-graduali`, `bonus-sociale`, `domestico-luce-bonus-vulnerabili` | vista editoriale unica di segmentazione cliente domestico, routing minimo tra vulnerabili, non vulnerabili, MT, STG e mercato libero, più raccordo bonus/vulnerabilità | restano solo rifiniture glossario sui ruoli di mercato e futuri consolidati ARERA |
| [domestico-luce-switching-voltura.md](domestico-luce-switching-voltura.md) | `switching`, `voltura-subentro-cessazione`, `RULE-EE-SWI-*`, `RULE-EE-VOL-*` | distinzione switching/voltura, titolo immobile, tempi voltura, subentro, cessazione/disattivazione, boundary chiuso della prima attivazione con lavori/preventivi, costi TIC vigenti e edge case su rifiuto e morosità pregressa | solo eventuali estensioni future A→Z su connessioni temporanee, MT o infrastrutturali e raccordo finale con la riforma switching 24h |
| [domestico-luce-pod-accessi-reporting.md](domestico-luce-pod-accessi-reporting.md) | `anagrafica-tecnica-pod-accessi-reporting`, `RULE-EE-POD-*`, `RULE-EE-RCU-*`, `RULE-EE-TIF-003`, `RULE-EE-TIME-003` | set minimo customer-facing e operator-facing del POD, accesso cliente e terze parti ai dati, limiti privacy minimi Portale/SII, boundary documentale tra Portale, TIQV e supporto durevole, e reporting dati misura direttamente collegato al punto | restano solo eventuali futuri atti ARERA/AU/SII che amplino davvero il perimetro, non gap SSOT attivi sul baseline |
| [domestico-luce-reporting-regolatorio.md](domestico-luce-reporting-regolatorio.md) | `reporting-regolatorio`, `qualita-commerciale-reclami`, `anagrafica-tecnica-pod-accessi-reporting`, `RULE-EE-TIQV-007..029`, `RULE-EE-TIME-003`, `RULE-EE-TIF-003`, `RULE-EE-BOLL-001` | package leggibile end-to-end su intake, classificazione TIQV, registri, call center, comunicazioni ad ARERA, pubblicazioni annuali e reporting del dato di misura verso SII e bolletta | nessun gap strutturale residuo nel package al `2026-04-15`, salvo futuri aggiornamenti normativi materiali |
| [domestico-luce-billing-misure.md](domestico-luce-billing-misure.md) | `fatturazione`, `misure`, `RULE-EE-TIF-*`, `RULE-EE-TIME-*`, `RULE-EE-PRESC-*` | ordine d'uso dei dati, tempi di emissione, bolletta di chiusura, ricostruzioni, prescrizione, Portale Consumi e accesso minimo di terze parti/privacy | solo clausole commerciali extra-standard fuori dal boundary SSOT uniforme |
| [domestico-luce-morosita-pagamenti.md](domestico-luce-morosita-pagamenti.md) | `morosita-cmor`, `pagamenti-garanzie-rateizzazioni`, `RULE-EE-TIMOE-*`, `RULE-EE-TISIND-*`, `RULE-EE-PLACET-*`, `RULE-EE-TIV-004..007`, `RULE-EE-STG-004..006` | baseline su pagamenti, deposito, rateizzazione regolata, mora, sospensione, interruzione fisica, ultima istanza e CMOR | solo clausole contrattuali extra-standard del libero e costing non standardizzato ex articolo 9 |
