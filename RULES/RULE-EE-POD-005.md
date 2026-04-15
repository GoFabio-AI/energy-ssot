# RULE-EE-POD-005

## Metadata
- ID: RULE-EE-POD-005
- Titolo: Il processo CDT mette a disposizione delle controparti commerciali i dati tecnici minimi del POD
- Dominio: anagrafica-tecnica-pod-accessi-reporting
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-SII-EE-CDT-SPEC-2020
- URL fonte: https://siiportale.acquirenteunico.it/documents/11387888/11424977/Specifiche_Tecniche_Consultazione_Dati_Tecnici_v1.0.pdf/60a3cfeb-f240-792f-7a48-4d21af16e08c?t=1752250348876&download=true
- Riferimento preciso: ambito della funzionalità CDT e descrizione del dataset consultabile
- Data pubblicazione: 2020-01-20
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Dal 19 aprile 2020 il SII mette a disposizione delle controparti commerciali, mediante Portale Web, una funzionalità di consultazione del RCU che consente interrogazioni puntuali o massive dei dati tecnici del POD. I dati tecnici minimi esposti comprendono almeno tipologia di misuratore installato, trattamento del punto ai sensi del TIS, data di messa a regime del misuratore 2G e stato di attivazione del POD.

## Citazione
"funzionalità di consultazione del RCU, mediante Portale Web"; "tipologia di misuratore installato"; "trattamento del punto ai sensi del TIS"; "data di messa a regime del misuratore 2G"; "stato di attivazione del POD"

## Interpretazione minima
Nel perimetro SSOT questa è la lista minima source-backed di anagrafica tecnica del POD accessibile agli operatori commerciali via SII.

## Impatto operativo
I modelli dati interni che rappresentano la scheda tecnica del punto devono almeno prevedere questi campi minimi e distinguere consultazione puntuale da massiva.

## Eccezioni e limiti
La specifica CDT non esaurisce tutte le informazioni di punto eventualmente presenti in altri processi SII o nei sistemi dei distributori.

## Conflitti o dipendenze
Si coordina con RULE-EE-RCU-002 per la distinzione PK/CDT e con RULE-EE-POD-007 per i dati minimi customer-facing in bolletta.

## Note
La specifica include anche la verifica dell’esistenza del POD nel RCU.
