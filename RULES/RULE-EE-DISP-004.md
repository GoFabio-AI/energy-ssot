# RULE-EE-DISP-004

## Metadata
- ID: RULE-EE-DISP-004
- Titolo: Nelle offerte domestiche libere elettriche variabili con aggiornamento almeno orario il corrispettivo dispacciamento/capacità può sostituire il CDISPD con i valori Terna/TIDE
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-386-2025-R-COM-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/25/386-2025-R-com.pdf
- Riferimento preciso: Allegato A alla deliberazione 555/2017/R/com, articolo 1, comma 1.2, lettera b), come modificato dalla deliberazione 386/2025/R/com
- Data pubblicazione: 2025-08-05
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per le offerte domestiche di energia elettrica del mercato libero che non prevedono corrispettivi onnicomprensivi, il corrispettivo separato a copertura del servizio di dispacciamento e del mercato della capacità è di regola pari al valore del `CDISPD` determinato e aggiornato dall’Autorità. Tuttavia, se l’offerta è a prezzo variabile con frequenza di aggiornamento almeno oraria, il venditore può applicare in sostituzione del `CDISPD` la somma del corrispettivo a copertura degli oneri netti di approvvigionamento della capacità definito da Terna e del corrispettivo di dispacciamento di cui alla Sezione 4-25 del `TIDE`.

## Citazione
"nel caso di offerte di energia elettrica con prezzo variabile con frequenza di aggiornamento almeno orari"; "in sostituzione del corrispettivo CDISPD"; "la somma del corrispettivo a copertura degli oneri netti di approvvigionamento della capacità ... e del corrispettivo di dispacciamento di cui alla Sezione 4-25 del TIDE"

## Interpretazione minima
Nel SSOT il dispacciamento del libero domestico con evidenza separata non ha un solo schema regolatorio riusabile. Occorre distinguere almeno il caso standard valorizzato a `CDISPD` e il caso eccezionale delle offerte variabili almeno orarie valorizzato con la combinazione `capacità Terna + dispacciamento TIDE`.

## Impatto operativo
I modelli dati e i parser delle condizioni economiche devono prevedere almeno due stati per il corrispettivo separato di dispacciamento/capacità nel libero domestico: `cdispd_autorita` e `terna_tide_orario`. Non va forzata la seconda casistica dentro un semplice alias del `CDISPD`.

## Eccezioni e limiti
La regola riguarda solo offerte domestiche elettriche non onnicomprensive e non impone che tutte le offerte orarie usino l’opzione sostitutiva. Non si estende alle offerte onnicomprensive, dove i corrispettivi confluiscono nel prezzo unico dell’offerta.

## Conflitti o dipendenze
Si coordina con RULE-EE-DISP-001, RULE-EE-PRC-007, RULE-EE-PRC-008 e RULE-EE-PRC-011.

## Note
Questa regola chiude il principale edge case residuo del dispacciamento nel libero domestico per le offerte orarie articolate.