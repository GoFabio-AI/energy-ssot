# RULE-EE-VOL-009

## Metadata
- ID: RULE-EE-VOL-009
- Titolo: Il subentro è un’attivazione con variazione dei soli dati identificativi su un punto di prelievo disattivo
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-617-23
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/617-23allb.pdf
- Riferimento preciso: Allegato B, art. 2 definizioni, lettera qq), p. 9
- Data pubblicazione: 2023-12-29
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel settore elettrico il subentro consiste nella richiesta di attivazione della fornitura, con contestuale variazione dei soli dati identificativi, riferita a un punto di prelievo disattivo.

## Citazione
"“subentro” è la richiesta di attivazione, con contestuale variazione dei soli dati identificativi, di un punto di prelievo disattivo"

## Interpretazione minima
Il subentro non è una voltura su punto attivo e non è un mero cambio fornitore; presuppone invece che il POD sia disattivo e che l'operazione rilevante sia un'attivazione.

## Impatto operativo
Nel SSOT il subentro va classificato come start supply state su punto disattivo, non come successione senza soluzione di continuità.

## Eccezioni e limiti
La regola definisce il perimetro minimo del subentro ma non esaurisce da sola i flussi SII e i tempi operativi.

## Conflitti o dipendenze
Da distinguere da RULE-EE-VOL-001 e RULE-EE-VOL-002 sulla voltura.

## Note
Regola primaria e atomica, utile come discriminante iniziale del caso d'uso.
