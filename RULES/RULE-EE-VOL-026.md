# RULE-EE-VOL-026

## Metadata
- ID: RULE-EE-VOL-026
- Titolo: Il ritardo imputabile al distributore su connessione o attivazione con lavori genera indennizzo automatico BT domestico, salvo cause escluse
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-617-23
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/617-23allb.pdf
- Riferimento preciso: Allegato B, artt. 25-28, pp. 25-27
- Data pubblicazione: 2023-12-29
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Se il distributore non rispetta i livelli specifici di qualità per cause a lui imputabili, al cliente BT domestico spetta un indennizzo automatico di 40,25 euro, che sale a 80,50 euro entro il doppio dello standard e a 120,75 euro oltre il triplo dello standard. Non è dovuto l'indennizzo se il ritardo dipende da forza maggiore, mancato ottenimento di atti autorizzativi, cause imputabili al cliente finale o a terzi, oppure se il cliente non è in regola con i pagamenti dovuti per la prestazione richiesta. L'indennizzo va corrisposto dal distributore tramite il venditore o con rimessa diretta entro 30 giorni solari dalla prestazione o, al più tardi, dal triplo del tempo standard.

## Citazione
"40,25 € per i clienti BT domestici"; "80,50 € per i clienti BT domestici"; "120,75 € per i clienti BT domestici"; "mancato ottenimento di atti autorizzativi"; "non è tenuto a corrispondere gli indennizzi automatici"; "entro 30 giorni solari"

## Interpretazione minima
Nel boundary nuova connessione o prima attivazione con lavori il diritto all'indennizzo esiste, ma solo per ritardo imputabile all'esercente. Non va promesso in automatico quando il caso è fermo su autorizzazioni, appuntamenti saltati, opere cliente o insoluti della prestazione.

## Impatto operativo
Script customer care, tracking e QA devono separare chiaramente tre livelli: standard applicabile, causa del ritardo e fascia economica dell'indennizzo. In caso di ritardo imputabile al distributore, il cliente BT domestico va istruito a verificare l'accredito in prima fattura utile o la rimessa diretta.

## Eccezioni e limiti
La regola riguarda il cliente BT domestico. Gli importi sono diversi per clienti BT non domestici e MT. Restano ferme le esclusioni specifiche previste dal TIQC.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-021, RULE-EE-VOL-024 e con il dominio qualita-commerciale-reclami per la gestione generale degli indennizzi.

## Note
Questa regola chiude il tratto customer-facing più pratico del slice lavori o preventivi: quando il cliente ha davvero diritto a un accredito e quando invece il ritardo è regolatoriamente escluso.