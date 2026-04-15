# Macro, prezzi domestici luce

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo slice già consolidati o parziali avanzati del repo su `Bolletta 2025`, `TIV`, `TIT/TIDE` e valori ARERA `maggior tutela` / `STG`.
- Non prova a ricostruire una formula unica del `mercato libero domestico`, perché la fonte primaria chiude struttura, disclosure e comparabilità minima, non una formula numerica cross-vendor.

## A colpo d'occhio
Nel repo è già chiuso il quadro minimo dei prezzi domestici regolati lato cliente: macro-voci della bolletta 2025, distinzione tra layer documentali, formule regolatorie di maggior tutela e STG, struttura base di rete, oneri e dispacciamento lato servizi regolati.

## Cosa si può dire con sicurezza
- Dal 2025 la bolletta elettrica lato cliente aggrega gli importi almeno in quattro aree leggibili: `Spesa per la vendita di energia elettrica`, `Spesa per la tariffa per l'uso della rete elettrica`, `Spesa per gli oneri generali di sistema`, `imposte`.
- Nel SSOT vanno tenuti distinti tre layer: `Scontrino dell'energia`, `Elementi di dettaglio`, `Glossario bolletta`.
- La `Spesa per la vendita di energia elettrica` può includere approvvigionamento, commercializzazione, dispacciamento, sconti e altri importi contrattuali di vendita.
- La macro-voce rete, nel perimetro domestico TIV già consolidato nel repo, è riconducibile a `σ1`, `σ2`, `σ3`, `UC3`, `UC6`.
- Gli oneri generali di sistema sono rappresentabili lato cliente con le componenti `ARIM` e `ASOS`.
- Per i clienti domestici in maggior tutela la rappresentazione minima chiusa è:
  - quota consumi: `PE + PD + PPE`
  - quota fissa per POD/anno: `PCV + DISPBT`
- Per i clienti domestici non vulnerabili in STG la rappresentazione minima chiusa è:
  - quota consumi: `CELD + CDISPD + CSED + CPSTGD`
  - quota fissa per POD/anno: `γ`
- Dal `2026-04-01`, per il `mercato libero domestico`, ARERA non impone una formula numerica unica cross-vendor ma una struttura standardizzata dei corrispettivi: nelle offerte non onnicomprensive `quota annua venditore + quota consumo venditore + dispacciamento/capacità + rete + oneri + imposte`; nelle offerte onnicomprensive `quota annua + quota consumo` comprensive di tutte le voci di spesa.
- Nel libero domestico restano vendor-specific il valore dei corrispettivi definiti dal venditore, l'indice o gli indici usati, l'eventuale adder, le articolazioni per fasce/scaglioni/potenza e gli eventuali sconti o servizi aggiuntivi.
- Per il dispacciamento del libero domestico il baseline minimo è ora chiuso su tre casi: `CDISPD` separato come default, eccezione `capacità Terna + dispacciamento TIDE` per offerte variabili almeno orarie, inclusione totale nelle offerte `onnicomprensive`.
- Le offerte `generalizzate` entrano nel `Portale Offerte`, che le confronta tramite `spesa annua stimata` e pagina di dettaglio standard; le offerte `non generalizzate` restano fuori da quel perimetro di comparabilità, mentre i casi art. `10.8` restano nel Portale con comparabilità derogatoria fino all'adeguamento.
- Il fatto che un'offerta sia `non generalizzata` chiude il perimetro `Portale Offerte`, non quello della disclosure domestica di base: la razionalizzazione 2026 dei corrispettivi è motivata da ARERA con riferimento a tutte le offerte domestiche, mentre bundle e servizi aggiuntivi restano in layer separato rispetto al prezzo energia.
- Sul piano promozionale il repo distingue ora in modo chiuso tra `sconti automatici primi 12 mesi`, che entrano nella `spesa annua stimata`, e altre promozioni o bonus, che restano rappresentati solo nel dettaglio dell'offerta con le relative condizioni.
- Sul recesso il baseline ora è chiuso anche sul piano attuativo ARERA: nel domestico il cambio fornitore e il recesso sono gratuiti come regola generale; un `onere di recesso anticipato` è ammissibile solo nel perimetro fixed-price fixed-term o fixed-price con condizioni economiche a termine, limitatamente al primo periodo fixed, con importo massimo ex ante, specifica approvazione del cliente, ricalcolo verso la perdita economica diretta effettiva e decadenza se il venditore varia unilateralmente le condizioni.
- Nel `Portale Offerte` l'eventuale onere di recesso anticipato resta un'informazione di presenza o di dettaglio e non entra nella `spesa annua stimata`.

