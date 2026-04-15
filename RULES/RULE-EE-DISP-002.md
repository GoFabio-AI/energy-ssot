# RULE-EE-DISP-002

## Metadata
- ID: RULE-EE-DISP-002
- Titolo: Nel servizio a tutele graduali il corrispettivo CDISPD è la traduzione customer-facing del dispacciamento con esclusioni espresse dal TIV
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIV-2026-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/Allegato_A_TIV_valido__dal_1_gennaio_2026.pdf
- Riferimento preciso: Articolo 48.8 e 48.9
- Data pubblicazione: 2026-01-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti domestici non vulnerabili nel servizio a tutele graduali, `CDISPD` è determinato come prodotto tra il parametro `λ` e la somma del corrispettivo di capacità e dei corrispettivi applicati da Terna per il servizio di dispacciamento, con esclusione del corrispettivo di sbilanciamento effettivo, del corrispettivo a copertura dell’onere netto di approvvigionamento della capacità di cui all’articolo 23bis del TIS e del corrispettivo di aggregazione misure di cui all’articolo 15 del TIS.

## Citazione
`Il corrispettivo CDISPD è determinato come prodotto tra il parametro λ ... e la somma del corrispettivo di capacità ... e dei corrispettivi applicati da Terna per il servizio di dispacciamento`

## Interpretazione minima
Nel SSOT il dispacciamento economico STG va modellato come corrispettivo derivato da componenti Terna e capacità, non come semplice sinonimo di una fee commerciale generica.

## Impatto operativo
I motori di pricing e riconciliazione STG devono separare `CDISPD` da `CELD`, `CSED` e `CPSTGD`, e non devono inglobare nel corrispettivo le esclusioni nominate dal TIV.

## Eccezioni e limiti
La regola riguarda solo il perimetro STG domestico non vulnerabile e non chiude la rappresentazione del dispacciamento nel mercato libero.

## Conflitti o dipendenze
Si coordina con RULE-EE-DISP-001 e RULE-EE-STG-002.

## Note
L’articolo 48.9 collega il corrispettivo di capacità ai costi attribuibili ai clienti finali in tutele graduali connessi al corrispettivo applicato all’utente del dispacciamento.
