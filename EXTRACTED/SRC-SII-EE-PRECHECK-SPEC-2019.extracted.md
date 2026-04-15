# EXTRACTED - SRC-SII-EE-PRECHECK-SPEC-2019

## Metadata
- Source ID: SRC-SII-EE-PRECHECK-SPEC-2019
- URL: https://siiportale.acquirenteunico.it/documents/11387888/11424977/Specifiche_tecniche_attuazione_delibera_82_2014_R_eel_v3.0.pdf/9ed666c3-dcc6-f140-6964-f4a35aa71bcd?t=1752250376944&download=true
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf)
- Relevance: alta per dettagliare il servizio PK di verifica abbinamento POD-cliente e l’integrazione anagrafica lato RCU

## Fatti chiave
1. Dopo la sottoscrizione di un contratto di vendita, il venditore può richiedere al SII la verifica dell’abbinamento tra il POD e il cliente finale.
2. Il processo PK verifica la corrispondenza tra POD e dati identificativi del cliente finale presenti nel RCU, con esito positivo anche in caso di scostamento non superiore a 2 caratteri alfanumerici su codice fiscale, partita IVA o, nei casi previsti, nome e cognome/ragione sociale.
3. In caso di esito positivo il SII restituisce almeno conferma dell’abbinamento, POD, dati identificativi del cliente presenti nel RCU e, nei casi previsti dalla specifica, ulteriori elementi operativi come PEC della controparte commerciale, eventuali CRPP, eventuale presenza di risoluzioni contrattuali e dato PMA del POD.
4. Per i POD attivi in maggior tutela senza codice fiscale o partita IVA associati, il venditore può integrare la richiesta con nome e cognome o ragione sociale del cliente finale.
5. Se il SII aggiorna il RCU con codice fiscale e/o partita IVA del cliente finale, trasmette entro un giorno lavorativo l’integrazione all’impresa distributrice tramite servizio PK2.

## Citazioni utili
- "il Venditore può richiedere la verifica dell’abbinamento tra il POD ed il Cliente Finale"
- "verificherà ... l’associazione tra POD/CF-PIVA"
- "non corretti per non più di 2 caratteri alfanumerici"
- "i dati identificativi del cliente finale titolare di tale punto presenti in RCU"
- "il dato di PMA (potenza media annua)"
- "inserendo il nome e cognome o la ragione sociale/denominazione del cliente finale titolare del punto di prelievo"
- "trasmette, entro un giorno lavorativo dalla richiesta di Pre-check, l’integrazione del codice fiscale e/o della partita IVA all’impresa di distribuzione"

## Uso nel SSOT
- fonte ufficiale di supporto per il dettaglio operativo del processo PK oltre la sola pagina processo SII
- utile per separare la consultazione tecnica CDT dalla verifica anagrafica POD-cliente e dalle integrazioni anagrafiche del RCU
- utile per modellare i campi minimi che il venditore può ricevere dal SII in fase precontrattuale o di verifica
