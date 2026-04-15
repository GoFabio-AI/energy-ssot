# RULE-EE-RCU-004

## Metadata
- ID: RULE-EE-RCU-004
- Titolo: Dopo l'ammissibilità del flusso VS1 il SII aggiorna il RCU entro 1 giorno lavorativo e notifica la nuova attivazione alla controparte commerciale
- Dominio: anagrafica-tecnica-pod-accessi-reporting
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-SII-EE-AOC-RCU-2025
- URL fonte: https://siiportale.acquirenteunico.it/documents/11387888/11388872/Specifiche+Tecniche_AggiornamentoOnConditionRCU_EE_v4.4.pdf/d3fd86b5-e3de-6c04-720a-0bd5337be6f7?t=1752239133288&download=true
- Riferimento preciso: § 5.1, p. 19
- Data pubblicazione: 2025-02-10
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel processo VS, verificata l'ammissibilità del flusso del distributore, il Gestore del SII aggiorna il RCU entro 1 giorno lavorativo e notifica la nuova attivazione alla controparte commerciale tramite VS2.0200.

## Citazione
"entro 1 giorno lavorativo, aggiorna il RCU e notifica alla controparte commerciale la nuova attivazione"

## Interpretazione minima
Tra esecuzione tecnica della prestazione e popolamento centrale del registro esiste un passaggio intermedio esplicito di ammissibilità del flusso VS1, seguito da aggiornamento SII e notifica di attivazione.

## Impatto operativo
Nel SSOT il cambio di stato del punto non va modellato come immediato e indistinto: il distributore esegue e comunica, il SII verifica e poi aggiorna il RCU notificando la controparte commerciale.

## Eccezioni e limiti
Fonte quasi-ufficiale di supporto operativo. Non sostituisce i diritti o SLA customer-facing di fonte ARERA primaria.

## Conflitti o dipendenze
Dipende da RULE-EE-VOL-014 e si coordina con RULE-EE-RCU-003 e RULE-EE-RCU-005.

## Note
Regola utile per state machine, ERP e audit del popolamento RCU dopo attivazione o subentro.
