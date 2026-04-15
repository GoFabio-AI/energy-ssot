# RULE-EE-VOL-019

## Metadata
- ID: RULE-EE-VOL-019
- Titolo: Solo allacciamento senza attivazione si chiede al distributore, allacciamento con attivazione si chiede al venditore
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-ATLANTE-ALLACCIAMENTO-RICHIESTA
- URL fonte: https://www.arera.it/atlante-per-il-consumatore/elettricita/la-fornitura/allacciamento/come-si-richiede-lallacciamento
- Riferimento preciso: testo principale pagina "Come si richiede l'allacciamento?"
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Se il cliente vuole ottenere solo l'allacciamento alla rete elettrica senza attivare subito la fornitura, la richiesta va presentata direttamente al distributore locale. Se invece chiede contestualmente allacciamento e attivazione della fornitura, deve rivolgersi al venditore scelto, che inoltra la richiesta al distributore entro 2 giorni lavorativi.

## Citazione
"Se si desidera ottenere l'allacciamento alla rete elettrica, ma non si ha interesse ad attivare fin da subito la fornitura, bisogna rivolgersi direttamente all'impresa distributrice locale"; "l'impresa di vendita inoltrerà la richiesta al distributore locale entro due giorni lavorativi"

## Interpretazione minima
Il contenitore generico "prima attivazione" va sempre spezzato almeno tra puro allacciamento e allacciamento con contestuale start supply.

## Impatto operativo
Nei flussi CRM, nei moduli di intake e negli script di customer care va chiesto subito se il cliente vuole solo predisporre il punto o anche attivare immediatamente la fornitura, perché cambia il soggetto a cui indirizzare la richiesta.

## Eccezioni e limiti
La fonte è un supporto ufficiale consumer-facing ARERA. I fondamenti primari su richiesta di connessione, dati minimi della domanda e qualità commerciale restano nel TIC e nel TIQC.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-020, RULE-EE-VOL-021 e RULE-EE-VOL-024.

## Note
Regola chiave per chiudere il boundary minimo della nuova connessione senza trasformare automaticamente ogni caso in subentro o attivazione standard.
