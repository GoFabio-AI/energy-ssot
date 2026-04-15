# Dominio: Fiscalità

## Perimetro attivo
- settore: energia elettrica
- segmento: clienti domestici
- focus: accisa e IVA domestiche al 2026-04-15
- esclusioni temporanee: gas, usi non domestici, forniture business, tributi diversi da accisa e IVA

## Scopo
Separare in un package autonomo la fiscalità domestica elettrica di base già chiusa nel repo, senza estendere il corpus oltre accisa abitazioni, agevolazione residente, IVA per uso domestico e principali esclusioni già verificate.

## Copre
- imponibilità generale dell'accisa sulla fornitura di energia elettrica
- aliquota base accisa per abitazioni
- agevolazione accisa per residenza anagrafica
- IVA per uso domestico
- criterio interpretativo dell'uso domestico ai fini IVA
- esclusione delle parti comuni condominiali dall'uso domestico IVA
- esposizione separata delle imposte nella bolletta elettrica 2025

## Fonti principali
- SRC-NORMATTIVA-DLGS-504-ART52
- SRC-ADM-ALIQUOTE-NAZIONALI-2026
- SRC-ADM-EE-ISTRUZIONI-2026
- SRC-NORMATTIVA-DPR-633-TABELLA-A-2026
- SRC-AE-RISOLUZIONE-8E-2017
- SRC-AE-RISPOSTA-3-2018
- SRC-ARERA-BOLLETTA-2025-PDF

## Fatti consolidati
- L'energia elettrica è sottoposta ad accisa ed è esigibile al momento della fornitura al consumatore finale oppure del consumo per uso proprio da parte del soggetto che la produce.
- Per le abitazioni, il prospetto ufficiale ADM aggiornato al 2026-01-01 riporta un'accisa base pari a `0,0227 euro/kWh`.
- L'esenzione accisa domestica residente vale solo per abitazioni di residenza anagrafica degli utenti, con potenza impegnata fino a `3 kW`, fino a `150 kWh` mensili, con i meccanismi di recupero previsti dalla stessa disciplina e dalle istruzioni ADM.
- Al 2026-04-15, l'energia elettrica per uso domestico rientra nel n. 103 della Tabella A, Parte III, del DPR 633/1972, quindi nell'aliquota IVA del `9%`.
- Le fonti Agenzia delle Entrate già consolidate nel repo qualificano l'uso domestico in base all'impiego della fornitura nell'abitazione familiare o in strutture collettive residenziali analoghe, purché l'energia non sia usata nell'esercizio di imprese o per prestazioni di servizi rilevanti ai fini IVA.
- Le parti comuni dei condomini non soddisfano il requisito dell'uso domestico ai fini IVA.
- Nella Bolletta 2025 le imposte sono riportate separatamente in un riquadro dedicato e non vanno confuse con i bucket economici principali della vendita, della rete e degli oneri generali di sistema.

## Interpretazione minima
- La distinzione `residente / non residente` è supportata nel repo sul lato accisa, perché l'agevolazione dell'articolo 52, comma 3, lettera e), è limitata alla residenza anagrafica.
- Per l'IVA il criterio rilevante emerso dal corpus è l'`uso domestico`, non una distinzione autonoma residente/non residente.
- Il package fiscale domestico del repo è chiuso per il baseline customer-facing e di classificazione, non per tutte le casistiche extra-perimetro o business.

## Evidenze estratte
- `EXTRACTED/SRC-NORMATTIVA-DLGS-504-ART52.extracted.md`
- `EXTRACTED/SRC-ADM-ALIQUOTE-NAZIONALI-2026.extracted.md`
- `EXTRACTED/SRC-ADM-EE-ISTRUZIONI-2026.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DPR-633-TABELLA-A-2026.extracted.md`
- `EXTRACTED/SRC-AE-RISOLUZIONE-8E-2017.extracted.md`
- `EXTRACTED/SRC-AE-RISPOSTA-3-2018.extracted.md`
- `EXTRACTED/SRC-ARERA-BOLLETTA-2025-PDF.extracted.md`

## Regole collegate
- RULE-EE-FISC-ACCISA-001
- RULE-EE-FISC-ACCISA-002
- RULE-EE-FISC-ACCISA-003
- RULE-EE-FISC-IVA-001
- RULE-EE-FISC-IVA-002
- RULE-EE-FISC-IVA-003

## Open questions
- nessuna open question normativa rossa specifica sul baseline fiscale domestico al 2026-04-15; restano solo futuri aggiornamenti di aliquote, chiarimenti ADM o consolidati fiscali ulteriori

## Stato avanzamento
- Coperti: accisa domestica base, agevolazione residente, IVA uso domestico, esclusione delle parti comuni condominiali e separazione delle imposte nella bolletta 2025.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15. Restano solo aggiornamenti futuri di fonte fiscale ufficiale.

## Vedi anche
- [prezzi-oneri-componenti.md](prezzi-oneri-componenti.md)
- [fatturazione.md](fatturazione.md)
- [bonus-sociale.md](bonus-sociale.md)
- [../OPEN-QUESTIONS.md](../OPEN-QUESTIONS.md)
- [../GLOSSARIO.md](../GLOSSARIO.md)

## Glossario collegato
- accisa
- IVA
- uso domestico
- residenza anagrafica
- imposte
