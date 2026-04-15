# RULE-EE-BONUS-005

## Metadata
- ID: RULE-EE-BONUS-005
- Titolo: Il bonus sociale elettrico è ripartito come sconto uguale ogni mese ed è esposto in bolletta come voce separata in detrazione con indicazione della scadenza
- Dominio: bonus-sociale
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: articolo 5.2, lettera k), articolo 6.9 e facsimile di bolletta; coordinamento operativo con la pagina ARERA `SRC-ARERA-BONUS-AMMONTANO`
- Data pubblicazione: 2025-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nella bolletta elettrica il bonus sociale, per i clienti che ne hanno titolo, è esposto come voce separata `bonus sociale` in detrazione dopo le voci `quota fissa` o `quota potenza` e `quota per consumi`; la bolletta riporta inoltre la data di scadenza del bonus sociale per disagio economico. In coordinamento con la pagina ARERA sugli importi, lo sconto è applicato in misura uguale ogni mese e in una bolletta bimestrale compare quindi la somma di due mensilità di bonus.

## Citazione
"a) “bonus sociale” in detrazione, per i clienti che ne hanno titolo;"; "la data di scadenza del bonus sociale per disagio economico"; "Bonus sociale (2 mesi) - 30,00 €"; "Il cliente trova quindi in ogni bolletta lo stesso sconto"

## Interpretazione minima
Le fonti ufficiali consultate non collocano il bonus dentro i bucket di spesa per vendita o rete/oneri, ma come detrazione separata visibile in bolletta. La ripartizione minima accertata è mensile costante, con evidenza aggregata in fattura in base al periodo fatturato.

## Impatto operativo
Template di bolletta, motori di calcolo e UX cliente devono mostrare il bonus come riga dedicata in detrazione, non come sconto nascosto dentro le altre bucket di spesa, e devono rendere disponibile la data di scadenza del bonus economico.

## Eccezioni e limiti
La fonte ARERA di struttura bolletta mostra la collocazione customer-facing e un facsimile bimestrale. La formula di dettaglio per qualunque prorata residua oltre i valori giornalieri e per 30 giorni pubblicati da ARERA non è ulteriormente esplicitata nelle fonti qui consolidate.

## Conflitti o dipendenze
Si coordina con `RULE-EE-BONUS-004` per gli importi 2026 e con `RULE-EE-BONUS-003` per il momento di prima applicazione nella prima fattura utile.

## Note
Il facsimile ARERA mostra un cliente domestico residente con potenza impegnata 3 kW e la riga `Bonus sociale (2 mesi) - 30,00 €`, coerente con una ripartizione mensile costante.
