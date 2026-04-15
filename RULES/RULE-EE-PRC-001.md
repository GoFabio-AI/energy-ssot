# RULE-EE-PRC-001

## Metadata
- ID: RULE-EE-PRC-001
- Titolo: La bolletta elettrica customer-facing vigente aggrega gli importi in vendita, rete e oneri generali di sistema
- Dominio: prezzi-oneri-componenti
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-BOLLETTA-2025-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Riferimento preciso: Allegato A, Tabella 1 e disposizioni valide dall’1 luglio 2025
- Data pubblicazione: 2024-07-23
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel customer-facing della bolletta elettrica vigente, gli importi fatturati sono aggregati almeno nelle voci `Spesa per la vendita di energia elettrica`, `Spesa per la tariffa per l’uso della rete elettrica` e `Spesa per gli oneri generali di sistema`, con imposte esposte separatamente.

## Citazione
"Spesa per la vendita di energia elettrica"; "Spesa per la tariffa per l’uso della rete elettrica"; "Spesa per gli oneri generali di sistema"

## Interpretazione minima
Questa è la tassonomia customer-facing primaria da preferire nel SSOT per il domestico elettrico al 2026-04-15.

## Impatto operativo
Le viste SSOT, i parser bolletta e i modelli di decomposizione devono partire da questi bucket, non da etichette legacy non più primarie.

## Eccezioni e limiti
La regola non chiude da sola il dettaglio delle imposte né dei corrispettivi contrattuali del mercato libero.

## Conflitti o dipendenze
Dipende da RULE-EE-PRC-002, RULE-EE-PRC-003 e RULE-EE-PRC-004 per il dettaglio dei bucket.

## Note
La guida consumatori ARERA continua a usare label legacy, da trattare come alias esplicativi e non come etichetta primaria.
