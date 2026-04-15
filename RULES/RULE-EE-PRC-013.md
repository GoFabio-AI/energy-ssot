# RULE-EE-PRC-013

## Metadata
- ID: RULE-EE-PRC-013
- Titolo: La razionalizzazione 2026 copre tutte le offerte domestiche, mentre prodotti e servizi aggiuntivi restano separati dal nucleo prezzo energia
- Dominio: contratti-offerte-trasparenza
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-386-2025-R-COM-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/25/386-2025-R-com.pdf
- Riferimento preciso: motivazione, pagina 26, lettera A.1; motivazione, pagina 31; coordinamento con articolo 10 come modificato
- Data pubblicazione: 2025-08-05
- Data ultima verifica: 2026-04-15

## Testo normalizzato
La razionalizzazione 2026 dei corrispettivi si applica a tutte le offerte di energia elettrica, sia a prezzo fisso sia a prezzo variabile, rivolte ai clienti finali domestici. I corrispettivi afferenti a prodotti e servizi aggiuntivi inclusi nell'offerta non rientrano però nel nucleo razionalizzato del prezzo di vendita energia e devono essere evidenziati a parte nella sezione contrattuale delle condizioni economiche, con le relative informazioni utili e condizioni di recesso.

## Citazione
"relativamente a tutte le offerte di energia elettrica ... rivolte ai clienti finali domestici"; "i corrispettivi afferenti a prodotti e/o servizi aggiuntivi"; "non rientrano nell’ambito di applicazione degli interventi di razionalizzazione"; "dovranno essere evidenziati a parte"; "relative condizioni di recesso"

## Interpretazione minima
Nel SSOT l'etichetta `offerta non generalizzata` va trattata come esclusione dal perimetro di comparabilità del Portale Offerte, non come esenzione dagli obblighi 2026 di struttura e disclosure delle condizioni economiche quando l'offerta è comunque rivolta a clienti domestici. Allo stesso tempo bundle, bonus e servizi accessori non vanno confusi con il prezzo energia razionalizzato: restano in layer separato.

## Impatto operativo
I modelli dati devono separare almeno quattro blocchi: `corrispettivi_vendita_razionalizzati`, `corrispettivi_regolati`, `sconti_bonus`, `prodotti_servizi_aggiuntivi`. La classificazione `generalizzata/non_generalizzata` governa Portale e comparabilità, non l'applicazione del blocco disclosure domestico di base.

## Eccezioni e limiti
La regola chiude il boundary minimo di struttura e disclosure, ma non esaurisce l'intera valutazione sostanziale consumer-law o marketing-law di bundle e promozioni. L'obbligo di pubblicazione sul sito del venditore resta invece espressamente limitato alle offerte in corso di validità pubblicate sul Portale Offerte.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRC-009, RULE-EE-PRC-010 e RULE-EE-CCC24-001.

## Note
Questa regola riduce il residuo aperto sulle offerte non generalizzate distinguendo il piano `fuori Portale` dal piano `fuori disclosure`, che non coincidono.
