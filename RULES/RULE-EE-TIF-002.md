# RULE-EE-TIF-002

## Metadata
- ID: RULE-EE-TIF-002
- Titolo: In fatturazione il venditore deve usare prima dati effettivi, poi autoletture validate, poi stime
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIF-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/16/TIF_All_a_aggiornato_dal_1__luglio_2025__463-16_.pdf
- Riferimento preciso: Articolo 5, commi 5.1 e 5.2
- Data pubblicazione: 2025-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per contabilizzare i consumi nella bolletta di periodo, il venditore deve usare nell’ordine: dati di misura effettivi messi a disposizione dal distributore, autoletture validate e solo in ultima istanza dati di misura stimati. Se ricorre alla stima, può usare il dato stimato messo a disposizione dal distributore oppure effettuare una propria stima.

## Citazione
"il venditore è tenuto a utilizzare i dati di misura nel rispetto del seguente ordine: a) dati di misura effettivi ... b) autoletture ... validate ... c) dati di misura stimati"

## Interpretazione minima
La stima è subordinata all’indisponibilità di dato effettivo e autolettura validata, non una scelta equivalente alle altre due categorie.

## Impatto operativo
La logica di billing deve mantenere la gerarchia effettivo > autolettura validata > stimato e tracciarne la provenienza.

## Eccezioni e limiti
Per il servizio di tutela della vulnerabilità il comma 5.1bis contiene una disciplina aggiuntiva sui dati riferiti a data successiva all’ultimo giorno del mese oggetto di fatturazione.

## Conflitti o dipendenze
Dipende da RULE-EE-TIME-002 per capire quando l’autolettura diventa equivalente a dato effettivo e da RULE-EE-TIF-004 per i criteri della stima.

## Note
Questa regola vale anche per la lettura funzionale ai successivi ricalcoli.