# RULE-EE-DISP-003

## Metadata
- ID: RULE-EE-DISP-003
- Titolo: In maggior tutela il dispacciamento lato cliente è presente sia nell'elemento `PD` sia nella componente `DISPBT`
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIV-2026-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/Allegato_A_TIV_valido__dal_1_gennaio_2026.pdf
- Riferimento preciso: definizioni in articolo 1, articolo 10.1, 10.2, 10.4 e 10.7
- Data pubblicazione: 2026-01-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel servizio di maggior tutela, il dispacciamento lato cliente non coincide con il solo elemento `PD`: il TIV definisce `PD` come elemento del `PED` a copertura dei costi di dispacciamento e mantiene separata anche la componente `DISPBT` tra i corrispettivi unitari applicati al cliente.

## Citazione
"elemento PD (prezzo dispacciamento) è l’elemento del corrispettivo PED"; "la componente DISPBT"

## Interpretazione minima
Nel SSOT il dispacciamento economico in maggior tutela va modellato almeno su due piani distinti, `PD` nella quota energia e `DISPBT` nella quota per punto/anno.

## Impatto operativo
I modelli di pricing, i controlli di coerenza e i mapping customer-facing non devono comprimere `DISPBT` dentro `PD`, né usare `PED` come sinonimo esaustivo di tutte le componenti di dispacciamento della maggior tutela.

## Eccezioni e limiti
La regola riguarda la maggior tutela e non sostituisce la formula STG del `CDISPD` né chiude il trattamento del dispacciamento nelle offerte di mercato libero.

## Conflitti o dipendenze
Si coordina con RULE-EE-DISP-001, RULE-EE-DISP-002, RULE-EE-TIV-002 e RULE-EE-PRC-005.

## Note
Le fonti ARERA lato consumatore aggregano poi `PD` e `DISPBT` nella label legacy `materia energia`, ma il SSOT deve conservarne la distinzione regolatoria.
