# Macro, bonus sociale e clienti vulnerabili

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo il nucleo già ben supportato nel repo su `bonus sociale per disagio economico` e `clienti vulnerabili`.
- Include ora anche gli importi ordinari 2026 del bonus sociale elettrico e la loro esposizione minima in bolletta, perché risultano coperti da fonte ARERA.

## A colpo d'occhio
Il repo ha già un nucleo forte su bonus sociale elettrico per disagio economico e su vulnerabilità: requisiti, flusso operativo, durata del beneficio e rapporto tra vulnerabili, maggior tutela e STG sono leggibili senza introdurre fonti nuove.

## Bonus sociale, quadro breve
- Il bonus sociale elettrico per disagio economico è uno sconto automatico in bolletta.
- Vale `12 mesi` e si applica su una sola fornitura elettrica agevolabile.
- Gli importi ordinari 2026 sono:
  - `146,00 euro/anno` per nuclei di `1-2 componenti`, pari a `0,40 euro/giorno` e `12,00 euro/30 gg`
  - `186,15 euro/anno` per nuclei di `3-4 componenti`, pari a `0,51 euro/giorno` e `15,30 euro/30 gg`
  - `204,40 euro/anno` per nuclei `oltre 4 componenti`, pari a `0,56 euro/giorno` e `16,80 euro/30 gg`
- Le soglie ISEE consolidate nel repo al 2026-04-15 sono:
  - `9.796 euro` per nuclei con massimo 3 figli a carico
  - `20.000 euro` per nuclei con almeno 4 figli a carico
- Per la fornitura diretta la bolletta deve essere intestata a un componente del nucleo ISEE, per uso domestico, attiva o sospesa per morosità.
- Il venditore non è il punto di avvio del diritto: il flusso passa da `DSU/ISEE`, `INPS`, `SII` e poi applicazione dello sconto nella prima fattura utile.
- Lo sconto è uguale ogni mese per i 12 mesi di diritto; ARERA fa l'esempio di una bolletta bimestrale con `30 euro` di riduzione quando il bonus mensile è `15 euro`.
- Nella bolletta il bonus è esposto come voce separata `bonus sociale` in detrazione, e la bolletta indica anche la data di scadenza del bonus per disagio economico.

## Vulnerabilità, quadro breve
- Il perimetro dei clienti vulnerabili è normativo e tassativo.
- Nel repo risultano coperte queste categorie: condizioni economicamente svantaggiate, gravi condizioni di salute o presenza di apparecchiature elettromedicali, disabilità ai sensi della legge 104/92, utenze in isole minori non interconnesse, utenze in strutture abitative di emergenza per eventi calamitosi, clienti con più di 75 anni.
- La vulnerabilità per disagio economico si collega direttamente al tema bonus sociale.

## Regime di servizio già leggibile nel repo
- Nelle more del servizio di vulnerabilità aggiudicato, il cliente vulnerabile può essere servito dall'esercente di maggior tutela competente per territorio.
- Se un cliente già in STG diventa vulnerabile, non esce automaticamente dallo STG: resta nel servizio fino a fine assegnazione, ma può scegliere maggior tutela o mercato libero.
- Per lo snapshot `2026-04-15`, il repo usa ormai come baseline cross-domain chiusa una catena ufficiale composta da `d.lgs. 210/2021 art. 11`, `TIV` coordinato con `DL 19/2025`, `ARERA 110/2025/R/eel` e `ARERA 96/2026/R/eel`; non manca più un ulteriore fatto normativo di base per leggere il perimetro vulnerabili.

## Cosa resta aperto
- Non resta un gap normativo rosso sul baseline clienti vulnerabili al `2026-04-15`.
- Resta solo un tema di manutenzione editoriale: se ARERA pubblicherà un consolidato unico ancora più esplicito, il repo potrà semplificare i rinvii senza cambiare i fatti già chiusi.

## Dove approfondire
- [../DOMAINS/bonus-sociale.md](../DOMAINS/bonus-sociale.md)
- [../DOMAINS/tutele-graduali.md](../DOMAINS/tutele-graduali.md)
- `RULE-EE-BONUS-001..005`
- `RULE-EE-VUL-001..003`

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-ARERA-63-21`
- `SRC-ARERA-BONUS-REQUISITI`
- `SRC-ARERA-BONUS-PROCEDIMENTO`
- `SRC-ARERA-BONUS-AMMONTANO`
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-INPS-PORTALE-ISEE`
- `SRC-NORMATTIVA-DLGS-210-2021-ART11`
- `SRC-GU-DL-19-2025-ART2`
- `SRC-ARERA-MT-VULNERABILI`
- `SRC-ARERA-ATLANTE-CLIENTI-VULNERABILI`
