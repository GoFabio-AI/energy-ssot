# RULE-EE-BOL-002

## Metadata
- ID: RULE-EE-BOL-002
- Titolo: Il Frontespizio unificato coincide con la prima facciata e contiene tutti e solo gli elementi previsti
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: Allegato A, articolo 5, comma 5.1
- Data pubblicazione: 2024-07-23
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il `Frontespizio unificato` corrisponde alla prima facciata della bolletta e deve riportare tutti e solo gli elementi previsti dalla disciplina ARERA.

## Citazione
"Il Frontespizio unificato corrisponde alla prima facciata della bolletta; i venditori sono tenuti a riportare nel Frontespizio unificato tutti e solo gli elementi"

## Interpretazione minima
La prima pagina ha un contenuto regolato e non può essere usata per spostare o aggiungere arbitrariamente informazioni fuori dal perimetro consentito, salvo lo spazio informativo espressamente ammesso dalla disciplina.

## Impatto operativo
Nel SSOT il `Frontespizio` va modellato come sezione distinta e rigidamente delimitata. In UI e OCR non vanno mischiati nel Frontespizio contenuti dello Scontrino, del Box o degli Elementi informativi essenziali.

## Eccezioni e limiti
La regola non elenca qui tutti gli elementi del Frontespizio, che sono disciplinati dal comma 5.2.

## Conflitti o dipendenze
Dipende da RULE-EE-BOL-001. Si coordina con SRC-ARERA-204-2025-R-COM-ALLEGATO-A, che riprende la stessa definizione in forma glossariale.

## Note
Nel Glossario elettrico il Frontespizio è presentato come prima facciata universale della bolletta.
