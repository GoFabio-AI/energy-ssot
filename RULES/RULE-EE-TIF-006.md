# RULE-EE-TIF-006

## Metadata
- ID: RULE-EE-TIF-006
- Titolo: Nei cambi venditore e nelle volture su punti monorari il cliente può comunicare l’autolettura da 5 giorni lavorativi prima a 3 dopo
- Dominio: misure
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIF-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/16/TIF_All_a_aggiornato_dal_1__luglio_2025__463-16_.pdf
- Riferimento preciso: Articoli 13 e 14
- Data pubblicazione: 2025-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nei casi di cessazione della fornitura di energia elettrica, esclusa la disattivazione, con riferimento ai punti di prelievo trattati monorari, il cliente può comunicare l’autolettura nel periodo compreso tra il quinto giorno lavorativo precedente e il terzo giorno lavorativo successivo alla decorrenza del cambio venditore o della voltura. Il venditore deve informare il cliente della possibilità di comunicarla, delle modalità e delle tempistiche, esplicitando il periodo utile.

## Citazione
"il periodo compreso tra il quinto giorno lavorativo precedente ed il terzo giorno lavorativo successivo"; "i venditori informano ... della possibilità di comunicare l’autolettura ... delle modalità e tempistiche per effettuarla"

## Interpretazione minima
La regola serve a formare il dato di confine tra vecchio e nuovo rapporto di fornitura o tra precedente e nuovo intestatario quando il punto è monorario.

## Impatto operativo
Workflow di switching e voltura devono aprire una finestra di raccolta autolettura e indirizzarla al venditore uscente o entrante secondo la data di comunicazione.

## Eccezioni e limiti
La disciplina è limitata ai punti trattati monorari e ai casi di cessazione senza disattivazione.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIF-003 per la gestione retail dell’autolettura e con RULE-EE-TIME-002 per la sua validazione tecnica.

## Note
Nel cambio venditore l’autolettura va al venditore uscente se comunicata entro il giorno precedente la data di cambio, e al venditore entrante se comunicata da quella data in avanti.