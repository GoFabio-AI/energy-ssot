# RULE-EE-BOLL-001

## Metadata
- ID: RULE-EE-BOLL-001
- Titolo: La bolletta deve distinguere letture, consumi e ricalcoli con motivazione e importo
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: Allegato A, commi 8.3, 8.4, 8.5, 8.6 e 8.10
- Data pubblicazione: 2024-07-23
- Data ultima verifica: 2026-04-15

## Testo normalizzato
La bolletta elettrica deve esporre separatamente letture rilevate, autoletture, letture ricondotte e letture stimate, nonché consumi effettivi, consumi stimati e consumi fatturati. Se la fatturazione include dati stimati, la bolletta deve avvisare che gli importi possono essere oggetto di successivo ricalcolo. Quando avviene un ricalcolo, la bolletta deve indicarne periodo, motivo e importo da addebitare o accreditare; nei casi previsti deve anche riportare lettura iniziale, lettura finale e importi già contabilizzati in detrazione.

## Citazione
"il dettaglio delle letture con l’indicazione separata tra letture rilevate, autoletture, letture ricondotte e letture stimate"; "nel caso di letture e consumi stimati, che gli importi fatturati potranno essere oggetto di successivo ricalcolo"; "ricalcolo per lettura precedentemente errata"; "ricalcolo per ricostruzione dei consumi"

## Interpretazione minima
La regola riguarda la trasparenza customer-facing della bolletta, non la formazione primaria del dato di misura, che resta disciplinata da TIF e TIME.

## Impatto operativo
Template bolletta, parser e controlli di compliance devono distinguere chiaramente effettivo, stimato e ricalcolato e conservare il motivo del ricalcolo.

## Eccezioni e limiti
La disciplina include anche casi non strettamente domestici, come l’energia reattiva per potenze superiori a 16,5 kW; nel perimetro domestico qui si utilizzano solo le parti su letture, consumi e ricalcoli.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIF-002, RULE-EE-TIF-004, RULE-EE-TIME-003 e RULE-EE-TIME-004.

## Note
Il consumo annuo aggiornato deve derivare da letture/autoletture/letture ricondotte, oppure dalla miglior stima del venditore se tali dati non sono disponibili.