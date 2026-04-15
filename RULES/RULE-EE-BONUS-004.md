# RULE-EE-BONUS-004

## Metadata
- ID: RULE-EE-BONUS-004
- Titolo: Nel 2026 il bonus sociale elettrico ordinario ha importi ARERA differenziati per numerosità familiare con valori annuali, giornalieri e per 30 giorni
- Dominio: bonus-sociale
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BONUS-AMMONTANO
- URL fonte: https://www.arera.it/consumatori/bonus-sociale/bonus-sociale-per-disagio-economico/a-quanto-ammontano
- Riferimento preciso: pagina ARERA "A quanto ammontano", sezione bonus elettrico per disagio economico, tabella anno 2026
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per l'anno 2026 il bonus sociale elettrico ordinario per POD è pari a 146,00 euro/anno, 0,40 euro/giorno e 12,00 euro per 30 giorni per nuclei di 1-2 componenti; 186,15 euro/anno, 0,51 euro/giorno e 15,30 euro per 30 giorni per nuclei di 3-4 componenti; 204,40 euro/anno, 0,56 euro/giorno e 16,80 euro per 30 giorni per nuclei oltre 4 componenti.

## Citazione
"Numerosità familiare 1-2 componenti 146,00 0,40 12,00"; "Numerosità familiare 3-4 componenti 186,15 0,51 15,30"; "Numerosità familiare oltre 4 componenti 204,40 0,56 16,80"

## Interpretazione minima
Il SSOT può modellare in modo chiuso gli importi ordinari 2026 del bonus elettrico per POD distinguendo tre bande di numerosità familiare e mantenendo sia il valore annuale sia i valori giornalieri e per 30 giorni pubblicati da ARERA.

## Impatto operativo
Pricing regolatorio, billing, CRM e supporto clienti devono usare queste tre fasce importo come baseline 2026 del bonus ordinario e non confonderle con il contributo straordinario 2025.

## Eccezioni e limiti
La regola riguarda solo il bonus sociale elettrico ordinario 2026 per disagio economico. Non copre bonus gas, bonus idrico, bonus per disagio fisico né contributi straordinari temporanei.

## Conflitti o dipendenze
Dipende dalle regole su requisiti ISEE e ammissibilità della fornitura. Si coordina con `RULE-EE-BONUS-005` per la rappresentazione in bolletta.

## Note
La pagina ARERA indica espressamente che i valori 2026 sono in vigore dal I trimestre 2026 fino al 31 dicembre 2026.
