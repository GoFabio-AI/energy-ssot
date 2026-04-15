# RULE-EE-TIQV-018

## Metadata
- ID: RULE-EE-TIQV-018
- Titolo: Entro il 28 febbraio il venditore deve comunicare ad ARERA i dati annuali su reclami, richieste, rettifiche e indennizzi
- Dominio: qualita-commerciale-reclami
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIQV-2026-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/16/TIQV_Allegato_A_in_vigore_dal_1_gennaio_2026.pdf
- Riferimento preciso: articoli 36.1, 36.2, 36.3, 36.4 e 36.5
- Data pubblicazione: 2026-01-01 (vigore indicato nel testo)
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Entro il 28 febbraio di ogni anno il venditore deve comunicare all'Autorità, per ciascuna tipologia di cliente e di fornitura, il numero totale di clienti finali alla fine di ciascun mese dell'anno precedente e i dati relativi all'anno precedente su reclami scritti, richieste di informazioni, rettifiche di fatturazione e di doppia fatturazione. La comunicazione comprende almeno volumi con e senza risposta motivata, casi con standard rispettato o non rispettato e relative cause, rettifiche eseguite con o senza rispetto del livello specifico, tempo effettivo medio di risposta o rettifica, pratiche ancora senza risposta o rettifica alla data di comunicazione, numero totale e ammontare complessivo degli indennizzi automatici corrisposti. ARERA può usare tali dati per monitoraggio, pubblicazione e controlli anche a campione.

## Citazione
"Entro il 28 febbraio di ogni anno il venditore è tenuto a comunicare all'Autorità" / "per ciascuna tipologia di cliente e per ciascuna tipologia di fornitura" / "il tempo effettivo medio di risposta o di rettifica" / "il numero totale degli indennizzi corrisposti" / "l'ammontare complessivo degli indennizzi corrisposti"

## Interpretazione minima
Il TIQV impone un reporting annuale strutturato end-to-end sul ciclo reclami e rettifiche, non un mero conteggio dei reclami ricevuti.

## Impatto operativo
Serve una data mart regolatoria che combini CRM, billing, SLA, cause di ritardo e contabilità degli indennizzi, con capacità di segmentazione per tipo cliente e tipo fornitura e con storicizzazione mensile.

## Eccezioni e limiti
La norma riguarda il perimetro di qualità commerciale TIQV. Ulteriori format, controlli o istruzioni operative ARERA possono dettagliare la trasmissione ma non sostituiscono il contenuto minimo già imposto dall'articolo 36.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIQV-016 sul registro dati di base e con RULE-EE-TIQV-019 sulla pubblicazione annuale verso il pubblico.

## Note
La comunicazione include anche i casi ancora aperti alla data del reporting, quindi il sistema deve distinguere tra anno di ricezione della pratica e stato alla data di invio ad ARERA.
