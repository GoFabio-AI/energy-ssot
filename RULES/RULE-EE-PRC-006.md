# RULE-EE-PRC-006

## Metadata
- ID: RULE-EE-PRC-006
- Titolo: Nella guida ARERA la label legacy `materia energia` in maggior tutela comprende `PE`, `PD`, `PPE`, `PCV` e `DISPBT`
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-GUIDA-VOCI-SPESA
- URL fonte: https://www.arera.it/bolletta/guida-alla-lettura-delle-voci-di-spesa
- Riferimento preciso: sezione dedicata alla `Spesa per la materia energia` per clienti in maggior tutela
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nelle fonti ARERA lato consumatore, per i clienti in maggior tutela la label legacy `Spesa per la materia energia` comprende le componenti `PE`, `PD`, `PPE`, `PCV` e `DispBT`.

## Citazione
"componenti energia (PE), dispacciamento (PD), perequazione (PPE), commercializzazione (PCV), componente di dispacciamento (DispBT)"

## Interpretazione minima
Nel SSOT la label legacy `materia energia` può essere trattata come alias esplicativo solo se resta ancorata al perimetro e alla fonte che la usano, senza sostituire la nomenclatura primaria della Bolletta 2025.

## Impatto operativo
I parser bolletta e i modelli semantici devono poter ricondurre il label legacy `materia energia` alla scomposizione `PE/PD/PPE/PCV/DISPBT` quando stanno lavorando su contenuti ARERA di maggior tutela o su dettaglio storico coerente.

## Eccezioni e limiti
La guida ARERA è fonte ufficiale di supporto lato consumatore e non sostituisce la disciplina primaria della Bolletta 2025 né autorizza estensioni automatiche al mercato libero.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRC-001, RULE-EE-PRC-002, RULE-EE-PRC-003, RULE-EE-PRC-004 e RULE-EE-TIV-002.

## Note
La stessa guida usa anche i label legacy `trasporto e gestione del contatore` e `oneri di sistema`, utili come alias ma non come nomenclatura primaria vigente.
