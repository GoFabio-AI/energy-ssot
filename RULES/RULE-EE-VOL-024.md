# RULE-EE-VOL-024

## Metadata
- ID: RULE-EE-VOL-024
- Titolo: Lo SLA di 5 giorni per l'attivazione vale su utenza già allacciata, altrimenti si applicano i tempi dell'allacciamento
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-ATLANTE-ATTIVAZIONE-TEMPI
- URL fonte: https://www.arera.it/atlante-per-il-consumatore/elettricita/la-fornitura/attivazione/quanto-tempo-occorre-per-lattivazione
- Riferimento preciso: testo principale pagina "Quanto tempo occorre per l'attivazione?"
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Se l'utenza è già allacciata alla rete di distribuzione, il venditore trasmette la richiesta di attivazione al distributore entro 2 giorni lavorativi e il distributore deve attivare la fornitura entro 5 giorni lavorativi dal ricevimento della richiesta completa. Se l'utenza non è ancora allacciata, si applicano invece i tempi massimi previsti per la procedura di allacciamento.

## Citazione
"Se l'utenza è già allacciata alla rete di distribuzione"; "deve attivare la fornitura entro cinque giorni lavorativi"; "Se invece l'utenza non è ancora allacciata, valgono i tempi massimi previsti per la procedura di allacciamento"

## Interpretazione minima
I 5 giorni lavorativi della regola di attivazione non vanno usati per promettere tempi di nuova connessione quando il punto non è ancora fisicamente disponibile o richiede lavori di connessione.

## Impatto operativo
In prodotto e customer care bisogna chiedere sempre se il punto è già allacciato. In caso contrario, la pratica va instradata sul binario preventivo o lavori, non sul binario attivazione standard.

## Eccezioni e limiti
La pagina segnala anche il blocco per morosità del medesimo titolare; la disciplina completa di quell'edge case resta nel dominio morosità o CMOR.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-010 e RULE-EE-VOL-021.

## Note
Regola di chiusura del boundary: separa in modo operativo la vera attivazione standard dalla prima attivazione che implica prima l'allacciamento.
