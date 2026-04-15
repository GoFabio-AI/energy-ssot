# RULE-EE-BONUS-002

## Metadata
- ID: RULE-EE-BONUS-002
- Titolo: Il bonus sociale elettrico per disagio economico richiede soglia ISEE valida e fornitura elettrica domestica intestata a un componente del nucleo
- Dominio: bonus-sociale
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BONUS-REQUISITI
- URL fonte: https://www.arera.it/consumatori/bonus-sociale/bonus-sociale-per-disagio-economico/quali-sono-i-requisiti
- Riferimento preciso: pagina ARERA requisiti del bonus sociale per disagio economico
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il bonus sociale elettrico per disagio economico spetta se il nucleo familiare ha ISEE non superiore a 9.796 euro per famiglie con massimo 3 figli a carico oppure non superiore a 20.000 euro per famiglie con almeno 4 figli a carico, e la fornitura elettrica diretta è intestata a un componente del nucleo ISEE, è per uso domestico ed è attiva o sospesa per morosità.

## Citazione
"non è superiore a 9.796 euro"; "non è superiore a 20.000 euro"; "la fornitura ... è intestata a uno dei componenti il nucleo ISEE"; "Sono considerate attive anche le forniture momentaneamente sospese per morosità del cliente"

## Interpretazione minima
L'eleggibilità economica da sola non basta: la fornitura deve anche essere tecnicamente e anagraficamente ammissibile.

## Impatto operativo
Validazioni interne e dataset SSOT devono prevedere almeno soglia ISEE, numerosità familiare, intestazione del contratto, uso domestico e stato della fornitura.

## Eccezioni e limiti
Se il contratto è intestato a un soggetto esterno al nucleo ISEE, il bonus non viene riconosciuto sulla fornitura diretta.

## Conflitti o dipendenze
Dipende dal flusso di verifica svolto dal SII.

## Note
La relazione tra bonus economico e vulnerabilità è rilevante anche per il perimetro clienti vulnerabili.