## Valori customer-facing già verificati nel repo
- Maggior tutela, trimestre aprile-giugno 2026: ARERA pubblica `0,15811 euro/kWh` monorario e `44,7311 euro/anno` di quota fissa.
- STG domestico non vulnerabile, marzo 2026: ARERA pubblica `0,174479 euro/kWh` monorario e `-73,1637 euro/anno` di quota fissa.

## Punto delicato da non semplificare troppo
- Il `dispacciamento` non va ridotto a una sola cosa: nel repo è chiuso come funzione di sistema Terna/TIDE e come traduzione economica regolata diversa in maggior tutela (`PD` + `DISPBT`) e in STG (`CDISPD`).
- Nel libero domestico non basta più la coppia `separato/incluso`: per le offerte con aggiornamento almeno orario esiste un terzo mapping minimo source-backed, cioè `corrispettivo separato Terna+TIDE` in luogo del `CDISPD`.
- Le etichette legacy come `materia energia` o `trasporto e gestione del contatore` sono utili come alias consumatore, ma non sostituiscono la nomenclatura primaria della Bolletta 2025.

## Cosa resta aperto
- Non esiste, e non va inventata, una formula numerica unica del mercato libero domestico valida per tutti i contratti.
- Sullo slice prezzi/customer-facing qui riassunto non resta un open question SSOT attivo: restano solo futuri aggiornamenti regolatori o casi extra-corpus che, se emergeranno, andranno verificati da fonte primaria prima di entrare nel repo.

## Cosa deve contenere la macro-categoria sul libero domestico
- schema dell'offerta: `standard` oppure `onnicomprensiva`
- quota annua e quota consumo definite dal venditore, con unità di misura e condizioni applicative
- presenza di indicizzazione, indice/i, periodicità e eventuale adder unico
- trattamento del dispacciamento: `separato_CDISPD`, `separato_Terna_TIDE_orario`, `incluso_onnicomprensiva`, oppure `rinvio_regolatorio`
- bucket regolati separati quando esponibili: `rete`, `oneri`, `imposte`
- metadati di comparabilità: `codice offerta`, `Portale Offerte`, `spesa annua stimata`, `durata condizioni economiche`, `comparabilita_standard_o_art10_8`
- disclosure commerciale minima: `sconti_automatici_in_stima`, `sconti_bonus_detail_only`, `prodotti o servizi aggiuntivi`, `condizioni di recesso`, `Scheda sintetica`, `link/QR ARERA ai corrispettivi regolati`
- boundary recesso: `ripensamento_14_giorni`, `recesso_senza_oneri_default`, `onere_recesso_anticipato_ammesso_solo_se_fixed_term_fixed_price`, `importo_massimo_ex_ante`, `perdita_economica_diretta`, `costi_pacchetti_servizi_gia_erogati`

## Dove approfondire
- [../DOMAINS/prezzi-oneri-componenti.md](../DOMAINS/prezzi-oneri-componenti.md)
- `RULE-EE-PRC-001..014`
- `RULE-EE-CTR-001..005`
- `RULE-EE-DISP-001..004`
- `RULE-EE-TIV-002..003`
- `RULE-EE-STG-002..003`

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-ARERA-TIT-2024-2027-PDF`
- `SRC-ARERA-TIDE-REV4-2025-PDF`
- `SRC-GU-DL-19-2025-ART5`
- `SRC-ARERA-386-2025-R-COM-PDF`
- `SRC-ARERA-250-23-PDF`
- `SRC-ARERA-PORTALE-OFFERTE-2024-PDF`
- `SRC-NORMATTIVA-DLGS-210-2021-ART7`
- `SRC-ARERA-ATLANTE-RECESSO-COSA-E`
- `SRC-ARERA-MT-VALORI-2026-XLSX`
- `SRC-ARERA-STG-VALORI-2026-XLSX`
- `SRC-ARERA-ONERI-SISTEMA-PAGE`
- `SRC-TERNA-DISPACCIAMENTO-PAGE`
