# EXTRACTED - SRC-ARERA-STG-VALORI-2026-XLSX

## Metadata
- Source ID: SRC-ARERA-STG-VALORI-2026-XLSX
- URL: https://www.arera.it/fileadmin/area_operatori/prezzi_e_tariffe/E2026_stg_domesticiNonVulnerabili.xlsx
- Date extracted: 2026-04-15
- Tool: local python extraction (openpyxl)
- Relevance: alta per il dettaglio numerico delle componenti customer-facing e regolatorie nel servizio a tutele graduali

## Fatti chiave ad alta confidenza
1. Il foglio ARERA si presenta come `Condizioni economiche per i clienti del Servizio a tutele graduali`, con `Valori al netto delle imposte`.
2. Il workbook avverte che le tabelle sono pubblicate `solo a scopo informativo` e che il valore dei corrispettivi approvati risulta esclusivamente dai provvedimenti pubblicati su arera.it.
3. Nel foglio `mar 2026`, per i clienti domestici non vulnerabili senza fornitura nel mercato libero, ARERA espone la tassonomia customer-facing: vendita di energia elettrica, tariffa per l’uso della rete elettrica, oneri generali di sistema.
4. Per abitazioni di residenza anagrafica nel mese di marzo 2026, la quota energia monoraria della vendita è pari a `0,174479 euro/kWh`, composta da `CELD 0,15774`, `CDISPD 0,016509`, `CSED 0,00056` e `CPSTGD -0,00033`.
5. Nello stesso foglio, la quota fissa annua è pari a `-73,1637 euro/anno`, coincidente con il `parametro γ`.
6. Il foglio conferma che rete e oneri restano bucket separati: `σ1, σ2, σ3, UC3, UC6` per la rete e `ASOS`, `ARIM` per gli oneri di sistema.

## Citazioni utili
- `Condizioni economiche per i clienti del Servizio a tutele graduali`
- `Valori al netto delle imposte`
- `Queste tabelle sono pubblicate solo a scopo informativo`
- `Vendita di energia elettrica: energia (CELD), dispacciamento (CDISPD), commercializzazione vendita (parametro γ), sbilanciamento (CSED), perequazione (CPSTGD)`
- `Quota energia (euro/kWh) ... 0,15774 ... 0,016509 ... 0,00056 ... -0,00033 ... 0,174479`
- `Quota fissa (euro/anno) ... parametro γ ... -73,1637`

## Uso nel SSOT
- fonte ufficiale numerica per verificare il passaggio da componenti regolatorie STG a valore customer-facing della vendita nel mese rilevante al 2026-04-15
- supporto operativo per formule, riconciliazioni e controlli di bolletta STG domestica

## Limiti noti
- il foglio è dichiarato informativo dalla stessa ARERA; in caso di conflitto prevale il provvedimento normativo e il TIV consolidato
