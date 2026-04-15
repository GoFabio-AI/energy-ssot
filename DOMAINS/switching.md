# Dominio: Switching

## Perimetro attivo
- settore: energia elettrica
- segmento: clienti domestici
- esclusioni temporanee: gas, business/non-domestico

## Scopo
Raccogliere il quadro regolatorio e operativo ufficiale per il cambio fornitore nel settore elettrico domestico, includendo i casi di risoluzione contrattuale senza disalimentazione e le transizioni ai servizi di ultima istanza.

## Copre
- switching su POD attivo
- distinzione tra switching e voltura
- distinzione tra switching e disattivazione/cessazione su richiesta cliente
- processi SE, RC e UI nel SII
- stato della riforma switching a 24 ore al 2026-04-15

## Fonti principali
### Regolatorie primarie
- SRC-NORMATTIVA-DL-105-2010-ART1BIS
- SRC-NORMATTIVA-DL-47-2014-ART5
- SRC-ARERA-487-15
- SRC-ARERA-58-26

### Operative ufficiali di supporto
- SRC-SII-EE-SWITCHING-PAGE
- SRC-SII-EE-SWITCHING-SPEC-2025
- SRC-AU-SII-SISTEMA-INFORMATIVO
- SRC-SII-EE-PRESTAZIONI-TECNICHE-2025

## Fatti regolatori primari
- L'articolo 1-bis del d.l. 105/2010 istituisce il SII presso Acquirente Unico e fonda la gestione centralizzata dei flussi e della banca dati dei punti/clienti.
- La deliberazione 487/2015/R/eel approva nel perimetro SII sia l'esecuzione del nuovo contratto su punto di prelievo attivo sia la risoluzione contrattuale senza disalimentazione con conseguente attivazione dei servizi di ultima istanza.
- L'articolo 5 del d.l. 47/2014 impone il titolo di disponibilità dell'immobile per voltura/stipulazione/rinnovo, ma esclude le ipotesi di successione di un fornitore del servizio a un altro. Questo è il discrimine normativo più netto tra voltura e switching.
- La deliberazione 58/2026/R/eel approva la riforma dello switching reseller con procedura tecnica a 24 ore, ma ne fissa l'applicazione dal 1 dicembre 2026 e l'abrogazione dell'Allegato A della 487/2015 solo dal 30 novembre 2026. Al 2026-04-15 il regime vigente resta quindi quello 487/2015.

## Fatti operativi di supporto
- Il portale SII definisce lo switching come successione senza soluzione di continuità di un Utente del Dispacciamento a un altro sullo stesso POD attivo.
- Il portale SII colloca lo switching sui punti censiti nel Registro Centrale Ufficiale e pubblica come processi principali SE, RC e UI.
- La specifica tecnica pubblica v3.1 del 31 ottobre 2025 copre variazione controparte commerciale, switching e risoluzione contrattuale in attuazione della deliberazione 487/2015/R/eel.
- La specifica SII sulle prestazioni tecniche 2025 chiarisce che la DS è una prestazione distinta, riferita alla disattivazione su richiesta del cliente finale, e che le pratiche di switching/voltura/RC possono essere annullate o chiuse d'ufficio se incompatibili con una disattivazione imminente.
- La riforma 58/2026 introduce per il futuro un preliminary check e, in prima fase, un'esecuzione in 1 giorno lavorativo solo per clienti domestici con punto non sospeso e senza Cmor attivo. Queste regole non vanno anticipate nei flussi al 2026-04-15.

## Edge cases operativi consolidati
- Se il caso riguarda solo la successione tra fornitori su POD attivo, non va richiesto il titolo di disponibilità dell'immobile ai sensi dell'articolo 5 del d.l. 47/2014.
- Se il contratto sul punto attivo si scioglie senza disalimentazione, il caso resta nel dominio switching tramite RC/UI e non va degradato automaticamente a cessazione o subentro.
- Se il cliente chiede la fine della fornitura con passaggio dello stato POD a disattivo, il caso esce dal dominio switching ed entra nel dominio voltura-subentro-cessazione tramite DS/cessazione.
- Le regole dello switching a 24 ore sono, al 2026-04-15, roadmap regolatoria approvata ma non ancora efficace.

## Evidenze estratte
- `EXTRACTED/SRC-NORMATTIVA-DL-105-2010-ART1BIS.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DL-47-2014-ART5.extracted.md`
- `EXTRACTED/SRC-ARERA-487-15.extracted.md`
- `EXTRACTED/SRC-ARERA-58-26.extracted.md`
- `EXTRACTED/SRC-SII-EE-SWITCHING-PAGE.extracted.md`
- `EXTRACTED/SRC-SII-EE-SWITCHING-SPEC-2025.extracted.md`
- `EXTRACTED/SRC-AU-SII-SISTEMA-INFORMATIVO.extracted.md`
- `EXTRACTED/SRC-SII-EE-PRESTAZIONI-TECNICHE-2025.extracted.md`

## Regole collegate
- RULE-EE-SII-001
- RULE-EE-RCU-001
- RULE-EE-SWI-001
- RULE-EE-SWI-002
- RULE-EE-SWI-003
- RULE-EE-SWI-004
- RULE-EE-VOL-011
- RULE-EE-VOL-015

## Open questions
- Nessuna open question SSOT attiva sul baseline switching vigente al 2026-04-15.
- Restano solo follow-up di monitoraggio futuro: acquisire, quando pubblicate da AU, le specifiche tecniche attuative post-deliberazione 58/2026 per il nuovo switching reseller dal 1 dicembre 2026 e verificare in un passaggio separato il coordinamento finale tra riforma 58/2026, pre-check/preliminary check e TIMOE lato morosità/Cmor.

## Stato avanzamento
- Coperti: switching su POD attivo, distinzione rispetto a voltura e disattivazione, perimetro SII su `SE/RC/UI`, non applicabilità anticipata della riforma reseller a 24 ore e boundary tra switching puro e casi che escono verso cessazione o attivazione.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15. Restano solo monitoraggio evolutivo della riforma 58/2026 e futuri atti tecnici AU/SII.
