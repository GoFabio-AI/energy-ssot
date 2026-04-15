# EXTRACTED - SRC-SII-EE-AOC-RCU-2025

## Metadata
- Source ID: SRC-SII-EE-AOC-RCU-2025
- URL: https://siiportale.acquirenteunico.it/documents/11387888/11388872/Specifiche+Tecniche_AggiornamentoOnConditionRCU_EE_v4.4.pdf/d3fd86b5-e3de-6c04-720a-0bd5337be6f7?t=1752239133288&download=true
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf) from SII PDF
- Relevance: alta per stati POD nel RCU e integrazione dei dati dopo attivazioni/subentri/disattivazioni

## Fatti chiave
1. Il documento pubblico SII "Specifiche Tecniche Aggiornamento On Condition RCU" v4.4 disciplina il processo VS di variazione stato POD e i processi AE/MO di aggiornamento dati RCU.
2. Il processo VS serve al distributore per comunicare al SII gli esiti positivi delle nuove connessioni, delle attivazioni e delle disattivazioni.
3. Le attivazioni comprendono i subentri, trattati come richieste di attivazione con contestuale variazione dei soli dati identificativi del cliente finale su un punto disattivato.
4. Il distributore comunica tali esiti entro 2 giorni lavorativi dall'esecuzione della prestazione tramite il servizio VS1.
5. Per ciascun punto per cui è stata eseguita nuova connessione, attivazione o disattivazione, la comunicazione deve includere almeno POD, identificativi cliente, UDD/EMT richiedente, prestazione eseguita e data di esecuzione.
6. Verificata l'ammissibilità dei flussi VS1, il SII aggiorna il RCU entro 1 giorno lavorativo e notifica alla controparte commerciale la nuova attivazione tramite VS2.0200.
7. Entro 3 giorni dalla notifica di attivazione del POD, ciascun UDD aggiorna tramite VS2.0201 i dati costituenti il RCU di propria competenza definiti nell'Allegato A alla deliberazione 628/2015/R/eel.
8. In caso di assenza di abbinamento POD-venditore, l'UDD opera come CC sul punto fino al successivo abbinamento; se i dati non vengono inviati tramite VS2, la CC abbinata al punto è tenuta a trasmetterli tramite AE1.0050.

## Citazioni utili
- p. 1: "SPECIFICHE TECNICHE AGGIORNAMENTO ON CONDITION RCU"
- p. 1: "DI ATTUAZIONE DELLA DELIBERAZIONE 628/2015/R/EEL"
- p. 17: "VS – Variazione stato POD: mediante il quale il Distributore comunica al SII gli esiti positivi delle nuove connessioni, le attivazioni e le disattivazioni"
- p. 17: "attivazione (comprensive dei subentri, in quanto trattati dal TIQE alla stregua di una richiesta di attivazione con contestuale variazione dei soli dati identificativi del cliente finale, di un punto disattivato)"
- p. 17: "entro 2 giorni lavorativi dall’esecuzione delle medesime"
- p. 18: "VS1 - Comunicazione Variazione Stato POD"
- p. 18: "VS2 - Notifica Attivazione POD"
- p. 18: "per ciascun punto di prelievo per il quale è stata eseguita una richiesta di nuova connessione, attivazione o disattivazione della fornitura"
- p. 19: "entro 1 giorno lavorativo, aggiorna il RCU e notifica alla controparte commerciale la nuova attivazione"
- p. 19: "Entro 3 giorni dalla notifica di attivazione del POD, ciascun UDD è tenuto ad aggiornare i dati costituenti il RCU di propria competenza"
- p. 19: "In caso di assenza di abbinamento POD-Venditore, l’Utente del Dispacciamento, in qualità di CC sul punto fino al successivo abbinamento, effettua la trasmissione dei dati"
- p. 19: "Nel caso in cui i dati non vengano inviati tramite il flusso VS2 la CC abbinata al punto è tenuta a inviare gli stessi tramite il flusso AE1.0050"

## Uso nel SSOT
- base quasi-ufficiale per gli stati di inizio/fine fornitura registrati nel RCU
- utile per raccordare subentro, attivazione e disattivazione con i flussi VS/VS2/AE1
- chiarisce i tempi di popolamento del RCU dopo l'esecuzione tecnica della prestazione
- chiude anche il passaggio post-attivazione tra notifica VS2.0200, integrazione UDD via VS2.0201 e fallback AE1.0050 della CC abbinata
