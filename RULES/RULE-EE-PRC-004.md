# RULE-EE-PRC-004

## Metadata
- ID: RULE-EE-PRC-004
- Titolo: Gli oneri generali di sistema customer-facing includono ARIM e ASOS e seguono una struttura domestica specifica
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-ONERI-SISTEMA-PAGE
- URL fonte: https://www.arera.it/area-operatori/prezzi-e-tariffe/oneri-generali-di-sistema-e-ulteriori-componenti
- Riferimento preciso: sezione elettricità, descrizione ASOS/ARIM e applicazione domestica
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel domestico elettrico, gli oneri generali di sistema si articolano nelle componenti `ASOS` e `ARIM`; per i clienti domestici non si applica la quota potenza e, per i clienti domestici in residenza anagrafica, non si applica nemmeno la quota fissa.

## Citazione
"ASOS"; "ARIM"; "Agli utenti domestici non è applicata la quota potenza"; "Agli utenti domestici in residenza anagrafica non è applicata nemmeno la quota fissa"

## Interpretazione minima
La bucket customer-facing oneri è chiusa a `ASOS` e `ARIM`, ma la struttura interna resta differenziata per tipologia domestica e residenza.

## Impatto operativo
Nel SSOT oneri e rete devono restare distinti; nei modelli domestici non va introdotta una quota potenza per gli oneri generali di sistema.

## Eccezioni e limiti
La regola non dettaglia tutti gli elementi interni di `ASOS` e `ARIM` né la fiscalità connessa.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRC-001 e con la Tabella 1 della Bolletta 2025 che chiude il bucket oneri in `ARIM` e `ASOS`.

## Note
`UC3` e `UC6` non appartengono a questo bucket, ma ai servizi di rete.
