# RULE-EE-TIF-008

## Metadata
- ID: RULE-EE-TIF-008
- Titolo: Il venditore ricalcola importi basati su stime solo quando diventano disponibili dati di misura effettivi
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIF-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/16/TIF_All_a_aggiornato_dal_1__luglio_2025__463-16_.pdf
- Riferimento preciso: Articolo 6, comma 6.4
- Data pubblicazione: 2025-07-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Il venditore procede al ricalcolo di importi precedentemente determinati sulla base di dati di misura stimati solo quando si rendono disponibili dati di misura effettivi messi a disposizione dall’impresa di distribuzione, comprese le autoletture.

## Citazione
"il venditore procede al ricalcolo di importi precedentemente determinati sulla base di dati di misura stimati, solo in caso di successiva disponibilità di dati di misura effettivi messi a disposizione dall’impresa di distribuzione, comprese le autoletture"

## Interpretazione minima
Il ricalcolo di una bolletta fondata su stima non è libero o discrezionale: richiede il sopravvenire di un dato di misura effettivo che sostituisca la base stimata.

## Impatto operativo
Il motore di billing deve collegare ogni ricalcolo a uno specifico dato effettivo sopravvenuto, tracciandone provenienza, data di disponibilità e periodo di competenza.

## Eccezioni e limiti
La regola disciplina il trigger del ricalcolo di importi già stimati. Non sostituisce la disciplina della bolletta di chiusura né il termine di fatturazione dei conguagli da rettifica misura, che va coordinato con la deliberazione 97/2018/R/com.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIF-002, RULE-EE-TIF-004, RULE-EE-TIME-002, RULE-EE-BOLL-001 e RULE-EE-PRESC-001.

## Note
Questa regola chiude il passaggio tra stima iniziale e successivo conguaglio customer-facing nel pacchetto TIF/TIME.