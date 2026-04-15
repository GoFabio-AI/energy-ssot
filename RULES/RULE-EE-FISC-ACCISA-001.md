# RULE-EE-FISC-ACCISA-001

## Metadata
- ID: RULE-EE-FISC-ACCISA-001
- Titolo: Aliquota accisa base per energia elettrica nelle abitazioni al 2026-04-15
- Dominio: fiscalita
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ADM-ALIQUOTE-NAZIONALI-2026
- URL fonte: https://www.adm.gov.it/portale/documents/20182/43975520/Aliquote+nazionali++aggiornamento+al+01+gennaio+2026.pdf/22915fb7-c5d8-f974-36d5-7ae5ad757385?t=1767194770129
- Riferimento preciso: sezione "Accise sull'energia elettrica", aggiornamento al 01 gennaio 2026
- Data pubblicazione: 2026-01-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Per qualsiasi applicazione nelle abitazioni, al 2026-04-15 il prospetto ufficiale ADM delle aliquote nazionali riporta un'accisa di euro 0,0227 per ogni kWh.

## Citazione
"per qualsiasi applicazione nelle abitazioni"; "€ 0,0227 per ogni kWh".

## Interpretazione minima
Questa è l'aliquota base domestica abitazioni. Non incorpora da sola l'esenzione specifica per residenza anagrafica prevista dall'art. 52, comma 3, lettera e).

## Impatto operativo
Nei modelli SSOT e nei motori di calcolo occorre distinguere tra aliquota base abitazioni e agevolazione residente, invece di usare una sola regola fiscale domestica indistinta.

## Eccezioni e limiti
La regola non copre locali e luoghi diversi dalle abitazioni né il recupero della fascia esente residente.

## Conflitti o dipendenze
Dipende da RULE-EE-FISC-ACCISA-002 per la casistica residente con esenzione.

## Note
Il prospetto ADM richiama il D.M. 30/12/2011 come riferimento normativo dell'aliquota abitazioni.
