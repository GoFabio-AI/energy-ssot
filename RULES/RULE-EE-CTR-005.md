# RULE-EE-CTR-005

## Metadata
- ID: RULE-EE-CTR-005
- Titolo: L'onere di recesso anticipato va comunicato come massimale ex ante ma applicato solo entro la perdita economica diretta effettiva
- Dominio: contratti-offerte-trasparenza
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-250-23-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/250-23.pdf
- Riferimento preciso: Articolo 1, comma 1.1, lettere fter, iv e articolo 21bis.1; motivazione, pagine 14, 17, 20-25
- Data pubblicazione: 2023-06-09
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Quando l'onere di recesso anticipato è ammesso, il venditore deve indicarlo in modo chiaro, espresso e agevolmente comprensibile già in fase precontrattuale, nel contratto e nel riquadro `Modalità e oneri di recesso` della Scheda sintetica come somma massima di denaro complessivamente dovuta, eventualmente differenziata in base ai mesi o giorni residui. Il venditore può aggiungere i criteri di determinazione dell'importo, ma deve evidenziare che il valore indicato è un massimale. Al momento dell'applicazione, l'importo richiesto deve essere adeguato all'effettiva perdita economica diretta se questa risulta inferiore al massimale comunicato.

## Citazione
"somma massima di denaro complessivamente dovuta"; "eventualmente differenziata ed esplicitata sulla base del numero di mesi o giorni"; "potrebbe essere ridotto in ragione della perdita economica diretta"; "adeguare la somma di denaro richiesta all’effettiva perdita economica diretta"

## Interpretazione minima
Nel SSOT il numero mostrato ex ante non è una penale fissa automaticamente dovuta. È un tetto massimo comunicato al cliente, che deve sempre essere ri-ancorato al danno diretto effettivo del fornitore nel momento in cui il recesso produce effetti.

## Impatto operativo
I sistemi devono tenere distinti almeno `massimale_ex_ante_onere_recesso`, `griglia_tempo_residuo`, `criteri_calcolo_aggiuntivi`, `importo_effettivo_post_ricalcolo`, `perdita_economica_diretta_provata`. Non è conforme trattare l'importo precontrattuale come addebito automatico non ricalcolabile.

## Eccezioni e limiti
La regola non impone un algoritmo ARERA uniforme di calcolo del massimale e non elimina l'onere della prova della perdita economica diretta già previsto dalla norma primaria. Resta applicabile solo nel perimetro contrattuale in cui l'onere è ammesso.

## Conflitti o dipendenze
Si coordina con RULE-EE-CTR-001, RULE-EE-CCC24-005 e RULE-EE-CDCONS-001.

## Note
Questa regola chiude il residuo sul metodo di quantificazione: ARERA non standardizza la formula commerciale del venditore, ma standardizza il formato informativo minimo e il vincolo di ricalcolo verso il danno diretto effettivo.