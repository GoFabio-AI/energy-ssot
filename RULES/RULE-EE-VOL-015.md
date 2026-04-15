# RULE-EE-VOL-015

## Metadata
- ID: RULE-EE-VOL-015
- Titolo: Nei processi SII lo stato del POD passa ad attivo o a disattivo solo dopo esito positivo del distributore e la disattivazione prevale sulle pratiche che cambiano titolarità quando prossima all’esecuzione
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-SII-EE-PRESTAZIONI-TECNICHE-2025
- URL fonte: https://siiportale.acquirenteunico.it/documents/11387888/11388872/Processo_di_richiesta_delle_Prestazioni+Tecniche_v3.2.pdf/9e71f89e-ac97-ad67-8870-654a74d528f5?t=1758640276477&download=true
- Riferimento preciso: Modelli AV e DS e prevalenze, pp. 30-32, 45 e 48-50
- Data pubblicazione: 2025-04-16
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel SII il passaggio dello stato di energizzazione del POD da disattivo ad attivo avviene solo dopo esito positivo del distributore nel processo AV; il passaggio a disattivo avviene solo dopo esito positivo del distributore nel processo DS. Quando una disattivazione è pendente e vicina alla data minima di esecuzione, non sono più eseguibili prestazioni che cambino cliente finale, controparte commerciale o UDD.

## Citazione
"lo stato di energizzazione del punto in RCU varia esclusivamente a seguito di esito della prestazione positivo trasmesso dal distributore al SII tramite il flusso DS2.0250"

## Interpretazione minima
Nel SSOT gli stati attivo/disattivo non vanno anticipati alla sola apertura pratica: servono esito positivo e data di esecuzione tecnica. Inoltre la fine fornitura chiesta dal cliente può bloccare o far decadere pratiche di voltura/switching/RC se temporalmente incompatibili.

## Impatto operativo
Regola utile per spiegare perché una pratica commerciale ancora aperta non garantisce il mantenimento dello stato attivo quando è già pendente una DS con esecuzione imminente.

## Eccezioni e limiti
Fonte quasi-ufficiale e tecnica; le prevalenze sono operative SII e vanno lette insieme alle fonti ARERA sul perimetro dei singoli processi.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-011 e con RULE-EE-SWI-003 sul confine con switching e risoluzione contrattuale senza disalimentazione.

## Note
Per la modellazione SSOT è utile distinguere tra apertura pratica, ammissibilità e variazione effettiva dello stato del POD.
