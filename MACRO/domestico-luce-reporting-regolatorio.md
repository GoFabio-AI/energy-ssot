# Macro, reporting regolatorio end-to-end domestico luce

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo materiale già consolidato nel repo su `TIQV`, `TIME`, `TIF`, bolletta, `Portale Consumi` e layer documentale minimo collegato ai reclami o all'area personale.
- Serve a leggere in un solo posto il package `reporting/comunicazioni/registri/call-center/pubblicazioni`, prima distribuito tra due domini diversi.
- Non sostituisce i domini di dettaglio su qualità commerciale, misure, fatturazione o dati `POD`.

## A colpo d'occhio
Nel repo il reporting regolatorio domestico luce ora si legge come due filiere che si incontrano senza confondersi:
- `misura -> SII -> bolletta -> visibilità cliente`
- `contatto cliente -> classificazione TIQV -> registro verificabile -> reporting/publishing annuale`

La nuova chiusura è editoriale, non inventa nulla di nuovo: mette nello stesso package solo materiale già source-backed.

## 1) Intake e prova della comunicazione
- Il venditore deve consentire l'invio online di reclami scritti o richieste di informazioni anche senza registrazione.
- L'invio deve lasciare una prova con `data di invio` e `codice pratica`.
- Se esiste un'area personale, deve esserci anche una modalità semplificata per selezionare la fornitura interessata e scaricare la copia della comunicazione inviata.

## 2) Post-cessazione e allegati minimi nelle risposte
- Se il venditore offre un'area personale, dopo la cessazione il cliente deve potervi accedere per almeno `6 mesi` almeno per reclami, richieste di informazioni, archivio bollette e archivio notifiche.
- Se il reclamo riguarda importi fatturati, la risposta motivata deve allegare gli `Elementi di dettaglio` della bolletta.
- Nel mercato libero, allo stesso reclamo vanno aggiunti anche `Scheda sintetica` dell'offerta ed eventuali preavvisi rilevanti su rinnovi o modifiche economiche.
- Questo non equivale a un obbligo generale di archivio documentale online del venditore: il repo continua a separare area personale TIQV, Portale Consumi e documenti su supporto durevole.

## 3) Classificazione e registri
- In caso di dubbio, la comunicazione va trattata come `reclamo` e non come semplice richiesta di informazioni.
- Reclami e richieste vanno classificati con la tabella A del `TIQV`.
- Il venditore deve mantenere un registro verificabile di reclami scritti, richieste scritte di informazioni, rettifiche di fatturazione e doppia fatturazione.
- Nel registro entrano almeno classificazione, `POD/PDR`, date rilevanti, cause di eventuale mancato rispetto e indennizzi.
- La documentazione di supporto deve restare ordinata, accessibile e verificabile per almeno `3 anni solari` successivi alla registrazione.

## 4) Call center e flussi annuali verso ARERA
- Il servizio telefonico commerciale deve avere almeno `35 ore settimanali` con operatore e rispettare gli standard minimi TIQV.
- Per ogni chiamata vanno registrati i dati necessari a rendere verificabili almeno `AS`, `TMA` e `LS`.
- I venditori sopra `50.000` clienti finali `TIQV` al `31 dicembre` devono comunicare ad `ARERA` entro il `28 febbraio` i dati mensili dell'anno precedente sul call center.
- Entro lo stesso `28 febbraio`, il venditore comunica anche i dati annuali su reclami, richieste, rettifiche, cause di mancato rispetto, tempi medi, pratiche aperte e indennizzi.

## 5) Pubblicazioni e survey
- Entro il `30 giugno` il venditore pubblica sul proprio sito standard, indennizzi e performance annuali di qualità commerciale.
- `ARERA` può selezionare venditori per survey sui call center e sulle risposte ai reclami.
- `ARERA` pubblica annualmente dati su qualità telefonica e qualità commerciale, anche con logiche comparative.
- Le determinazioni ARERA richiamate dal `TIQV` in questo punto sono procedurali, non nuove estensioni materiali del baseline.

## 6) Reporting del dato di misura
- Il `TIME` impone che i dati di misura siano messi a disposizione del `SII` con tempi regolati e qualificazione come `effettivi`, `autoletture` o `stimati`.
- Per i misuratori `2G` messi a regime, la disponibilità del dato è giornaliera.
- `TIF` e disciplina bolletta impongono poi di mostrare separatamente letture, autoletture, letture stimate, consumi effettivi, consumi stimati e consumi fatturati, oltre alla finestra di autolettura nei casi previsti.
- Il `Portale Consumi` resta il layer self-service del cliente sui dati della fornitura, distinto dalle pubblicazioni annuali e distinto da un archivio documentale generale del venditore.

## 7) Boundary già chiuso nel repo
- Il reporting regolatorio end-to-end non è più solo una combinazione implicita di due domini.
- Il nuovo package unifica, senza duplicare nuove regole, il layer `comunicazioni/registri/call-center/pubblicazioni/reporting misura` già consolidato.
- Restano invece nei rispettivi domini di dettaglio gli `SLA`, le regole complete di risposta al reclamo, i dettagli di fatturazione, il set `POD` e il perimetro privacy o documentale completo.

## Dove approfondire
- [../DOMAINS/reporting-regolatorio.md](../DOMAINS/reporting-regolatorio.md)
- [../DOMAINS/qualita-commerciale-reclami.md](../DOMAINS/qualita-commerciale-reclami.md)
- [../DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md](../DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md)
- [../DOMAINS/misure.md](../DOMAINS/misure.md)
- [../DOMAINS/fatturazione.md](../DOMAINS/fatturazione.md)
- `RULE-EE-TIQV-007..029`
- `RULE-EE-TIME-003`
- `RULE-EE-TIF-003`
- `RULE-EE-BOLL-001`

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-ARERA-TIQV-2026-PDF`
- `SRC-ARERA-TIME-2024-PDF`
- `SRC-ARERA-TIF-2025-PDF`
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-ARERA-PORTALE-CONSUMI-PAGE`
- `SRC-AU-PORTALE-CONSUMI-HOMEPAGE-PAGE`
- `SRC-ARERA-CCC24-PDF`
- `SRC-NORMATTIVA-DLGS-206-2005`
