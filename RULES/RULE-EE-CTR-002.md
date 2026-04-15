# RULE-EE-CTR-002

## Metadata
- ID: RULE-EE-CTR-002
- Titolo: Nel Portale Offerte gli sconti automatici dei primi 12 mesi entrano nella spesa annua stimata, mentre le altre promozioni restano nel dettaglio
- Dominio: contratti-offerte-trasparenza
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-PORTALE-OFFERTE-2024-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/18/051-18all_ti.pdf
- Riferimento preciso: articolo 10, commi 10.7 e 10.8; articolo 12
- Data pubblicazione: 2024-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel Portale Offerte la `spesa annua stimata` incorpora gli sconti applicati automaticamente nei primi 12 mesi di fornitura. Le altre promozioni o sconti non automatici non entrano nel calcolo della stima e devono restare rappresentati nella pagina di dettaglio dell'offerta, insieme alle relative condizioni e tempistiche di applicazione. Anche servizi o prodotti aggiuntivi con relativi corrispettivi e condizioni di recesso restano su un layer descrittivo separato rispetto alla sola stima numerica.

## Citazione
"Eventuali altri sconti non sono considerati ai fini della suddetta stima, ma sono rappresentati unicamente nella pagina di dettaglio"; "eventuali corrispettivi richiesti e delle relative condizioni di recesso"

## Interpretazione minima
Nel SSOT non tutti gli sconti o bonus hanno lo stesso peso comparativo. Occorre distinguere tra promozioni che incidono direttamente sulla metrica ufficiale di comparazione del Portale e promozioni che restano soltanto descrittive nel dettaglio dell'offerta.

## Impatto operativo
I modelli offerta devono prevedere almeno i campi `sconto_automatico_12_mesi_in_stima`, `promozione_detail_only`, `condizioni_promozione` e `servizi_aggiuntivi_detail_only`. Non va appiattita in un solo flag la differenza tra sconto numericamente incorporato nella stima e promozione soltanto narrativa o condizionata.

## Eccezioni e limiti
La regola riguarda la rappresentazione nel Portale Offerte e la comparabilità ufficiale, non esaurisce da sola la disciplina consumeristica di validità della promozione. Va inoltre coordinata con la deliberazione 386/2025/R/com quando la stessa promozione compare nelle condizioni economiche standardizzate del venditore.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRC-009, RULE-EE-PRC-010 e RULE-EE-PRC-013.

## Note
Questa regola chiude il residuo minimo sulle strutture promozionali domestiche senza trasformare ogni bonus o sconto in un elemento della `spesa annua stimata`.
