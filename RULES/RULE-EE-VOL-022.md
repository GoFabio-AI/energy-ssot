# RULE-EE-VOL-022

## Metadata
- ID: RULE-EE-VOL-022
- Titolo: L'allacciamento permanente ordinario BT si paga con quota distanza e quota potenza, con regola speciale per la residenza fino a 3,3 kW
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-616-23
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/616-23allc.pdf
- Riferimento preciso: Allegato C, artt. 8.7, 11.1, 12.4 e 13.1, pp. 10, 12-13, tabella 1 p. 23
- Data pubblicazione: 2023-12-29
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per le connessioni permanenti ordinarie in bassa tensione si applicano contributi a forfait commisurati alla quota potenza e alla quota distanza. Per i clienti domestici nelle abitazioni di residenza anagrafica con potenza disponibile fino a 3,3 kW, oltre alla quota potenza si applica la quota fissa di cui alla Tabella 1, lettera a). Per potenze richieste fino a 30 kW con limitatore, la potenza disponibile è pari alla potenza richiesta aumentata del 10%.

## Citazione
"si applicano contributi a forfait commisurati alla potenza disponibile (quota potenza) e alla distanza convenzionale ... (quota distanza)"; "Per la connessione di clienti domestici nelle abitazioni di residenza anagrafica, con potenza disponibile fino a 3,3 kW"; "La potenza disponibile è pari alla potenza richiesta complessiva, aumentata del 10%"

## Interpretazione minima
Il costo regolato dell'allacciamento ordinario non è un importo unico fisso ma una combinazione di distanza e potenza, con una regola domestica speciale per la residenza fino a 3,3 kW.

## Impatto operativo
Simulatori, preventivi assistiti e script customer care devono chiedere almeno distanza convenzionale, uso residenza sì o no e potenza richiesta, evitando di trattare l'allacciamento ordinario come fee piatta universale.

## Eccezioni e limiti
La regola riguarda le connessioni permanenti ordinarie BT. I casi particolari a spesa relativa e le connessioni temporanee seguono discipline diverse.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-019, RULE-EE-VOL-020 e RULE-EE-VOL-023.

## Note
Include il punto utile customer-facing sulla potenza disponibile 10% più alta quando il contatore è dotato di limitatore. Per i valori correnti al 2026-04-15, usare il testo consolidato `SRC-ARERA-TIC-VIGENTE-2026-PDF`, che quantifica quota fissa 209,62 euro, quote distanza 105,08 o 209,62 o 419,24 euro per gli scaglioni oltre 200/700/1200 metri e quota potenza 78,81 euro/kW.
