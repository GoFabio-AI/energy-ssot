# RULE-EE-TIMOE-008

## Metadata
- ID: RULE-EE-TIMOE-008
- Titolo: Il coordinamento TIMOE/TIV per i clienti domestici non vulnerabili non disalimentabili è sostanzialmente chiuso dal TIV 2026, con solo residuo redazionale del TIMOE 24.3
- Dominio: morosita-cmor
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIV-2026-PDF, SRC-ARERA-TIMOE-2024-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/Allegato_A_TIV_valido__dal_1_gennaio_2026.pdf, https://www.arera.it/fileadmin/allegati/docs/15/258-15TIMOE_new.pdf
- Riferimento preciso: TIV articoli 4.4, 47.2, 48.14, 50.1; TIMOE articolo 24.3
- Data pubblicazione: 2026-01-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il TIMOE articolo 24.3 cita testualmente l'instradamento dei clienti non disalimentabili verso Acquirente Unico o salvaguardia. Tuttavia, il TIV 2026 è fonte successiva e speciale per il domestico elettrico e prevede espressamente: all'articolo 4.4, che i clienti domestici non vulnerabili senza venditore sul mercato libero sono inseriti nel contratto di dispacciamento dell'esercente STG; all'articolo 48.14, che l'esercente STG domestico fornisce alle condizioni STG anche i clienti attivati ai sensi del Titolo III del TIMOE (cioè i non disalimentabili risolti nel libero); all'articolo 50.1, che l'esercente STG applica ai clienti di cui all'articolo 48.14 gli stessi corrispettivi e le stesse modalità degli altri clienti STG. Il routing dei non disalimentabili domestici non vulnerabili verso STG è quindi sostanzialmente chiuso dal TIV 2026 e il TIMOE 24.3 va letto come residuo redazionale non ancora allineato.

## Citazione
TIV 2026, art. 4.4: "per i clienti di cui al comma 47.2, nel contratto di dispacciamento dell'esercente le tutele graduali per i clienti domestici non vulnerabili"; TIV 2026, art. 48.14: "L'esercente il servizio a tutele graduali per i clienti domestici non vulnerabili fornisce il servizio ... ai clienti finali attivati ai sensi del Titolo III del TIMOE"; TIV 2026, art. 50.1: "applica i medesimi corrispettivi e le medesime modalità"; TIMOE art. 24.3: "per gli aventi diritto alla maggior tutela, nel contratto di dispacciamento dell'Acquirente unico ... per gli aventi diritto alla salvaguardia, nel contratto di dispacciamento dell'esercente la salvaguardia"

## Interpretazione minima
Per il SSOT, il routing dei clienti domestici non vulnerabili non disalimentabili è chiuso: vanno nello STG. Il testo del TIMOE 24.3 è residuo redazionale che non modifica il comportamento atteso.

## Impatto operativo
Motori di orchestrazione e customer care devono instradare i domestici non vulnerabili non disalimentabili verso STG secondo TIV 2026, non verso Acquirente Unico o salvaguardia secondo la lettera non aggiornata del TIMOE 24.3.

## Eccezioni e limiti
I clienti domestici vulnerabili non disalimentabili seguono comunque la maggior tutela secondo TIV articoli 4.4 e 8.2. Questa regola riguarda solo i domestici non vulnerabili.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIMOE-007, RULE-EE-TIV-007 e RULE-EE-STG-003.

## Note
Al 2026-04-15 non risulta un TIMOE consolidato che allinei testualmente il comma 24.3 al routing STG; la chiusura è sostanziale, non formale.
