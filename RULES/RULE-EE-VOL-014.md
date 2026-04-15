# RULE-EE-VOL-014

## Metadata
- ID: RULE-EE-VOL-014
- Titolo: Nel RCU il distributore comunica entro 2 giorni lavorativi gli esiti positivi di attivazioni e disattivazioni, e le attivazioni comprendono i subentri
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-SII-EE-AOC-RCU-2025
- URL fonte: https://siiportale.acquirenteunico.it/documents/11387888/11388872/Specifiche+Tecniche_AggiornamentoOnConditionRCU_EE_v4.4.pdf/d3fd86b5-e3de-6c04-720a-0bd5337be6f7?t=1752239133288&download=true
- Riferimento preciso: §§ 5 e 5.1, pp. 17-19
- Data pubblicazione: 2025-02-10
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel processo SII di Variazione Stato POD il distributore comunica al RCU, entro 2 giorni lavorativi dall'esecuzione, gli esiti positivi di nuove connessioni, attivazioni e disattivazioni; le attivazioni comprendono anche i subentri su punto disattivo.

## Citazione
"attivazione (comprensive dei subentri, in quanto trattati dal TIQE alla stregua di una richiesta di attivazione ... di un punto disattivato)"

## Interpretazione minima
Nel modello RCU lo start supply state del subentro è gestito come attivazione e non come processo autonomo separato.

## Impatto operativo
Il SSOT può raccordare il fatto normativo ARERA sul subentro con il fatto operativo SII sulla propagazione dello stato nel registro centrale.

## Eccezioni e limiti
Fonte quasi-ufficiale di supporto operativo, non sostituisce il fondamento regolatorio primario ARERA sui diritti e SLA.

## Conflitti o dipendenze
Dipende da RULE-EE-VOL-009 e si coordina con RULE-EE-VOL-015.

## Note
La stessa fonte chiarisce anche il successivo aggiornamento dei dati RCU da parte di UDD/CC dopo la notifica di attivazione.
