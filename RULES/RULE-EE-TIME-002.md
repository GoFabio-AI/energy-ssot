# RULE-EE-TIME-002

## Metadata
- ID: RULE-EE-TIME-002
- Titolo: L’autolettura validata equivale a un dato effettivo e si intende validata se manca esito entro tre giorni lavorativi
- Dominio: misure
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIME-2024-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/19/568-19time.pdf
- Riferimento preciso: Articolo 15, commi 15.1, 15.2, 15.3 e 15.4
- Data pubblicazione: 2019-12-17
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il responsabile della misura deve validare le autoletture comunicate dal cliente al venditore e comunicarne l’esito entro il terzo giorno lavorativo successivo alla ricezione. L’autolettura validata è equiparata a un dato di misura effettivo. Se l’esito non viene comunicato entro il termine, l’autolettura si intende comunque validata.

## Citazione
"comunicarne l’esito entro il terzo giorno lavorativo successivo"; "L’autolettura validata ... è equiparata a un dato di misura effettivo"; "l’autolettura si intende comunque validata"

## Interpretazione minima
La validazione tacita impedisce che il silenzio del responsabile della misura degradi il dato di autolettura a semplice informazione non utilizzabile.

## Impatto operativo
I flussi venditore-distributore devono avere timestamp certi di ricezione e un meccanismo di scadenza che trasformi in automatico il dato in autolettura validata se manca risposta entro il termine.

## Eccezioni e limiti
Il responsabile della misura non è tenuto a validare il dato comunicato dal venditore oltre il termine indicato dal TIF per l’autolettura in finestra.

## Conflitti o dipendenze
Dipende da RULE-EE-TIF-003 e RULE-EE-TIF-006 per il corretto conferimento dell’autolettura e alimenta RULE-EE-TIF-002 per la priorità d’uso in bolletta.

## Note
Lo scambio dei flussi deve avvenire con i canali e i formati previsti dalla regolazione e, comunque, almeno tramite PEC.
