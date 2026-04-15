# RULE-EE-TIMOE-007

## Metadata
- ID: RULE-EE-TIMOE-007
- Titolo: I clienti non disalimentabili hanno elenco dedicato e, se morosi nel mercato libero, seguono la via della risoluzione contrattuale e dell'ultima istanza
- Dominio: morosita-cmor
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIMOE-2024-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/15/258-15TIMOE_new.pdf
- Riferimento preciso: Articolo 23, commi 23.1-23.4; Articolo 24, commi 24.1-24.5
- Data pubblicazione: 2024-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il TIMOE individua come non disalimentabili solo i clienti rientranti nelle categorie tassative dell'articolo 23 e impone al distributore di mantenere un elenco aggiornato con POD e codice fiscale o partita IVA. Il cliente può rinunciare per iscritto alla qualifica e l'utente del trasporto deve inoltrare al distributore, entro il giorno lavorativo successivo, l'eventuale richiesta del cliente di essere inserito nell'elenco. Se un cliente finale non disalimentabile servito nel mercato libero è moroso, l'utente del trasporto non segue la sospensione ordinaria del punto ma può risolvere i contratti di dispacciamento e di trasporto; il distributore trasferisce quindi il punto nel contratto di dispacciamento del servizio di ultima istanza previsto dal TIMOE e ne attiva il relativo servizio secondo le tempistiche ordinarie delle variazioni dell'utente del dispacciamento.

## Citazione
"I clienti non disalimentabili sono i clienti che appartengono ad una delle seguenti categorie"; "entro il giorno lavorativo successivo al suo ricevimento"; "In caso di morosità dei clienti finali non disalimentabili serviti sul mercato libero, l’utente del trasporto può risolvere i relativi contratti di dispacciamento e di trasporto"; "L’attivazione dei servizi di ultima istanza di cui al comma 24.3 avviene secondo le medesime tempistiche previste per le altre variazioni dell’utente del dispacciamento"

## Interpretazione minima
Per i non disalimentabili la morosità non sfocia nella normale sequenza riduzione-sospensione del Titolo II, ma in un percorso speciale di risoluzione contrattuale con continuità della fornitura tramite servizio di ultima istanza.

## Impatto operativo
Anagrafiche, processi collection e motori di orchestrazione SII devono distinguere i punti non disalimentabili prima di avviare la morosità ordinaria, tracciare eventuali richieste di inserimento o rinuncia e attivare il percorso di risoluzione contrattuale invece della sospensione fisica.

## Eccezioni e limiti
Il comma 24.3 del TIMOE instrada i punti verso Acquirente Unico per gli aventi diritto alla maggior tutela e verso salvaguardia per gli aventi diritto alla salvaguardia. Per il mapping domestico vigente al 2026-04-15 il TIV 2026 chiarisce però espressamente che i clienti di cui al comma 47.2 entrano nello STG e disciplina anche i casi di attivazione ai sensi del Titolo III del TIMOE agli articoli 48.14 e 50.1. Resta quindi solo un disallineamento redazionale del TIMOE consolidato, non un dubbio sostanziale di routing.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIMOE-001 e RULE-EE-TIMOE-005, che disciplinano le procedure ordinarie per i clienti disalimentabili, con RULE-EE-SWI-002 per la cornice SII di risoluzione contrattuale e con RULE-EE-TIV-007 per l'aggancio customer-facing ai servizi di ultima istanza domestici vigenti.

## Note
Nel perimetro domestico il caso più chiaramente tracciabile in articolo 23 è quello dei clienti con compensazione TIBEG non identificati come interrompibili; altre categorie dell'articolo 23 sono meno tipiche del domestico puro.
