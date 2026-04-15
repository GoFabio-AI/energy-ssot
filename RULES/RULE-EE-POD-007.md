# RULE-EE-POD-007

## Metadata
- ID: RULE-EE-POD-007
- Titolo: La bolletta elettrica deve riportare i dati minimi identificativi e tecnici del punto di fornitura
- Dominio: anagrafica-tecnica-pod-accessi-reporting
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: Allegato A, commi 6.2 e 8.2
- Data pubblicazione: 2024-07-23
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nella bolletta elettrica il venditore deve riportare almeno i dati identificativi del punto, cioè indirizzo del punto, codice POD e potenza impegnata. Negli Elementi informativi essenziali deve inoltre riportare, per il settore elettrico, la tipologia di cliente e la tensione nominale di alimentazione.

## Citazione
"i dati identificativi del punto di prelievo"; "l’indirizzo cui corrisponde il punto"; "il codice POD"; "la potenza impegnata"; "la tipologia di cliente"; "la tensione nominale di alimentazione"

## Interpretazione minima
Questa è la minima anagrafica tecnica customer-facing del POD che emerge in modo esplicito dalla disciplina ARERA della bolletta sintetica.

## Impatto operativo
Template bolletta, parser documentali e data model customer-facing devono prevedere almeno questi campi come obbligatori nel domestico elettrico.

## Eccezioni e limiti
La regola non pretende di esaurire tutti i dati tecnici potenzialmente disponibili al cliente tramite altri canali come Portale Consumi o contatti con il venditore.

## Conflitti o dipendenze
Si coordina con RULE-EE-POD-003 per l’accesso self-service del cliente ai dati e con RULE-EE-POD-005 per la diversa vista tecnica disponibile agli operatori.

## Note
La fonte distingue chiaramente tra dati identificativi del punto e caratteristiche tecniche della fornitura, entrambe rilevanti per il minimo set customer-facing.
