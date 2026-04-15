# RULE-EE-POD-009

## Metadata
- ID: RULE-EE-POD-009
- Titolo: L'informativa privacy del Portale Consumi limita la conservazione dei dati personali a 36 mesi e riconosce accesso, portabilità e rettifica
- Dominio: anagrafica-tecnica-pod-accessi-reporting
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-AU-PORTALE-CONSUMI-PRIVACY-PAGE
- URL fonte: https://www.consumienergia.it/portaleConsumi/it/privacy.page
- Riferimento preciso: informativa privacy del Portale Consumi, sezioni su dati raccolti, conservazione e diritti dell'interessato
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per il Portale Consumi Acquirente Unico tratta dati identificativi del cliente, POD o PDR, indirizzi di ubicazione, misure dei consumi e tracciatura degli accessi. L'informativa dichiara che tali dati sono conservati solo per il tempo necessario alle finalità perseguite e comunque non oltre 36 mesi dalla data cui si riferiscono, e riconosce all'interessato almeno accesso, portabilità, rettifica e opposizione nei limiti di legge.

## Citazione
"codice fiscale, punto di prelievo (POD)"; "misure consumi"; "Tracciatura degli accessi effettuati sul Portale Consumi"; "non oltre i 36 mesi decorrenti dalla data cui si riferiscono"; "l’accesso ai dati personali"; "la copia dei dati personali forniti (c.d. portabilità)"; "la rettifica dei dati in nostro possesso"

## Interpretazione minima
Il repo dispone ora di un boundary ufficiale minimo sulla privacy del Portale Consumi, compresa la retention dichiarata e i diritti esercitabili dall'interessato.

## Impatto operativo
Se si modellano dati o funzionalità che replicano la vista del Portale Consumi, va considerato il limite di retention di 36 mesi dichiarato dal Portale e la necessità di distinguere i canali di rettifica tra Identity Provider e soggetti competenti sui dati energetici.

## Eccezioni e limiti
Questa regola riguarda l'informativa privacy del Portale Consumi e non può essere estesa automaticamente alla conservazione delle bollette, ai sistemi dei venditori o alla disponibilità post-cessazione dei documenti contrattuali.

## Conflitti o dipendenze
Si coordina con RULE-EE-POD-003 e RULE-EE-POD-008 sul perimetro dati disponibile al cliente e con RULE-EE-POD-010 sul diverso perimetro privacy del SII.

## Note
L'informativa precisa anche che per nome e cognome la rettifica va chiesta all'Identity Provider usato per l'accesso al Portale.