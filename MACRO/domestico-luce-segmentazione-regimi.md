# Macro, segmentazione cliente e routing di regime domestico luce

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo il materiale già consolidato nel repo su `attori-mercato`, `tutele-graduali`, `bonus-sociale` e `bonus-vulnerabili`.
- Serve come vista editoriale unica del routing minimo cliente/regime, non come nuovo testo normativo autonomo.

## A colpo d'occhio
Nel repo il domestico luce è ormai leggibile con una segmentazione minima unica: `cliente vulnerabile`, `cliente non vulnerabile`, `cliente nel mercato libero`, `cliente nel servizio regolato rilevante` e caso speciale del `cliente già in STG che diventa vulnerabile`. Il bonus sociale economico entra come beneficio separato, ma si collega direttamente alla vulnerabilità per disagio economico.

## Segmenti minimi da tenere distinti
- `cliente domestico vulnerabile`
- `cliente domestico non vulnerabile`
- `cliente nel mercato libero`
- `cliente nel servizio a tutele graduali`
- `cliente servito in maggior tutela` nel quadro transitorio consultato per i vulnerabili

## Vulnerabilità, quadro breve
- Il perimetro dei clienti vulnerabili è normativo e tassativo.
- Nel repo risultano coperte queste categorie: condizioni economicamente svantaggiate, gravi condizioni di salute o apparecchiature elettromedicali, disabilità ai sensi della legge `104/92`, utenze in isole minori non interconnesse, utenze in strutture abitative di emergenza per eventi calamitosi, clienti con più di `75` anni.
- La vulnerabilità per disagio economico si collega direttamente al bonus sociale elettrico, ma non esaurisce tutte le categorie di vulnerabilità.

## Routing di regime già leggibile nel repo
- Il cliente vulnerabile può scegliere il mercato libero oppure il servizio regolato competente per territorio.
- Nelle more dell'aggiudicazione del servizio di vulnerabilità, il cliente vulnerabile può essere servito dall'esercente di maggior tutela competente per territorio.
- Il servizio a tutele graduali è il regime regolato rilevante per il domestico non vulnerabile nel perimetro già chiuso del repo.
- Se un cliente già in `STG` diventa vulnerabile, non esce automaticamente dallo `STG`: resta nel servizio fino a fine assegnazione, ma può scegliere maggior tutela o mercato libero.
- Il bonus sociale per disagio economico non coincide con un regime di servizio: è uno sconto automatico in bolletta che passa dal flusso `DSU/ISEE -> INPS -> SII -> venditore`.

## Vista editoriale minima di routing
- `vulnerabile` -> può stare nel `mercato libero` oppure richiedere il `servizio regolato` competente; nel quadro transitorio del repo questo coincide con la `maggior tutela` per territorio
- `non vulnerabile` -> può stare nel `mercato libero`; quando il repo guarda il perimetro regolato domestico di ultima istanza, il riferimento è lo `STG`
- `cliente STG che diventa vulnerabile` -> resta `STG` fino a fine assegnazione, con facoltà di passare a `maggior tutela` o `mercato libero`
- `cliente in disagio economico` -> se ricorrono i requisiti ISEE e di fornitura, ha anche il percorso `bonus sociale`, separato dal routing del regime ma collegato allo status di vulnerabilità

## Attori da non confondere con i regimi
- `SII` e `RCU` sono backbone di dati e processi, non regimi di servizio.
- `Acquirente Unico` mantiene un ruolo di sistema e pubblica il prezzo di cessione agli esercenti la maggior tutela per i clienti domestici vulnerabili.
- `Venditore`, `controparte commerciale`, `UdD` e `distributore` sono soggetti di processo e di mercato, non etichette di segmentazione cliente.

## Cosa evitare
- Non trattare `vulnerabile` e `beneficiario bonus` come sinonimi perfetti.
- Non trattare `maggior tutela` come destinazione automatica di ogni cliente vulnerabile in ogni caso.
- Non dire che il cliente che diventa vulnerabile esce automaticamente dallo `STG`.
- Non confondere ruolo dell'attore di mercato, stato di vulnerabilità e regime di servizio come se fossero lo stesso oggetto.

## Cosa resta aperto
- Non resta un gap normativo rosso sul baseline di segmentazione e routing minimo al `2026-04-15`.
- Restano solo rifiniture editoriali future, soprattutto su definizioni glossario di alcuni ruoli di mercato e su eventuali futuri consolidati ARERA che semplifichino i rinvii oggi già chiusi nel repo.

## Dove approfondire
- [../DOMAINS/attori-mercato.md](../DOMAINS/attori-mercato.md)
- [../DOMAINS/tutele-graduali.md](../DOMAINS/tutele-graduali.md)
- [../DOMAINS/bonus-sociale.md](../DOMAINS/bonus-sociale.md)
- [domestico-luce-bonus-vulnerabili.md](domestico-luce-bonus-vulnerabili.md)

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-NORMATTIVA-DLGS-210-2021-ART11`
- `SRC-GU-DL-19-2025-ART2`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-ARERA-110-25-PDF`
- `SRC-ARERA-96-26-PAGE`
- `SRC-ARERA-ATLANTE-CLIENTI-VULNERABILI`
- `SRC-ARERA-MT-VULNERABILI`
- `SRC-AU-PREZZO-CESSIONE`
- `SRC-ARERA-BONUS-REQUISITI`
- `SRC-ARERA-BONUS-PROCEDIMENTO`
- `SRC-ARERA-BONUS-AMMONTANO`
- `SRC-INPS-PORTALE-ISEE`
