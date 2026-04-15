# RULE-EE-TIF-003

## Metadata
- ID: RULE-EE-TIF-003
- Titolo: Per i punti monorari o non dotati di smart meter il venditore deve gestire l’autolettura in finestra
- Dominio: misure
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIF-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/16/TIF_All_a_aggiornato_dal_1__luglio_2025__463-16_.pdf
- Riferimento preciso: Articolo 7, commi 7.1, 7.2 e 7.3
- Data pubblicazione: 2025-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti con punti trattati monorari ai sensi del TIS o non dotati di smart meter, il venditore deve mettere a disposizione almeno una modalità di raccolta dell’autolettura, indicare in ogni bolletta la finestra temporale utile, comunicare la presa in carico o la non presa in carico del dato e trasmettere al distributore i dati raccolti nella finestra entro 4 giorni lavorativi dall’acquisizione.

## Citazione
"mettere a disposizione almeno una modalità di raccolta dell’autolettura"; "indicare in ogni bolletta sintetica la finestra temporale"; "entro e non oltre 4 (quattro) giorni lavorativi successivi"

## Interpretazione minima
La non presa in carico è ammessa solo se il dato è palesemente errato, cioè differisce dall’ultimo dato effettivo disponibile di almeno un ordine di grandezza.

## Impatto operativo
Servono canali di raccolta attivi, SLA di presa in carico e invio al distributore, e un controllo di plausibilità limitato ai casi di errore manifesto.

## Eccezioni e limiti
La regola è circoscritta ai punti del comma 7.1. Le autoletture extra-finestra seguono la disciplina dell’articolo 8.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIME-002 per la validazione dell’autolettura e con RULE-EE-BOLL-001 per l’esposizione della finestra in bolletta.

## Note
Il TIF impone almeno un canale, ma non vincola a una sola modalità tecnica.