# EXTRACTED - SRC-ARERA-MT-VALORI-2026-XLSX

## Metadata
- Source ID: SRC-ARERA-MT-VALORI-2026-XLSX
- URL: https://www.arera.it/fileadmin/area_operatori/prezzi_e_tariffe/E2026-smt.xlsx
- Date extracted: 2026-04-15
- Tool: local python extraction (openpyxl)
- Relevance: alta per il dettaglio numerico delle componenti customer-facing e regolatorie in maggior tutela

## Fatti chiave ad alta confidenza
1. Il foglio ARERA si presenta come `Condizioni economiche per i clienti del Servizio di maggior tutela`, con `Valori al netto delle imposte`.
2. Il workbook avverte che le tabelle sono pubblicate `solo a scopo informativo` e che il valore dei corrispettivi approvati risulta esclusivamente dai provvedimenti pubblicati su arera.it.
3. Nel foglio `apr-giu 2026`, per i clienti vulnerabili, ARERA espone già la tassonomia customer-facing: materia energia, trasporto e gestione del contatore, oneri di sistema.
4. Per abitazioni di residenza anagrafica in aprile-giugno 2026, la quota energia monoraria della materia energia è pari a `0,15811 euro/kWh`, composta da `PE 0,15086`, `PD 0,01752` e `PPE -0,01027`.
5. Nello stesso foglio, la quota fissa annua è pari a `44,7311 euro/anno`, composta da `PCV 43,5` e `DISPbt 1,2311`.
6. Il foglio conferma che rete e oneri restano bucket separati: `σ1, σ2, σ3, UC3, UC6` per trasporto e gestione del contatore, `ASOS` e `ARIM` per gli oneri di sistema.

## Citazioni utili
- `Condizioni economiche per i clienti del Servizio di maggior tutela`
- `Valori al netto delle imposte`
- `Queste tabelle sono pubblicate solo a scopo informativo`
- `Materia energia: energia (PE), dispacciamento (PD), commercializzazione vendita (PCV), componenti di perequazione (PPE) e di dispacciamento (DISPbt)`
- `Quota energia (euro/kWh) ... 0,15086 ... 0,01752 ... -0,01027 ... 0,15811`
- `Quota fissa (euro/anno) ... 43,5 ... 1,2311 ... 44,7311`

## Uso nel SSOT
- fonte ufficiale numerica per verificare il passaggio da componenti regolatorie a valore customer-facing della materia energia in maggior tutela
- supporto operativo per formule e controlli bolletta nel trimestre rilevante al 2026-04-15

## Limiti noti
- il foglio è dichiarato informativo dalla stessa ARERA; in caso di conflitto prevale il provvedimento normativo e il TIV consolidato
