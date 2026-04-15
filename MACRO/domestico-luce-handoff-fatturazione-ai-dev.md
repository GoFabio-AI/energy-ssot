# Macro, handoff AI dev, fatturazione

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Questa nota serve come pacchetto di handoff verso un agente che deve implementare codice su billing, misure, pagamenti o bolletta per il domestico luce.
- Non introduce fatti nuovi: ricompone solo file e regole SSOT già chiusi nel repo.
- Non sostituisce `DOMAINS/`, `RULES/`, `EXTRACTED/` o `CITATIONS/`.
- Se un caso non è coperto dai file indicati qui, va trattato come `gap da esplicitare` o `decisione prodotto`, non come regola implicita.

## Obiettivo pratico
Se devi far scrivere codice a un'AI sul tratto `misura -> fattura -> pagamento -> reclamo billing`, non darle tutto il repo. Passale il pacchetto minimo giusto, con il vincolo esplicito di non inventare regole.

## Pacchetto minimo da passare all'AI che sviluppa
### Contesto leggibile
- `MACRO/domestico-luce-master-2026-04-15.md`
- `MACRO/domestico-luce-billing-misure.md`

### Fonte di verità operativa
- `DOMAINS/fatturazione.md`
- `DOMAINS/misure.md`
- `DOMAINS/pagamenti-garanzie-rateizzazioni.md`

### Domini di supporto da includere se il modulo tocca rendering bolletta o pricing customer-facing
- `DOMAINS/prezzi-oneri-componenti.md`
- `DOMAINS/fiscalita.md`
- `DOMAINS/bonus-sociale.md`
- `DOMAINS/contratti-offerte-trasparenza.md`

## Regole SSOT da tradurre in codice
### Billing e bolletta
- `RULE-EE-BOL-001..006`
- `RULE-EE-BOLL-001`
- `RULE-EE-TIF-001..008`
- `RULE-EE-TIQV-004`
- `RULE-EE-TIQV-011..014`
- `RULE-EE-PRESC-001..005`
- `RULE-EE-CCC24-002..003`

### Misure e disponibilità dato
- `RULE-EE-TIME-001..004`
- `RULE-EE-POD-003`
- `RULE-EE-TIF-002..004`
- `RULE-EE-TIF-006`
- `RULE-EE-TIF-008`

### Pagamenti, garanzie e rateizzazione
- `RULE-EE-CCC24-001..002`
- `RULE-EE-PLACET-001..005`
- `RULE-EE-TIV-004..005`
- `RULE-EE-STG-004..006`
- `RULE-EE-LIB-001`
- `RULE-EE-TIQV-011`
- `RULE-EE-TIF-005`

### Se il codice genera bolletta customer-facing completa
- `RULE-EE-BONUS-005`
- `RULE-EE-FISC-ACCISA-001..003`
- `RULE-EE-FISC-IVA-001..003`

## Invarianti implementative che il repo consente già di usare
- Ordine d'uso dei dati per fatturazione: `dato effettivo -> autolettura validata -> stima`.
- Frequenza domestica elettrica: `bimestrale`.
- Termine ordinario di emissione: entro `45 giorni` dall'ultimo giorno di consumo addebitato.
- I ricalcoli di importi inizialmente stimati si innestano solo sulla successiva disponibilità di dati effettivi.
- La bolletta di chiusura va emessa entro `sei settimane` dalla cessazione.
- Se in cessazione manca ancora il dato di misura, la bolletta provvisoria restituisce comunque il deposito cauzionale eventualmente versato.
- La bolletta 2025 separa letture e consumi effettivi o stimati e i motivi del ricalcolo.
- Gli `Elementi di dettaglio` restano un layer separato dalla bolletta sintetica e vanno allegati nei reclami sugli importi fatturati.
- Se il venditore offre area personale, dopo la cessazione deve mantenerla accessibile almeno `6 mesi` per archivio bollette, archivio notifiche, reclami e richieste di informazioni.
- Il dies a quo della prescrizione biennale si lega al termine entro cui la fattura doveva essere emessa.
- Se una rettifica di misura viene resa disponibile nel `SII`, il venditore ha `45 giorni` per fatturare il relativo conguaglio.
- Il repo chiude come baseline uniforme del libero la rateizzazione solo per `periodicità mancata` o `importi anomali`; oltre questo perimetro non vanno inventati diritti retail generali.
- In caso di reclamo accolto su bolletta già pagata o già rateizzata, il minimo regolato su accredito o rimessa diretta è quello TIQV già richiamato nei domini.

## Cose che l'AI dev NON deve inventare
- Nessuna formula unica del mercato libero domestico valida per tutti i contratti.
- Nessun diritto uniforme ad archivio online completo oltre il minimo TIQV già chiuso.
- Nessuna rateizzazione retail generale di ogni maxiconguaglio del libero non `PLACET`.
- Nessuna clausola vendor-specific più favorevole elevata a regola SSOT generale.
- Nessuna decisione UX o prodotto spacciata per norma.

## Prompt pronto da incollare a un coding agent
Implementa il modulo `fatturazione domestico luce` usando come SSOT esclusivo i seguenti file del repo:
- `knowledge/energia-ssot/DOMAINS/fatturazione.md`
- `knowledge/energia-ssot/DOMAINS/misure.md`
- `knowledge/energia-ssot/DOMAINS/pagamenti-garanzie-rateizzazioni.md`
- se il modulo tocca rendering bolletta o calcolo customer-facing, includi anche `prezzi-oneri-componenti.md`, `fiscalita.md` e `bonus-sociale.md`
- usa inoltre le `RULE-*` richiamate nei file come vincoli implementativi atomici

Vincoli:
- non inventare regole non presenti nel repo
- tratta i casi non coperti come gap espliciti o decisioni prodotto separate
- non promuovere clausole vendor-specific a baseline generale
- separa chiaramente `regola SSOT`, `assunzione tecnica`, `decisione prodotto`
- se una scelta implementativa non è chiusa dal SSOT, restituisci una lista di decisioni aperte invece di dedurla

Output atteso:
- domain model del billing
- invarianti applicative derivate dalle `RULE-*`
- casi di test minimi per emissione, stima, ricalcolo, chiusura, prescrizione, accredito e rateizzazione regolata
- elenco dei punti che richiedono `DECISIONS/` invece di codice hardcoded

## Dove approfondire nel repo
- [../DOMAINS/fatturazione.md](../DOMAINS/fatturazione.md)
- [../DOMAINS/misure.md](../DOMAINS/misure.md)
- [../DOMAINS/pagamenti-garanzie-rateizzazioni.md](../DOMAINS/pagamenti-garanzie-rateizzazioni.md)
- [../DOMAINS/prezzi-oneri-componenti.md](../DOMAINS/prezzi-oneri-componenti.md)
- [../DOMAINS/fiscalita.md](../DOMAINS/fiscalita.md)
- [../DOMAINS/bonus-sociale.md](../DOMAINS/bonus-sociale.md)
- [domestico-luce-billing-misure.md](domestico-luce-billing-misure.md)
- [domestico-luce-master-2026-04-15.md](domestico-luce-master-2026-04-15.md)
- [../DECISIONS/DECISION-TEMPLATE.md](../DECISIONS/DECISION-TEMPLATE.md)
