# RULE-EE-BOL-005

## Metadata
- ID: RULE-EE-BOL-005
- Titolo: Lo Scontrino dell’energia espone gli importi nella logica quantità, prezzo medio e importo
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: Allegato A, articolo 6, commi 6.3 e 6.4
- Data pubblicazione: 2024-07-23
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Lo `Scontrino dell’energia` riporta la formazione dell’importo complessivo in relazione ai volumi e al prezzo medio del periodo di fatturazione. Per la `quota per consumi` espone la quantità, il `prezzo medio` e l’importo totale risultante dal prodotto delle due grandezze.

## Citazione
"Lo Scontrino dell’energia riporta la formazione dell’importo complessivo dell’energia, in relazione ai volumi e al prezzo medio"; "la quantità ... il prezzo medio ... l’importo totale risultante dal prodotto delle due grandezze"

## Interpretazione minima
La logica customer-facing dello Scontrino è una decomposizione sintetica `Q × P = I`, non l’esposizione integrale di tutti i corrispettivi unitari applicati, che restano rinviati agli `Elementi di dettaglio`.

## Impatto operativo
Nel SSOT la rappresentazione dello Scontrino va separata dalla struttura analitica dei corrispettivi. I motori di rendering devono poter calcolare o leggere quantità, prezzo medio e importo per quota consumi, quota fissa e, se applicabile, quota potenza.

## Eccezioni e limiti
Il prezzo medio è un valore di sintesi e non coincide necessariamente con un unico prezzo contrattuale elementare.

## Conflitti o dipendenze
Si coordina con RULE-EE-BOL-004, RULE-EE-PRC-001 e con il Glossario elettrico SRC-ARERA-204-2025-R-COM-ALLEGATO-A.

## Note
Il Glossario elettrico rende esplicita la formula sintetica come `Q x P = I`.
