# RULE-EE-VOL-005

## Metadata
- ID: RULE-EE-VOL-005
- Titolo: Nella voltura con cambio fornitore l'utente del dispacciamento può usare il servizio informativo IV per valutare il POD prima della richiesta
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-135-21
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/21/135-21.pdf
- Riferimento preciso: articolo 2 e articolo 3; pagg. 14-15
- Data pubblicazione: 2021-03-30
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il SII rende disponibile agli utenti del dispacciamento il servizio informativo per attivazione contrattuale per la voltura con cambio fornitore. In caso di esito positivo il servizio restituisce almeno stato del punto, CRPP, PMA, mercato di provenienza distinguendo tra mercato libero e servizi di ultima istanza, e date di switching, volture e volture con cambio fornitore finalizzate negli ultimi 12 mesi. L'accesso richiede POD, disponibilità della documentazione della richiesta di voltura, codice fiscale del cliente finale e data presunta di decorrenza.

## Citazione
"servizio informativo per attivazione contrattuale"; "mercato di provenienza del punto, distinguendo tra mercato libero e servizi di ultima istanza"; "date delle richieste di switching finalizzate, eseguite negli ultimi 12 mesi"

## Interpretazione minima
La voltura con cambio fornitore non è un blind transfer. Il nuovo UdD ha un pre-check informativo esplicito per valutare il rischio operativo e commerciale del POD.

## Impatto operativo
Nei sistemi e nelle procedure di onboarding voltura con cambio fornitore va modellato il passaggio IV prima della richiesta VT quando si vuole valutare provenienza da ultima istanza, churn recente, PMA o altre criticità del punto.

## Eccezioni e limiti
Il servizio è uno strumento informativo pre-richiesta, non sostituisce i controlli documentali sulla disponibilità dell'immobile né la decisione commerciale del venditore.

## Conflitti o dipendenze
Si coordina con RULE-EE-VOL-002, RULE-EE-VOL-006 e con SRC-SII-EE-VOLTURA-SPEC-2025.

## Note
Regola chiave per superare il solo modello base VT del pacchetto SII.
