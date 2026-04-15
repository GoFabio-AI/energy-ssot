# RULE-EE-VOL-020

## Metadata
- ID: RULE-EE-VOL-020
- Titolo: Il preventivo di connessione BT deve separare l'eventuale attivazione e ricordare che la richiesta di attivazione passa dal venditore
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-617-23
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/617-23allb.pdf
- Riferimento preciso: Allegato B, art. 5.3, p. 12
- Data pubblicazione: 2023-12-29
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per le richieste di lavori sulla rete BT non incluse nella Tabella 5, il preventivo del distributore deve indicare i corrispettivi previsti per l'esecuzione del lavoro richiesto fino all'attivazione della fornitura, valorizzando separatamente l'eventuale attivazione, e deve precisare che la relativa richiesta di attivazione va presentata tramite un venditore.

## Citazione
"fino all’attivazione della fornitura, quest’ultima valorizzata separatamente, ove richiesta"; "la richiesta di attivazione deve essere presentata tramite un venditore"

## Interpretazione minima
Nel boundary nuova connessione o prima attivazione, il preventivo lavori e la successiva attivazione non vanno fusi in un unico oggetto opaco: il preventivo deve già esplicitare il raccordo con il venditore.

## Impatto operativo
Preventivi, interfacce e workflow devono tenere separati costo lavori o allacciamento e costo di attivazione, e non devono permettere di chiudere il flusso senza indicare il passaggio tramite venditore quando l'energizzazione è richiesta.

## Eccezioni e limiti
La regola riguarda i casi BT non coperti dalla Tabella 5 e non sostituisce il perimetro del preventivo rapido per i lavori semplici predeterminabili.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-019, RULE-EE-VOL-021 e RULE-EE-VOL-024.

## Note
Regola molto utile per chiudere il boundary documentale e di handoff tra distributore e venditore.
