# EXTRACTED - SRC-SII-EE-PRESTAZIONI-TECNICHE-2025

## Metadata
- Source ID: SRC-SII-EE-PRESTAZIONI-TECNICHE-2025
- URL: https://siiportale.acquirenteunico.it/documents/11387888/11388872/Processo_di_richiesta_delle_Prestazioni+Tecniche_v3.2.pdf/9e71f89e-ac97-ad67-8870-654a74d528f5?t=1758640276477&download=true
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf) from SII PDF
- Relevance: alta per modellare gli stati attivo/disattivo del POD e le prevalenze tra DS, AV e pratiche commerciali

## Fatti chiave
1. Il documento pubblico SII "Processo di richiesta delle prestazioni tecniche" v3.2 disciplina i processi centralizzati di sospensione, riattivazione, attivazione, disattivazione e variazione potenza in attuazione delle deliberazioni 638/2022/R/eel e 135/2024/R/eel.
2. Il processo AV consente agli utenti del dispacciamento di richiedere tramite SII un'attivazione su punti di prelievo non attivi e contendibili.
3. Le prestazioni PA1 e PA2 riguardano l'energizzazione di un punto di consegna disattivo preposato, rispettivamente a parità di condizioni o con variazione di potenza.
4. Il SII verifica in ammissibilità che lo stato del punto sia coerente con la prestazione richiesta e che non esista un'altra richiesta di attivazione in corso.
5. La prestazione tecnica di attivazione è quella che cambia lo stato di energizzazione del POD da disattivo ad attivo; tale variazione avviene esclusivamente a seguito di esito positivo trasmesso dal distributore tramite AV2.0250 e decorre dalla data di esecuzione della prestazione.
6. Il processo DS centralizza le sole disattivazioni D01 su richiesta del cliente finale riferite a forniture permanenti; D02, D03 e le disattivazioni temporanee restano fuori dal processo centralizzato.
7. Lo stato di energizzazione del punto in RCU varia per disattivazione esclusivamente a seguito di esito positivo trasmesso dal distributore tramite DS2.0250; la decorrenza coincide con la data di esecuzione della prestazione.
8. A partire dal giorno precedente alla data minima di esecuzione di una DS, o dal giorno stesso se tale data non è valorizzata, non è più eseguibile alcuna prestazione che modifichi cliente finale, CC o UDD.
9. Se una DS arriva mentre esistono pratiche SW/VT/RC/UI già in corso, il SII applica regole di prevalenza che possono portare a esito negativo, annullamento o chiusura d'ufficio della DS o della pratica commerciale a seconda della decorrenza relativa.

## Citazioni utili
- p. 1: "PROCESSO DI RICHIESTA DELLE PRESTAZIONI TECNICHE"
- p. 1: "IN ATTUAZIONE DELLE DELIBERAZIONI 638/2022/R/EEL 135/2024/R/EEL"
- p. 30: "Il processo “Richiesta di attivazione” permette a ciascun Utente del Dispacciamento di richiedere tramite il SII l’esecuzione di una attivazione su punti di prelievo non attivi e contendibili"
- p. 32: "PA1: “Prestazione di Attivazione 1” riferita all’energizzazione di un punto di consegna disattivo preposato"
- p. 32: "lo stato del punto al momento della richiesta sia coerente con la prestazione richiesta"
- p. 45: "La prestazione che cambia lo stato di energizzazione del POD da disattivo ad attivo è la prestazione tecnica di attivazione"
- p. 45: "lo stato di energizzazione del punto in RCU varia esclusivamente a seguito di esito della prestazione stessa positivo trasmesso dal distributore al SII tramite il flusso AV2.0250"
- p. 35: "Il processo “Richiesta di disattivazione” permette a ciascuna Controparte Commerciale di richiedere tramite il SII l’esecuzione di una disattivazione sui punti di propria titolarità"
- p. 35: "esclusivamente le prestazioni di disattivazione su richiesta del cliente finale"
- p. 48: "lo stato di energizzazione del punto in RCU varia esclusivamente a seguito di esito della prestazione positivo trasmesso dal distributore al SII tramite il flusso DS2.0250"
- p. 48: "non sarà più eseguibile alcuna prestazione che modifichi il cliente finale, la CC o l’UDD"
- p. 49: "La richiesta di DS è ammissibile ed il giorno precedente la DATA_ESECUZIONE_MINIMA ... il Gestore del SII trasmette un esito negativo per la VT e gli annullamenti per SW e RC"

## Uso nel SSOT
- fonte quasi-ufficiale per modellare start/end supply states nel SII
- utile per distinguere attivazione/subentro da disattivazione su richiesta cliente
- base operativa per i conflitti fra DS e pratiche commerciali su punto attivo o in transizione
