# Macro, fiscalità domestica luce

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo il materiale già consolidato nel repo su `accisa`, `agevolazione residente` e `IVA uso domestico`.
- Non estende le regole qui riassunte a casi fuori perimetro, come forniture business o altri usi non domestici.

## A colpo d'occhio
La fiscalità domestica elettrica è già leggibile nel repo senza grandi buchi: l'accisa è coperta come regola generale più agevolazione residente, l'IVA è coperta come uso domestico con chiarimento sulle esclusioni delle parti comuni condominiali.

## Cosa si può dire con sicurezza
- L'energia elettrica è soggetta ad accisa al momento della fornitura al consumatore finale.
- Per le abitazioni, il prospetto ADM aggiornato al 2026-01-01 riporta un'accisa base di `0,0227 euro/kWh`.
- L'agevolazione residente non è una nozione commerciale generica: vale per abitazioni di residenza anagrafica dell'utente, con potenza impegnata fino a `3 kW`, fino a `150 kWh` mensili, con i meccanismi di recupero previsti dalla norma e dalle istruzioni ADM.
- Al 2026-04-15 l'energia elettrica per uso domestico rientra nell'aliquota IVA del `9%`.
- Per l'IVA il criterio emerso nel repo è l'`uso domestico`, non una distinzione autonoma residente/non residente.
- Le parti comuni dei condomini non rientrano nell'uso domestico IVA.

## Distinzione pratica importante
- Sul lato accisa la distinzione residente/non residente conta, perché l'esenzione è legata alla residenza anagrafica.
- Sul lato IVA il repo non supporta una regola autonoma residente/non residente: ciò che conta è l'uso domestico della fornitura.

## Cosa evitare
- Non fondere in una sola regola `domestico = sempre stessa fiscalità`.
- Non creare una regola IVA `residente` o `non residente` come se fosse espressa dalle fonti già lavorate.
- Non trattare le utenze condominiali delle parti comuni come uso domestico IVA solo perché l'edificio è residenziale.

## Cosa resta aperto
- Non c'è un gap normativo importante nel perimetro fiscale base già lavorato.
- Il dominio autonomo `fiscalita` esiste ora nel repo; restano solo futuri aggiornamenti ADM o fiscali, non un gap strutturale di packaging.

## Dove approfondire
- [../DOMAINS/fiscalita.md](../DOMAINS/fiscalita.md)
- [../DOMAINS/prezzi-oneri-componenti.md](../DOMAINS/prezzi-oneri-componenti.md)
- `RULE-EE-FISC-ACCISA-001..003`
- `RULE-EE-FISC-IVA-001..003`

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-NORMATTIVA-DLGS-504-ART52`
- `SRC-ADM-ALIQUOTE-NAZIONALI-2026`
- `SRC-ADM-EE-ISTRUZIONI-2026`
- `SRC-NORMATTIVA-DPR-633-TABELLA-A-2026`
- `SRC-AE-RISOLUZIONE-8E-2017`
- `SRC-AE-RISPOSTA-3-2018`
