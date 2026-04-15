# RULE-EE-PRC-011

## Metadata
- ID: RULE-EE-PRC-011
- Titolo: Nelle offerte domestiche onnicomprensive i corrispettivi includono tutte le voci di spesa e non richiedono la scomposizione separata di dispacciamento, rete e oneri
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-386-2025-R-COM-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/25/386-2025-R-com.pdf
- Riferimento preciso: Allegato A alla deliberazione 555/2017/R/com, articolo 1, comma 1.6, e articolo 10.3bis, come modificati dalla deliberazione 386/2025/R/com
- Data pubblicazione: 2025-08-05
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nelle offerte domestiche di energia elettrica del mercato libero con corrispettivi onnicomprensivi il venditore applica un unico corrispettivo in quota annua e un unico corrispettivo dipendente dal consumo. Nella sezione economica il venditore non è tenuto a suddividere le sottosezioni dedicate ai corrispettivi regolati, ma deve riportare una tabella recante la dicitura `Corrispettivi onnicomprensivi` e una dicitura che specifichi che i corrispettivi includono tutte le voci di spesa.

## Citazione
"il venditore non è tenuto a suddividere"; "Corrispettivi onnicomprensivi"; "i corrispettivi includono tutte le voci di spesa"

## Interpretazione minima
Nel SSOT, quando l’offerta è qualificata come `onnicomprensiva`, dispacciamento, tariffa rete e oneri generali non sono componenti separatamente ricostruibili dalla tabella commerciale customer-facing dell’offerta. Vanno quindi marcati come `inclusi` e non come bucket autonomamente valorizzati.

## Impatto operativo
I modelli pricing devono distinguere in modo esplicito il flag `onnicomprensiva` e impedire tentativi di scomposizione artificiale del prezzo in `dispacciamento`, `rete` e `oneri` quando la fonte disponibile è solo la tabella commerciale standardizzata dell’offerta.

## Eccezioni e limiti
La regola non elimina l’obbligo di indicare i valori unitari effettivi e le modalità di applicazione dei corrispettivi onnicomprensivi. Non si applica alle offerte non onnicomprensive, per le quali la disciplina richiede invece evidenza separata del corrispettivo dispacciamento/capacità e dei bucket regolati richiamati.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRC-007, RULE-EE-PRC-010 e RULE-EE-DISP-004.

## Note
Questa regola chiude l’edge case residuo del libero domestico in cui il dispacciamento resta economicamente presente ma non più separatamente esposto nel layout commerciale.