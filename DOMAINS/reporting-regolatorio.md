# Dominio: Reporting regolatorio, comunicazioni e registri

## Perimetro attivo
- settore: energia elettrica
- segmento: clienti domestici
- data di riferimento SSOT: 2026-04-15
- focus: layer end-to-end di intake, comunicazioni verificabili, registri, call center, flussi verso ARERA, pubblicazioni annuali e reporting di misura direttamente collegato alla fornitura

## Scopo
Unificare in un package dedicato il layer di reporting regolatorio che nel repo era già chiuso nei contenuti ma distribuito tra `anagrafica-tecnica-pod-accessi-reporting` e `qualita-commerciale-reclami`, senza introdurre nuove fonti o nuovi fatti.

## Copre
- invio online di reclami scritti o richieste di informazioni senza registrazione, con prova di invio e codice pratica
- funzionalità semplificata nell'area personale e disponibilità post-cessazione minima quando l'area personale esiste
- pacchetto documentale minimo da allegare alle risposte sui reclami relativi agli importi fatturati
- classificazione prudenziale TIQV tra reclamo e richiesta di informazioni e tassonomia tabella A
- standard minimi di call center e registrazione dei dati necessari a rendere verificabili gli indicatori telefonici
- registri verificabili di reclami, richieste, rettifiche e doppie fatturazioni, con retention documentale minima
- comunicazioni annuali ad ARERA su call center e qualità commerciale
- pubblicazione annuale lato venditore e pubblicazione o survey lato ARERA
- reporting regolato dei dati di misura verso il SII e loro rappresentazione separata in bolletta
- boundary tra Portale Consumi, pubblicazioni regolatorie, documenti su supporto durevole e archivi interni del venditore

## Fonti principali
### Primarie
- SRC-ARERA-TIQV-2026-PDF
- SRC-ARERA-TIME-2024-PDF
- SRC-ARERA-TIF-2025-PDF
- SRC-ARERA-BOLLETTA-2025-PDF
- SRC-ARERA-CCC24-PDF
- SRC-NORMATTIVA-DLGS-206-2005
- SRC-GU-L-205-2017-ART1-C6-C8

### Ufficiali di supporto
- SRC-ARERA-PORTALE-CONSUMI-PAGE
- SRC-AU-PORTALE-CONSUMI-HOMEPAGE-PAGE
- SRC-AU-PORTALE-CONSUMI-PRIVACY-PAGE
- SRC-AU-SII-TRATTAMENTO-DATI-PERSONALI-PAGE

## Fatti consolidati
### Intake digitale e comunicazioni verificabili verso il cliente
- Il sito del venditore deve mettere a disposizione una funzionalità che consenta di inviare reclami scritti o richieste di informazioni anche senza registrazione, con ricevuta che attesti la data di invio e il codice pratica.
- Se il venditore offre un'area personale, deve esistere anche una funzionalità di invio semplificato che consenta di selezionare la fornitura interessata e di scaricare la copia della comunicazione inviata.
- Se il venditore offre un'area personale online, dopo la cessazione il cliente deve poter continuare ad accedervi per almeno 6 mesi almeno per reclami, richieste di informazioni, archivio delle bollette emesse e archivio delle notifiche.
- Quando il reclamo riguarda importi fatturati, la risposta motivata deve allegare gli `Elementi di dettaglio` della bolletta e, nel mercato libero, anche la `Scheda sintetica` dell'offerta e gli eventuali preavvisi rilevanti su variazioni unilaterali, evoluzioni automatiche o rinnovi con modifica delle condizioni economiche.
- Questo layer non trasforma il reporting regolatorio in un obbligo generale di archivio documentale online del venditore: le copie di contratto, `Scheda sintetica` e conferme contrattuali restano coperte come documenti su supporto durevole nei rispettivi domini.

### Classificazione prudenziale e registri verificabili
- Nel TIQV, in caso di dubbio la comunicazione del cliente va trattata come reclamo prima e indipendentemente dal merito, non come semplice richiesta di informazioni.
- Reclami e richieste vanno classificati secondo la tabella A del TIQV, con bucket ufficiali riusabili almeno su contratti, morosità e sospensione, mercato, fatturazione, misura, connessioni o qualità tecnica, bonus sociale, qualità commerciale e altro o non competenza.
- Il venditore deve mantenere un registro verificabile di reclami scritti, richieste scritte di informazioni, rettifiche di fatturazione e doppia fatturazione, con classificazione, POD o PDR, date rilevanti, eventuali cause di mancato rispetto e indennizzi.
- La documentazione di supporto a tale registro deve restare ordinata, accessibile e verificabile per almeno 3 anni solari successivi alla registrazione.

### Call center e comunicazioni annuali ad ARERA
- Il servizio telefonico commerciale deve avere almeno 35 ore settimanali con operatore e rispettare gli standard minimi TIQV sul call center.
- Per ogni chiamata pervenuta al call center devono essere registrati i dati necessari a rendere verificabili almeno `AS`, `TMA` e `LS`.
- I venditori sopra la soglia di 50.000 clienti finali TIQV al 31 dicembre devono comunicare ad ARERA entro il 28 febbraio i dati mensili dell'anno precedente su chiamate e indicatori del call center.
- Entro il 28 febbraio il venditore deve inoltre comunicare ad ARERA i dati annuali su reclami, richieste, rettifiche, doppie fatturazioni, esiti, cause di mancato rispetto, tempi medi, pratiche ancora aperte e indennizzi.

