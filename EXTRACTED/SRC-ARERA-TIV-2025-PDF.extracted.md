# EXTRACTED - SRC-ARERA-TIV-2025-PDF

## Metadata
- Source ID: SRC-ARERA-TIV-2025-PDF
- URL: https://www.arera.it/fileadmin/allegati/docs/23/362-23TIV.pdf
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf)
- Relevance: molto alta per formule regolatorie domestiche luce

## Fatti chiave ad alta confidenza
1. Il PDF è il TIV consolidato con frontespizio "Valido dall’8 aprile 2025".
2. Per il servizio di maggior tutela, le condizioni economiche si articolano in `PED`, `PCV`, `PPE` e `DISPBT`.
3. Il TIV stabilisce espressamente che `PED = PE + PD`.
4. Il TIV definisce `PE` come elemento a copertura dei costi di acquisto dell’energia e `PD` come elemento a copertura dei costi di dispacciamento.
5. Il TIV definisce `PCV` come corrispettivo di commercializzazione vendita, `PPE` come corrispettivo di perequazione energia e `DISPBT` come componente di dispacciamento a copertura di specifici meccanismi del TIV.
6. Per il servizio a tutele graduali dei clienti domestici non vulnerabili, le condizioni economiche si articolano in `CELD`, `CDISPD`, `CSED`, `CPSTGD` e `γ`.
7. `CDISPD` è definito da formula come prodotto tra `λ` e la somma del corrispettivo di capacità e dei corrispettivi applicati da Terna per il servizio di dispacciamento, con esclusioni espresse nel testo.
8. Nel servizio STG domestico non vulnerabile, i corrispettivi di trasporto, distribuzione, misura e le aliquote A e UC sono applicati separatamente dall’esercente, sulla base di quanto applicato dal distributore.
9. Nella versione verificata del TIV, la Tabella 21 riporta `CSED = 0,056` centesimi di euro/kWh; la Tabella 22 riporta `CPSTGD = -2,086` centesimi di euro/kWh dal 2025-04-01; la Tabella 23 riporta `γ = -7.265,42` centesimi di euro/POD/anno dal 2024-07-01.

## Citazioni utili
- "Valido dall’8 aprile 2025"
- "Le condizioni economiche ... maggior tutela ... PED ... PCV ... PPE ... DISPBT"
- "Il corrispettivo PED è fissato pari alla somma dei seguenti elementi: a) PE; b) PD"
- "Le condizioni economiche ... tutele graduali ... CELD ... CDISPD ... CSED ... CPSTGD ... parametro γ"
- "L’esercente le tutele graduali applica ... i corrispettivi ... per i servizi di trasporto, distribuzione e misura"

## Uso nel SSOT
- base primaria per la formula regolatoria del domestico in maggior tutela
- base primaria per la formula regolatoria del domestico non vulnerabile in STG
- base primaria per la collocazione economica del dispacciamento nei regimi regolati domestici

## Limiti noti
- Il pacchetto non estende la verifica a tutta la baseline consolidata TIV/TIT/TIDE al 2026-04-15.
- Il parametro `λ` è richiamato dal testo e usato nelle formule; per il checkpoint 2026-04-15 questo file resta materiale di raccordo storico rispetto al baseline composito ormai chiuso con `TIV 2026 + DL 19/2025 + ARERA 110/2025 + ARERA 96/2026 + TIT + TIDE`.
