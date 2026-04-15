# RULE-EE-POD-006

## Metadata
- ID: RULE-EE-POD-006
- Titolo: L’aggiornamento del RCU deve passare per processi SII dedicati al tipo di evento
- Dominio: anagrafica-tecnica-pod-accessi-reporting
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-SII-EE-POPOLAMENTO-RCU-PAGE
- URL fonte: https://siiportale.acquirenteunico.it/processi/settore-elettrico/popolamento-e-aggiornamento-rcu
- Riferimento preciso: elenco dei processi principali della pagina processo
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel portale SII l’aggiornamento del RCU avviene tramite processi dedicati, tra cui VS, AE, SM/RT, DS, AV, VP, TDE e CP, distinti in funzione della natura dell’evento o del dato aggiornato.

## Citazione
"I processi principali tramite i quali viene aggiornato il RCU sono"; "VS - Variazione Stato"; "TDE - Trasmissione Dati Elettrici"; "CP - Check Pod"

## Interpretazione minima
Anagrafiche, stati del punto, vulnerabilità, potenze e dati elettrici non confluiscono nel RCU con un aggiornamento indistinto.

## Impatto operativo
Nel SSOT ogni modifica del punto o del suo assetto informativo deve essere ricondotta, quando possibile, al processo SII di riferimento e non a un generico update POD.

## Eccezioni e limiti
La pagina processo non fornisce il dettaglio dei singoli tracciati o delle regole di validazione dei processi elencati.

## Conflitti o dipendenze
Si coordina con RULE-EE-RCU-003 e con RULE-EE-POD-004 per le integrazioni anagrafiche via PK2.

## Note
La distinzione dei processi è rilevante anche per stabilire quale attore di filiera sia responsabile del dato.
