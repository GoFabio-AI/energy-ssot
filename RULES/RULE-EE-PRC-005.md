# RULE-EE-PRC-005

## Metadata
- ID: RULE-EE-PRC-005
- Titolo: Al 2026-04-15 ARERA pubblica per la maggior tutela una materia energia customer-facing riconducibile a `PE + PD + PPE` e `PCV + DISPBT`
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-MT-VALORI-2026-XLSX
- URL fonte: https://www.arera.it/fileadmin/area_operatori/prezzi_e_tariffe/E2026-smt.xlsx
- Riferimento preciso: foglio `apr-giu 2026`, sezione `Abitazioni di residenza anagrafica`, righe quota energia e quota fissa
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti domestici vulnerabili in maggior tutela, il foglio ARERA verificato al 2026-04-15 pubblica, per il trimestre aprile-giugno 2026, una `Materia energia` monoraria pari a `0,15811 euro/kWh`, risultante da `PE 0,15086 + PD 0,01752 + PPE -0,01027`, e una quota fissa annua pari a `44,7311 euro/anno`, risultante da `PCV 43,5 + DISPBT 1,2311`. Nel periodo verificato, la rappresentazione customer-facing minima è quindi `quota consumi = PED + PPE = PE + PD + PPE` e `quota fissa = PCV + DISPBT`.

## Citazione
`Quota energia (euro/kWh) ... PE 0,15086 ... PD 0,01752 ... PPE -0,01027 ... Materia energia 0,15811`

## Interpretazione minima
Il dato customer-facing della `Materia energia` in maggior tutela può essere ricostruito in modo rigoroso come somma di componenti regolatorie pubblicate da ARERA per il periodo corrente, distinguendo parte a consumo e parte fissa.

## Impatto operativo
Il SSOT può verificare la coerenza tra dettaglio componenti e prezzo finale della `Materia energia` per il trimestre di riferimento, mantenendo separate le imposte e le bucket rete/oneri e senza comprimere `DISPBT` dentro `PD`.

## Eccezioni e limiti
La regola è periodizzata su aprile-giugno 2026 ed è ricavata da un foglio ARERA dichiarato informativo; in caso di conflitto prevalgono i provvedimenti normativi e il TIV.

## Conflitti o dipendenze
Dipende da RULE-EE-TIV-002 e RULE-EE-TIV-003; si coordina con RULE-EE-PRC-002.

## Note
La pagina consumatori `SRC-ARERA-MT-VALORI-2026-PAGE` espone lo stesso prezzo in forma customer-facing, senza il dettaglio analitico delle componenti.
