# RULE-EE-PRC-007

## Metadata
- ID: RULE-EE-PRC-007
- Titolo: Dal 2026-04-01 il mercato libero domestico elettrico ha una struttura standardizzata dei corrispettivi, ma non una formula numerica unica uguale per tutti i venditori
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-386-2025-R-COM-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/25/386-2025-R-com.pdf
- Riferimento preciso: Articolo 1, commi 1.2, 1.3 e 1.6; Articolo 6, comma 6.1
- Data pubblicazione: 2025-08-05
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per le offerte di energia elettrica del mercato libero rivolte ai clienti finali domestici, dal 2026-04-01 la disciplina ARERA non impone una formula numerica unica valida per tutti i venditori, ma una struttura standardizzata dei corrispettivi. Nelle offerte non onnicomprensive il cliente deve avere: un corrispettivo annuo unico in €/POD/anno definito dal venditore, un corrispettivo consumo unico in €/kWh definito dal venditore, un corrispettivo separato per dispacciamento e mercato della capacità, più i corrispettivi rete e gli oneri generali di sistema. Nelle offerte con corrispettivi onnicomprensivi il cliente ha invece un corrispettivo annuo unico e un corrispettivo consumo unico che includono tutte le voci di spesa.

## Citazione
"un unico corrispettivo in quota annua, espresso in €/POD/anno"; "un unico corrispettivo dipendente dal consumo, espresso in €/kWh"; "un corrispettivo a copertura dei costi del servizio di dispacciamento e del mercato della capacità"; "offerta con corrispettivi onnicomprensivi"; "comprensivi di tutte le voci di spesa"

## Interpretazione minima
Il SSOT non deve inventare un’unica formula del libero domestico. Deve invece distinguere almeno due schemi regolati: offerte standard con dispacciamento separato e offerte onnicomprensive con inclusione di tutte le voci.

## Impatto operativo
I modelli dati devono separare: quota annua venditore, quota consumo venditore, dispacciamento/capacità separato o incluso, rete, oneri e imposte. La presenza del flag `onnicomprensiva` cambia il modo in cui i bucket sono ricostruibili.

## Eccezioni e limiti
La regola non fissa i valori delle componenti vendor-defined e non elimina la variabilità contrattuale tra offerte.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRC-001, RULE-EE-PRC-003, RULE-EE-DISP-003 e RULE-EE-PRC-008.

## Note
La fonte collega questa razionalizzazione all’attuazione dell’articolo 5 del decreto-legge 19/2025.