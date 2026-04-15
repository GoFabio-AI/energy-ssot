# RULE-EE-VOL-011

## Metadata
- ID: RULE-EE-VOL-011
- Titolo: Per i clienti BT la disattivazione su richiesta del cliente finale ha tempo massimo di 5 giorni lavorativi e include la chiusura contrattuale con lettura finale
- Dominio: voltura-subentro-cessazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-617-23
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/617-23allb.pdf
- Riferimento preciso: Allegato B, art. 16 e art. 22 Tabella 1, pp. 18-19 e 23
- Data pubblicazione: 2023-12-29
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per i clienti BT il tempo massimo di disattivazione della fornitura su richiesta del cliente finale è di 5 giorni lavorativi. Ai fini della rilevazione, la disattivazione comprende anche la semplice chiusura contrattuale con acquisizione della lettura finale che assicuri al cliente l'assenza di ulteriori addebiti di consumo.

## Citazione
"È inoltre assimilata alla disattivazione la semplice chiusura contrattuale, con acquisizione della lettura finale, che assicuri al cliente che non gli saranno addebitati ulteriori consumi"

## Interpretazione minima
La cessazione/disattivazione customer-requested può essere soddisfatta anche senza rimozione fisica del misuratore, purché il cliente sia protetto da ulteriori addebiti e venga registrata la lettura finale.

## Impatto operativo
Nel SSOT la cessazione ordinaria va mappata a una disattivazione regolata con SLA di 5 giorni lavorativi per il domestico BT.

## Eccezioni e limiti
La rilevazione non si applica alle richieste contestuali a riattivazioni per cambio titolarità senza intervento di disattivazione, come volture o subentri immediati, né ai passaggi tra venditori o tra libero e tutela.

## Conflitti o dipendenze
Da tenere distinto dal dominio switching e da RULE-EE-VOL-009 sul subentro.

## Note
Regola chiave per separare la fine fornitura chiesta dal cliente da voltura, subentro immediato e switching.
