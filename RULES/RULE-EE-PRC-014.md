# RULE-EE-PRC-014

## Metadata
- ID: RULE-EE-PRC-014
- Titolo: Nel Portale Offerte l'onere di recesso anticipato è un'informazione di presenza e non una componente della spesa annua stimata
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-250-23-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/250-23.pdf
- Riferimento preciso: motivazione, pagina 14; articolo 3, comma 3.1, punti i-iii, pagine 26-27
- Data pubblicazione: 2023-06-09
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel Portale Offerte l'eventuale onere di recesso anticipato delle offerte elettriche è rappresentato come informazione di presenza nell'elenco delle offerte, nei filtri di ricerca e nella pagina di dettaglio. L'onere non entra però nel computo della `spesa annua stimata`, perché dipende dal verificarsi del recesso anticipato e non è preventivabile come componente ordinaria del costo annuo della fornitura.

## Citazione
"assenza ... degli oneri di recesso anticipato dal computo della stima della spesa annua"; "l’indicazione della presenza dell’eventuale onere di recesso anticipato"; "la presenza dell’eventuale onere di recesso anticipato"

## Interpretazione minima
Nel SSOT il costo di uscita eventuale non va sommato alla metrica comparativa ufficiale del Portale. Deve invece essere modellato come metadato di rischio/condizione contrattuale separato dalla stima annua di spesa.

## Impatto operativo
I modelli pricing e comparazione devono tenere separati `spesa_annua_stimata_portale` e `presenza_onere_recesso_anticipato`. Non è conforme inquinare il ranking o il calcolo della convenienza annua standard con un onere eventuale e condizionato.

## Eccezioni e limiti
La regola riguarda il Portale Offerte e la comparabilità standard, non la validità sostanziale dell'onere, che resta subordinata al d.lgs. 210/2021 e alla disciplina ARERA di dettaglio. Non esclude che il dettaglio dell'offerta esponga il massimale o altre informazioni descrittive ulteriori.

## Conflitti o dipendenze
Si coordina con RULE-EE-CTR-002, RULE-EE-PRC-012 e RULE-EE-CTR-005.

## Note
Questa regola chiude il residuo customer-facing tra comparabilità economica e disclosure contrattuale: l'onere di recesso anticipato è visibile nel Portale, ma resta fuori dal prezzo annuo comparato.