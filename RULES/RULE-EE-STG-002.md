# RULE-EE-STG-002

## Metadata
- ID: RULE-EE-STG-002
- Titolo: Nel servizio a tutele graduali domestico non vulnerabile la formula regolata distingue CELD, CDISPD, CSED, CPSTGD e γ
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIV-2026-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/Allegato_A_TIV_valido__dal_1_gennaio_2026.pdf
- Riferimento preciso: Articolo 48.6, 48.8, 48.10, 48.11, 48.13 e 48.15
- Data pubblicazione: 2026-01-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti domestici non vulnerabili nel servizio a tutele graduali, le condizioni economiche si articolano nei corrispettivi `CELD`, `CDISPD`, `CSED`, `CPSTGD` e nel parametro `γ`. Il `CDISPD` è determinato come prodotto tra `λ` e la somma del corrispettivo di capacità e dei corrispettivi applicati da Terna per il servizio di dispacciamento, con le esclusioni espressamente previste dal TIV. I corrispettivi di trasporto, distribuzione, misura e le aliquote A e UC sono applicati separatamente dall’esercente sulla base di quanto applicato dal distributore.

## Citazione
"Le condizioni economiche ... si articolano nei seguenti corrispettivi unitari: a) corrispettivo CELD; b) corrispettivo CDISPD; c) corrispettivo CSED; d) corrispettivo CPSTGD; e) parametro γ."

## Interpretazione minima
Nel SSOT STG domestico la parte commodity regolata e la parte rete/oneri applicata dal distributore devono restare distinte.

## Impatto operativo
La rappresentazione minima del prezzo STG domestico deve almeno separare quota consumo (`CELD + CDISPD + CSED + CPSTGD`) e quota per POD/anno (`γ`), mantenendo fuori da questa formula la rete e gli oneri applicati dal distributore.

## Eccezioni e limiti
La regola non chiude l’intera baseline TIV/TIT/TIDE né l’eventuale variabilità successiva a modifiche ulteriori rispetto alla versione valida dall’1 gennaio 2026.

## Conflitti o dipendenze
Dipende da RULE-EE-DISP-001 e si coordina con RULE-EE-PRC-003 e RULE-EE-PRC-004.

## Note
Nella versione verificata del TIV valida dall’1 gennaio 2026, la Tabella 21 riporta `CSED = 0,056`, la Tabella 22 `CPSTGD = -0,033` dal 2026-01-01 e la Tabella 23 `γ = -7.316,37` dal 2025-07-01.
