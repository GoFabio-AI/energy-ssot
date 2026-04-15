# RULE-EE-POD-010

## Metadata
- ID: RULE-EE-POD-010
- Titolo: Nel SII i dati personali dei clienti finali sono usati solo per i processi del sistema e non per marketing o promozione
- Dominio: anagrafica-tecnica-pod-accessi-reporting
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-AU-SII-TRATTAMENTO-DATI-PERSONALI-PAGE
- URL fonte: https://siiportale.acquirenteunico.it/funzionamento-del-sii/trattamento-dati-personali-e-politica-di-sicurezza
- Riferimento preciso: pagina SII "Trattamento dati personali e Politica di Sicurezza"
- Data pubblicazione: n/d
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel Sistema Informativo Integrato i dati personali dei clienti finali scambiati tra Utenti e Gestore sono necessari e utilizzati esclusivamente ai fini dell'esecuzione dei processi del SII, secondo la regolazione ARERA e le regole e specifiche tecniche del Gestore. Sono esclusi usi, anche indiretti, per ricerche di mercato, promozione, pubblicità o vendita diretta. Il cliente finale può chiedere ad Acquirente Unico la verifica e l'eventuale correzione delle informazioni che lo riguardano.

## Citazione
"utilizzati esclusivamente ai fini dell'esecuzione dei Processi del SII"; "Sono esclusi trattamenti finalizzati, anche indirettamente, a ricerche di mercato e promozione, pubblicità o vendita diretta"; "la verifica delle informazioni che lo riguardano"

## Interpretazione minima
Il SII non è una base dati liberamente riusabile per finalità commerciali: l'uso dei dati è confinato ai processi regolati del sistema.

## Impatto operativo
Ogni modellazione SSOT o processo applicativo che richiami dati SII deve mantenere distinto il perimetro dei processi regolati dalle finalità commerciali o di marketing, e deve prevedere canali di verifica o correzione lato cliente quando il dato è trattato nel SII.

## Eccezioni e limiti
La regola chiarisce il perimetro di finalità e una garanzia minima di verifica/correzione, ma non sostituisce il quadro GDPR completo né definisce da sola tutti i tempi o canali di rettifica dei singoli processi SII.

## Conflitti o dipendenze
Si coordina con RULE-EE-RCU-001 e RULE-EE-RCU-003 sul ruolo del SII/RCU e con RULE-EE-POD-008 e RULE-EE-POD-009 sul lato cliente del Portale Consumi.

## Note
La pagina richiama espressamente anche il rispetto dell'Allegato A alla delibera ARG/com 201/10, oltre a GDPR e Codice privacy.