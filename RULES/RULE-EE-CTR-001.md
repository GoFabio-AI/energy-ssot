# RULE-EE-CTR-001

## Metadata
- ID: RULE-EE-CTR-001
- Titolo: Nel domestico il recesso è gratuito salvo stretta eccezione per contratti a prezzo fisso e a tempo determinato, con onere proporzionato alla perdita diretta
- Dominio: contratti-offerte-trasparenza
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-NORMATTIVA-DLGS-210-2021-ART7
- URL fonte: https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2021;210~art7
- Riferimento preciso: articolo 7, commi 1, 4, 5 e 7
- Data pubblicazione: 2021-11-08
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti civili dell'energia elettrica il recesso e il cambio fornitore non possono essere gravati da oneri come regola generale. Un onere economico è ammesso solo nel caso di recesso anticipato da un contratto di fornitura a tempo determinato e a prezzo fisso, purché sia indicato in modo espresso, chiaro e agevolmente comprensibile nel documento informativo precontrattuale e nel contratto e sia specificamente approvato e sottoscritto dal cliente. La somma richiesta deve essere proporzionata e non può eccedere la perdita economica direttamente subita dal fornitore; l'onere della prova di tale perdita grava sul fornitore.

## Citazione
"non è soggetto ad alcun onere"; "in caso di recesso anticipato da un contratto di fornitura a tempo determinato e a prezzo fisso"; "specificamente approvato e sottoscritto dal cliente"; "deve in ogni caso essere proporzionata"; "non può eccedere la perdita economica direttamente subita dal fornitore"

## Interpretazione minima
Nel SSOT l'eventuale onere di recesso anticipato non va trattato come penale libera o genericamente disponibile su qualunque offerta: la regola primaria è la gratuità del recesso del cliente civile, mentre l'eccezione è circoscritta ai contratti fixed-term fixed-price e resta agganciata alla perdita economica diretta del fornitore.

## Impatto operativo
I modelli offerta e contratto devono distinguere almeno tra `recesso_senza_oneri_default` e `onere_recesso_anticipato_ammesso_solo_se_fixed_term_fixed_price`, con evidenza della base di calcolo, del massimale esposto al cliente secondo la regolazione ARERA e della documentazione probatoria della perdita economica diretta.

## Eccezioni e limiti
La regola chiude il boundary sostanziale minimo dell'onere di recesso, ma non esaurisce da sola la disciplina di disclosure documentale, che va coordinata con il CCC24, con la Scheda sintetica e con il Portale Offerte. Nel presente slice il focus è sui clienti civili domestici e non sulle piccole imprese pure anch'esse richiamate dalla norma.

## Conflitti o dipendenze
Si coordina con RULE-EE-CCC24-003, RULE-EE-CCC24-005, RULE-EE-CDCONS-001 e RULE-EE-PRC-010.

## Note
La stessa norma tutela anche il cambio fornitore come diritto da esercitare senza discriminazioni legate a costi, oneri o tempi e demanda ad ARERA misure di conformità sulle modalità di determinazione degli oneri ammessi.
