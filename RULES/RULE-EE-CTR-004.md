# RULE-EE-CTR-004

## Metadata
- ID: RULE-EE-CTR-004
- Titolo: L'onere di recesso anticipato domestico è ammesso solo nel primo periodo a prezzo fisso predeterminato e decade se il venditore varia unilateralmente le condizioni
- Dominio: contratti-offerte-trasparenza
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-250-23-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/250-23.pdf
- Riferimento preciso: Articolo 2, comma 2.1, punto iv, nuovo articolo 6.6 della deliberazione 302/2016/R/com; motivazione, pagine 16-17 e 26
- Data pubblicazione: 2023-06-09
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti domestici elettrici l'onere di recesso anticipato può essere previsto solo per contratti a prezzo fisso e a tempo determinato, oppure per contratti a prezzo fisso e a tempo indeterminato ma con condizioni economiche a tempo determinato. Se l'offerta prevede un primo periodo a prezzo fisso e poi un passaggio a prezzo variabile, l'onere può essere richiesto solo con riferimento al primo periodo predeterminato a prezzo fisso. Restano esclusi i contratti a prezzo variabile e quelli che applicano nello stesso periodo un prezzo fisso e un prezzo variabile. Nei contratti a tempo indeterminato con condizioni economiche a tempo determinato l'onere può essere previsto solo fino alla prima scadenza delle condizioni economiche. Se il venditore esercita una variazione unilaterale delle condizioni, l'eventuale onere decade.

## Citazione
"può essere richiesto solamente con riferimento al primo periodo predeterminato in cui si applica il prezzo fisso"; "non rientrano in tale casistica"; "può essere previsto solo fino alla prima scadenza delle condizioni economiche"; "comporta la decadenza dell’eventuale applicazione di oneri di recesso anticipato"

## Interpretazione minima
La compliance ARERA non lascia un perimetro libero per applicare oneri di uscita a offerte variabili, ibride o rinnovate tacitamente oltre il primo periodo fixed. Nel SSOT l'onere ammesso va ancorato a un segmento contrattuale fixed-price con orizzonte predeterminato e con termine finale esplicito.

## Impatto operativo
I modelli contratto e offerta devono distinguere almeno tra `periodo_fixed_con_onere_ammissibile`, `offerta_variabile_o_mista_esclusa`, `scadenza_primo_periodo_fixed`, `decadenza_onere_per_variazione_unilaterale`. Non va mantenuto un flag generico `ha_onere_recesso` scollegato dal periodo contrattuale in cui l'onere può operare.

## Eccezioni e limiti
La regola riguarda il perimetro customer-facing domestico trattato nel presente slice. Non trasforma i rinnovi taciti o le condizioni economiche successive alla prima scadenza in nuovi segmenti automaticamente gravabili da onere. Si coordina con la disciplina PLACET, che nel repo resta trattata separatamente.

## Conflitti o dipendenze
Si coordina con RULE-EE-CTR-001, RULE-EE-CCC24-005 e RULE-EE-PRC-013.

## Note
La motivazione della deliberazione 250/2023/R/com adotta un'interpretazione restrittiva della deroga al recesso gratuito, in coerenza con la direttiva elettrica e con l'articolo 7 del d.lgs. 210/2021.