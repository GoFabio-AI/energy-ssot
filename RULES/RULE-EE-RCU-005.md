# RULE-EE-RCU-005

## Metadata
- ID: RULE-EE-RCU-005
- Titolo: Dopo la notifica di attivazione l'UDD deve integrare i dati RCU entro 3 giorni e, se il flusso VS2 manca, interviene la controparte commerciale via AE1.0050
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
Dopo la notifica di attivazione del POD, ciascun UDD deve aggiornare entro 3 giorni i dati RCU di propria competenza tramite VS2.0201; in assenza di abbinamento POD-venditore l'UDD trasmette come CC sul punto fino al successivo abbinamento, e se i dati non vengono inviati tramite VS2 la CC abbinata deve trasmetterli tramite AE1.0050.

## Citazione
"Entro 3 giorni dalla notifica di attivazione del POD, ciascun UDD è tenuto ad aggiornare i dati costituenti il RCU di propria competenza"

## Interpretazione minima
L'attivazione nel RCU non è completa con il solo cambio di stato: dopo la notifica di VS2.0200 esiste un obbligo ulteriore di integrazione dei dati di competenza UDD/CC, con fallback esplicito sulla controparte commerciale abbinata.

## Impatto operativo
Nel SSOT un subentro o una nuova attivazione deve prevedere una seconda fase di completamento anagrafico-contrattuale del RCU, separata dal semplice esito tecnico di attivazione.

## Eccezioni e limiti
Fonte quasi-ufficiale di supporto operativo. Il documento non sostituisce la fonte primaria ARERA sulla disciplina dei diritti del cliente finale.

## Conflitti o dipendenze
Dipende da RULE-EE-RCU-004 e si coordina con RULE-EE-VOL-014 e RULE-EE-VOL-017.

## Note
La stessa pagina mostra anche il caso di assenza di abbinamento POD-venditore e il fallback AE1.0050 della CC abbinata.
