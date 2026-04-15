# RULE-EE-TIF-004

## Metadata
- ID: RULE-EE-TIF-004
- Titolo: Le stime del venditore devono basarsi sui consumi storici effettivi del cliente e rispettare uno standard generale
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIF-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/16/TIF_All_a_aggiornato_dal_1__luglio_2025__463-16_.pdf
- Riferimento preciso: Articolo 6, comma 6.2; Articolo 10, commi 10.1-10.3; Tabella 4
- Data pubblicazione: 2025-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Quando il venditore utilizza una propria stima, deve determinare il dato di misura stimato sulla base dei consumi storici effettivi del cliente forniti dal distributore, eventualmente integrati con altre informazioni ritenute utili. Nel settore elettrico la qualità complessiva delle stime è presidiata da uno standard generale semestrale di incidenza dei consumi stimati rispetto ai consumi effettivi pari a `≤ 0,50`.

## Citazione
"il venditore determina il dato di misura stimato sulla base dei consumi storici effettivi del cliente"; "Energia elettrica ≤ 0,50"

## Interpretazione minima
La base primaria della stima è la storia effettiva del singolo cliente, non una stima astratta sganciata dai dati disponibili.

## Impatto operativo
I motori di stima devono usare come input prioritario la storia effettiva fornita dal distributore e devono supportare KPI di qualità semestrali.

## Eccezioni e limiti
Lo standard `≤ 0,50` è un indicatore aggregato di qualità per venditore, non un limite numerico applicabile automaticamente a ogni singola bolletta.

## Conflitti o dipendenze
Dipende da RULE-EE-TIF-002 per l’ordine che consente di arrivare alla stima e si riflette in RULE-EE-BOLL-001 per i ricalcoli successivi.

## Note
Le stime possono essere superate da successivi dati effettivi o autoletture validate, generando conguagli o ricalcoli.