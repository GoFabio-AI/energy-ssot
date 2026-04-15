# Dominio: Tutele graduali e regimi di servizio

## Perimetro attivo
- settore: energia elettrica
- segmento: clienti domestici
- focus: distinzione regolatoria tra clienti vulnerabili, clienti non vulnerabili e regimi di servizio rilevanti al 2026-04-15
- esclusioni temporanee: contratti/offerte di mercato libero di dettaglio, salvo i richiami minimi necessari a delimitare il perimetro

## Scopo
Consolidare il quadro minimo dei regimi di servizio domestici elettrici, separando il perimetro dei clienti vulnerabili, il servizio a tutele graduali per i non vulnerabili e i rinvii verso maggior tutela e mercato libero quando già coperti nel repo.

## Copre
- clienti domestici vulnerabili e non vulnerabili
- servizio a tutele graduali domestico non vulnerabile
- maggior tutela per clienti vulnerabili nel quadro transitorio consultato
- collegamento con il TIV e con le formule economiche regolatorie già chiuse altrove nel repo

## Fonti principali
- SRC-ARERA-362-23
- SRC-ARERA-TIV-2026-PDF
- SRC-ARERA-110-25-PDF
- SRC-ARERA-96-26-PAGE
- SRC-ARERA-TIT-2024-2027-PDF
- SRC-ARERA-TIDE-REV4-2025-PDF
- SRC-NORMATTIVA-DLGS-210-2021-ART11
- SRC-ARERA-ATLANTE-CLIENTI-VULNERABILI
- SRC-ARERA-MT-VULNERABILI
- SRC-AU-PREZZO-CESSIONE
- SRC-ARERA-FINE-TUTELA-ELE

## Fatti consolidati
- ARERA disciplina il servizio a tutele graduali per i clienti domestici non vulnerabili del settore elettrico.
- Il baseline regolatorio minimo vigente al 2026-04-15 per maggior tutela e STG domestico è il TIV valido dall'1 gennaio 2026, da coordinare con la deliberazione 110/2025/R/eel sul d.l. 19/25 e con l'aggiornamento trimestrale 96/2026/R/eel.
- Per uso trasversale nel repo, il baseline cross-domain al 2026-04-15 è da considerare chiuso come baseline composita ufficiale: `TIV` per regimi di servizio e vendita di ultima istanza, `DL 19/2025` articolo 2 comma 3 e `ARERA 110/2025/R/eel` per la permanenza dei vulnerabili nello STG, `ARERA 96/2026/R/eel` come checkpoint vigente del trimestre, `TIT` per rete e `TIDE` per dispacciamento quando i corrispettivi economici vengono raccordati con il dominio prezzi.
- Le categorie di clienti vulnerabili sono definite dall'articolo 11 del d.lgs. 210/2021 vigente.
- Nelle more dell'aggiudicazione del servizio di vulnerabilità, il cliente vulnerabile può essere servito nel perimetro di maggior tutela dal soggetto competente per territorio.
- Acquirente Unico pubblica il prezzo di cessione agli esercenti la maggior tutela per i clienti domestici vulnerabili.
- La formula economica regolata STG domestico non vulnerabile è già coperta nel repo, ma resta referenziata nel dominio prezzi-oneri-componenti e non va duplicata qui.

## Evidenze estratte
- `EXTRACTED/SRC-ARERA-362-23.extracted.md`
- `EXTRACTED/SRC-ARERA-TIV-2026-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-110-25-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-96-26-PAGE.extracted.md`
- `EXTRACTED/SRC-ARERA-TIT-2024-2027-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIDE-REV4-2025-PDF.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DLGS-210-2021-ART11.extracted.md`
- `EXTRACTED/SRC-ARERA-ATLANTE-CLIENTI-VULNERABILI.extracted.md`
- `EXTRACTED/SRC-ARERA-MT-VULNERABILI.extracted.md`
- `EXTRACTED/SRC-AU-PREZZO-CESSIONE.extracted.md`

## Regole collegate
- RULE-EE-STG-001
- RULE-EE-STG-002
- RULE-EE-STG-003
- RULE-EE-VUL-001
- RULE-EE-VUL-002
- RULE-EE-VUL-003
- RULE-EE-TIV-001
- RULE-EE-TIV-003

## Open questions
- nessuna open question normativa rossa residua sul baseline vulnerabili/STG al 2026-04-15; resta solo monitoraggio editoriale di eventuali futuri consolidati ARERA che incorporino in un unico testo aggiornamenti già coordinati nel repo

## Stato avanzamento
- Coperti: categorie di vulnerabilità, maggior tutela per vulnerabili nel quadro transitorio, STG per non vulnerabili, raccordo con TIV e baseline composita TIV/TIT/TIDE usata nel repo.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15. Restano solo consolidati futuri o rifiniture editoriali di rinvio.

## Vedi anche
- [DOMAINS/attori-mercato.md](attori-mercato.md)
- [DOMAINS/prezzi-oneri-componenti.md](prezzi-oneri-componenti.md)
- [DOMAINS/bonus-sociale.md](bonus-sociale.md)
- [OPEN-QUESTIONS.md](../OPEN-QUESTIONS.md)
- [GLOSSARIO.md](../GLOSSARIO.md)

## Glossario collegato
- cliente finale domestico
- cliente vulnerabile
- maggior tutela
- servizio a tutele graduali
- mercato libero
