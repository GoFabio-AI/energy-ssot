# RULE-EE-PLACET-002

## Metadata
- ID: RULE-EE-PLACET-002
- Titolo: Nelle offerte PLACET domestiche il deposito è addebitato in prima fattura utile, si ricostituisce se usato e va restituito con interesse legale
- Dominio: pagamenti-garanzie-rateizzazioni
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-PLACET-2017-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/17/555-17_Allegato_A.pdf
- Riferimento preciso: Articolo 9, commi 9.3, 9.4 e 9.5
- Data pubblicazione: 2017
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nelle offerte PLACET elettriche il deposito cauzionale è addebitato al cliente nella prima fattura utile e, per i punti domestici di cui al TIV articolo 2.3, lettera a), è pari a 11,5 euro per ogni kW di potenza contrattualmente impegnata. Se il venditore usa il deposito, in tutto o in parte, per coprire insoluti, il cliente deve ricostituirlo con addebito sulla prima fattura utile. Il deposito deve essere restituito al cliente con il tasso di interesse legale, senza richiedere prova del versamento.

## Citazione
"nella prima fattura utile"; "11,5 euro per ogni kW di potenza contrattualmente impegnata"; "il cliente è tenuto a ricostituirlo con addebito sulla prima fattura utile"; "Il deposito cauzionale è restituito al cliente maggiorato in base al tasso di interesse legale"

## Interpretazione minima
Il deposito PLACET ha un ciclo di vita rigidamente regolato: prima fattura utile, eventuale ricostituzione se assorbito da insoluti e restituzione finale con interesse legale.

## Impatto operativo
I sistemi di billing PLACET devono tracciare addebito iniziale, utilizzi compensativi su insoluti, ricostituzione automatica e rimborso con interesse legale in chiusura del rapporto.

## Eccezioni e limiti
Nel presente slice è atomizzato solo il valore domestico di 11,5 euro/kW; il resto della casistica articolo 9.3 resta esterno se non domestico.

## Conflitti o dipendenze
Si coordina con RULE-EE-PLACET-001, con RULE-EE-TIF-005 per la restituzione del deposito nella bolletta provvisoria di chiusura e con RULE-EE-STG-004 per l'applicazione nello STG via rinvio TIV.

## Note
La disciplina PLACET collega gli eventuali raddoppi del deposito alle condizioni del TIV, ma quel dettaglio non è ri-atomizzato qui oltre il perimetro domestico necessario.
