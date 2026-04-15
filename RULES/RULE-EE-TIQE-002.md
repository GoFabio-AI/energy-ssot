# RULE-EE-TIQE-002

## Metadata
- ID: RULE-EE-TIQE-002
- Titolo: Se la riattivazione per morosità supera lo standard, al cliente BT domestico spetta un rimborso automatico di 35, 70 o 105 euro
- Dominio: morosita-cmor
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIQE-646-15-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/15/646-15all.pdf
- Riferimento preciso: tabella 15, voce "Tempo massimo di riattivazione della fornitura in seguito a sospensione per morosità di cui all'articolo 90"
- Data pubblicazione: 2015-12-22
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti BT domestici, se la riattivazione della fornitura in seguito a sospensione per morosità viene eseguita oltre lo standard di 1 giorno feriale, spetta un rimborso automatico di 35 euro se la prestazione è eseguita entro il doppio del tempo standard, di 70 euro se è eseguita entro il triplo del tempo standard e di 105 euro se è eseguita oltre il triplo del tempo standard.

## Citazione
"Tempo massimo di riattivazione della fornitura in seguito a sospensione per morosità di cui all’articolo 90"; "1 giorno feriale"; "35,00"; "70,00"; "105,00"

## Interpretazione minima
Il tempo di riattivazione post-morosità non è presidiato solo da uno SLA tecnico, ma anche da un rimborso automatico crescente a favore del cliente domestico BT.

## Impatto operativo
I flussi con il distributore e la fatturazione devono monitorare il superamento dello standard e assicurare l'accredito automatico del rimborso dovuto al cliente senza necessità di ulteriore reclamo.

## Eccezioni e limiti
La regola qui atomizzata riguarda i clienti BT domestici e il rimborso collegato al ritardo della prestazione di riattivazione, non gli indennizzi TIMOE per vizi della procedura di mora imputabili al venditore.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIQE-001 per lo standard temporale della riattivazione e con RULE-EE-TIMOE-003 per gli indennizzi e i divieti di addebito che scattano invece quando la procedura di mora è stata violata dal venditore.

## Note
Nel linguaggio customer-facing ARERA la stessa scala è resa come 35, 70 e 105 euro.