### Pubblicazioni lato venditore e lato ARERA
- Entro il 30 giugno il venditore deve pubblicare sul proprio sito standard, indennizzi e performance annuali di qualità commerciale.
- Il TIQV non si esaurisce nei flussi annuali ordinari: ARERA può selezionare venditori per indagini annuali sui call center e sulle risposte ai reclami.
- ARERA pubblica annualmente dati sulla qualità dei servizi telefonici e sulla qualità commerciale dei venditori, anche con logiche comparative.
- Le determinazioni ARERA richiamate dagli articoli 31, 33, 38 e 39 del TIQV sono atti operativi e procedurali, non estensioni materiali del baseline regolatorio già chiuso nel repo.

### Reporting del dato di misura e visibilità regolata della fornitura
- Il `TIME` impone che i dati di misura siano messi a disposizione del `SII` con tempi regolati e con qualificazione del dato come effettivo, autolettura o stimato; per i misuratori 2G messi a regime la disponibilità è giornaliera.
- Il `TIF` e la disciplina della bolletta impongono al venditore di mostrare separatamente letture, autoletture, letture stimate, consumi effettivi, consumi stimati e consumi fatturati, oltre alla finestra di autolettura nei casi previsti e all'avviso di possibile ricalcolo quando si usano dati stimati.
- Il `Portale Consumi` resta il layer online data-centric di accesso del cliente a consumi, letture e principali informazioni della fornitura, distinto sia dalle pubblicazioni regolatorie annuali sia da un eventuale archivio documentale del venditore.
- Il boundary SSOT ora è quindi leggibile end-to-end: `dato di misura -> SII -> bolletta e visibilità cliente` da un lato, `intake reclamo o richiesta -> classificazione -> registro -> reporting/publishing TIQV` dall'altro.

### Boundary del package
- Questo package unifica il layer reporting e comunicazioni, ma non sostituisce i domini di dettaglio su `misure`, `fatturazione`, `anagrafica-tecnica-pod-accessi-reporting` e `qualita-commerciale-reclami`.
- Non restano open question strutturali attive su questo slice al `2026-04-15`: il gap residuo del repo era editoriale e viene chiuso qui senza creare nuove regole.

## Evidenze estratte
- `EXTRACTED/SRC-ARERA-TIQV-2026-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIME-2024-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIF-2025-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-BOLLETTA-2025-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-PORTALE-CONSUMI-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-PORTALE-CONSUMI-HOMEPAGE-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-PORTALE-CONSUMI-PRIVACY-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-SII-TRATTAMENTO-DATI-PERSONALI-PAGE.extracted.md`
- `EXTRACTED/SRC-ARERA-CCC24-PDF.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DLGS-206-2005.extracted.md`
- `EXTRACTED/SRC-GU-L-205-2017-ART1-C6-C8.extracted.md`

## Regole collegate
- RULE-EE-BOLL-001
- RULE-EE-TIF-003
- RULE-EE-TIME-003
- RULE-EE-TIQV-007
- RULE-EE-TIQV-008
- RULE-EE-TIQV-009
- RULE-EE-TIQV-010
- RULE-EE-TIQV-013
- RULE-EE-TIQV-014
- RULE-EE-TIQV-015
- RULE-EE-TIQV-016
- RULE-EE-TIQV-017
- RULE-EE-TIQV-018
- RULE-EE-TIQV-019
- RULE-EE-TIQV-020
- RULE-EE-TIQV-021
- RULE-EE-TIQV-022
- RULE-EE-TIQV-023
- RULE-EE-TIQV-024
- RULE-EE-TIQV-025
- RULE-EE-TIQV-026
- RULE-EE-TIQV-027
- RULE-EE-TIQV-028
- RULE-EE-TIQV-029

## Open questions
- Nessuna open question strutturale residua dentro il boundary di questo package al `2026-04-15`.
- Eventuali futuri aggiornamenti ARERA o AU potranno solo riaprire il package se introdurranno nuovi flussi materiali, non per il solo layer procedurale già chiuso dal TIQV.

## Stato avanzamento
- Coperti: intake, registri, classificazione prudenziale, call center, comunicazioni annuali ad ARERA, pubblicazioni annuali lato venditore o lato ARERA e reporting di misura verso SII e bolletta.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15. Restano solo futuri aggiornamenti materiali di ARERA o AU.

## Vedi anche
- [anagrafica-tecnica-pod-accessi-reporting.md](anagrafica-tecnica-pod-accessi-reporting.md)
- [qualita-commerciale-reclami.md](qualita-commerciale-reclami.md)
- [misure.md](misure.md)
- [fatturazione.md](fatturazione.md)
- [../MACRO/domestico-luce-reporting-regolatorio.md](../MACRO/domestico-luce-reporting-regolatorio.md)
- [../ROADMAP-DOMESTICO-LUCE-2026-04-15.md](../ROADMAP-DOMESTICO-LUCE-2026-04-15.md)
