# RULE-EE-PRC-008

## Metadata
- ID: RULE-EE-PRC-008
- Titolo: Nel libero domestico elettrico restano vendor-specific i valori e le articolazioni dei corrispettivi di vendita, entro i vincoli strutturali ARERA
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-386-2025-R-COM-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/25/386-2025-R-com.pdf
- Riferimento preciso: Articolo 1, commi 1.2 e 1.3
- Data pubblicazione: 2025-08-05
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nelle offerte domestiche elettriche del mercato libero, i corrispettivi di vendita restano definiti dal venditore entro la struttura ARERA. In particolare, il venditore determina il valore della quota annua e della quota consumo; può differenziarle in funzione di potenza impegnata, fasce orarie, scaglioni di consumo, raggruppamenti di giorni dell’anno o altre caratteristiche specifiche del cliente. Se l’offerta è a prezzo variabile, la quota consumo è pari a uno o più indici di riferimento identificati dal venditore più un eventuale unico corrispettivo aggiuntivo. Se l’offerta è a prezzo fisso, la quota consumo è nota e invariabile per il periodo indicato. Le strutture miste sono ammesse.

## Citazione
"È facoltà del venditore differenziare"; "in funzione di fasce orarie, scaglioni di consumo"; "uno o più indici di riferimento identificati dal venditore"; "un unico eventuale corrispettivo aggiuntivo"; "è noto e invariabile per il periodo di tempo indicato nell’offerta"

## Interpretazione minima
Il perimetro SSOT uniforme finisce alla struttura e alla disclosure minima. I valori numerici, i marker di indicizzazione, i moltiplicatori contrattuali e le articolazioni commerciali restano vendor-specific e vanno memorizzati come dati dell’offerta, non come costanti regolatorie di sistema.

## Impatto operativo
Non va costruita una formula canonica che assuma un unico spread, un unico indice o un unico set di fasce per tutte le offerte del mercato libero domestico. Le pipeline devono modellare esplicitamente indici, adder, articolazioni e condizioni applicative dell’offerta specifica.

## Eccezioni e limiti
La regola non riguarda i corrispettivi rete e oneri generali di sistema, che seguono fonti regolatorie distinte, né il dispacciamento/capacità separato disciplinato dal comma 1.2, lettera b).

## Conflitti o dipendenze
Dipende da RULE-EE-PRC-007 e si coordina con RULE-EE-PRC-009 e RULE-EE-PRC-010.

## Note
La possibilità di differenziazione vendor-specific non supera gli obblighi di chiarezza, comparabilità e disclosure previsti dal Codice di condotta commerciale e dal Portale Offerte.