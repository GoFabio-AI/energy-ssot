# RULE-EE-PRC-003

## Metadata
- ID: RULE-EE-PRC-003
- Titolo: Per il domestico TIV la spesa rete può includere solo σ1, σ2, σ3, UC3 e UC6
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: Allegato A, Tabella 1, riga "Spesa per la tariffa per l’uso della rete elettrica", clienti articolo 2.3 lettera a) del TIV
- Data pubblicazione: 2024-07-23
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti di cui all’articolo 2.3 lettera a) del TIV, nella `Spesa per la tariffa per l’uso della rete elettrica` possono essere ricompresi solo ed esclusivamente `σ1`, `σ2`, `σ3`, `UC3` e `UC6`.

## Citazione
"Possono essere ricompresi solo ed esclusivamente: σ1, σ2, σ3, UC3, UC6"

## Interpretazione minima
La bucket rete del domestico TIV è chiusa a questo set minimo di componenti customer-facing.

## Impatto operativo
I motori di classificazione e le riconciliazioni bolletta non devono collocare in questa voce né `ARIM/ASOS` né corrispettivi di vendita.

## Eccezioni e limiti
La regola è scritta sul perimetro clienti articolo 2.3 lettera a) TIV e non sostituisce la regolazione tariffaria tecnica di livello TIT.

## Conflitti o dipendenze
Dipende dalla corretta classificazione domestica TIV e si coordina con RULE-EE-TIV-001.

## Note
La legenda della Bolletta 2025 chiarisce che la bucket rete copre trasmissione, distribuzione e misura.
