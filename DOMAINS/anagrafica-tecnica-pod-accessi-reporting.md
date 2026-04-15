# Dominio: Anagrafica tecnica POD, accessi e reporting

## Perimetro attivo
- settore: energia elettrica
- segmento: clienti domestici
- data di riferimento SSOT: 2026-04-15
- focus: accesso cliente e operatore ai dati del punto, minima anagrafica tecnica del POD, boundary documentale tra cliente e venditore, disponibilità post-cessazione e reporting rilevante

## Scopo
Raccogliere il minimo riusabile e source-backed su come il POD e i relativi dati tecnici/anagrafici vengono identificati, consultati, aggiornati e resi visibili al cliente finale o agli operatori nel domestico elettrico.

## Copre
- base legale SII/RCU per punto e intestatario
- accesso gratuito del cliente ai propri dati di consumo
- Portale Consumi e limiti minimi rilevanti
- accesso di terze parti autorizzate dal cliente tramite Portale Consumi
- accesso operatori via PK e CDT
- aggiornamento RCU
- perimetro privacy minimo lato Portale Consumi e lato SII sui dati del cliente finale
- minima anagrafica tecnica customer-facing in bolletta
- accesso online a reclami e richieste di informazioni senza registrazione
- accesso post-cessazione all'area personale e all'archivio bollette o notifiche nel minimo TIQV
- pacchetto documentale minimo da allegare ai reclami sugli importi fatturati
- boundary tra documenti consegnati al cliente su supporto durevole e archivio online o retention interna del venditore
- obblighi TIQV di registrazione e reporting su reclami, richieste, rettifiche e call center
- boundary minimo di retention lato venditore fuori Portale Consumi
- obblighi minimi di reporting su letture, consumi e messa a disposizione al SII direttamente collegati al POD

## Fonti principali
### Primarie
- SRC-NORMATTIVA-DL-105-2010-ART1BIS
- SRC-GU-L-205-2017-ART1-C6-C8
- SRC-ARERA-BOLLETTA-2025-PDF
- SRC-ARERA-TIF-2025-PDF
- SRC-ARERA-TIME-2024-PDF
- SRC-ARERA-TIQV-2026-PDF
- SRC-ARERA-CCC24-PDF
- SRC-NORMATTIVA-DLGS-206-2005
- SRC-GU-CC-ART2220
- SRC-NORMATTIVA-DPR-600-1973-ART22
- SRC-NORMATTIVA-DPR-633-1972-ART39

### Ufficiali di supporto
- SRC-ARERA-PORTALE-CONSUMI-PAGE
- SRC-AU-PORTALE-CONSUMI-HOMEPAGE-PAGE
- SRC-AU-PORTALE-CONSUMI-TERZE-PARTI-PAGE
- SRC-AU-PORTALE-CONSUMI-PRIVACY-PAGE
- SRC-AU-SII-TRATTAMENTO-DATI-PERSONALI-PAGE
- SRC-SII-EE-INTERROGAZIONE-RCU-PAGE
- SRC-SII-EE-PRECHECK-SPEC-2019
- SRC-SII-EE-CDT-SPEC-2020
- SRC-SII-EE-POPOLAMENTO-RCU-PAGE
- SRC-SII-EE-AOC-RCU-2025

## Fatti consolidati
### Base dati e accesso cliente
- Il SII ha base legale in una banca dati dei punti di prelievo e dei dati identificativi dei clienti finali.
- La legge 205/2017 collega nello stesso perimetro: acquisizione dei dati effettivi di consumo, facoltà di incentivare l’autolettura senza oneri e diritto del cliente finale ad accedere ai propri dati di consumo tramite il SII senza oneri.
- L’implementazione customer-facing disponibile nel perimetro ufficiale è il Portale Consumi: accesso gratuito tramite SPID, profondità storica fino a 36 mesi, letture e autoletture, principali informazioni tecniche e contrattuali della fornitura, e per l’elettrico dettaglio fino al quartorario quando disponibile.
- La homepage ufficiale di Acquirente Unico rafforza questo boundary descrivendo il Portale Consumi come servizio gratuito previsto dalla legge per accedere alle informazioni sulle proprie utenze, in particolare `anagrafiche`, `contratti` e `misure`: il layer online customer-facing esiste quindi oltre il minimo TIQV, ma come self-service dati o informazioni della fornitura, non come archivio generale dei documenti del venditore.
- Dal 1 ottobre 2025 il Portale Consumi aggiunge un canale formale di accesso di terze parti: il cliente può autorizzare e revocare direttamente dal Portale l’accesso ai dati di consumo da parte di soggetti qualificati accreditati al SII, con finestra massima di 48 mesi intorno alla data di autorizzazione.

### Accesso operatore e aggiornamento RCU
- Sul lato operatori il SII separa la verifica anagrafica dal dato tecnico: PK verifica l’abbinamento fra POD e dati identificativi del cliente finale, mentre CDT espone i dati tecnici del POD.
- La specifica PK dettaglia che il venditore può interrogare l’associazione POD-cliente dopo la sottoscrizione del contratto, con tolleranza limitata sugli identificativi e con possibilità, in alcuni casi di maggior tutela, di integrare la richiesta con nome/cognome o ragione sociale.
- La stessa specifica PK mostra che, quando l’anagrafica fiscale manca ma la congruenza è verificata, il SII può aggiornare il RCU e notificare l’integrazione al distributore tramite PK2.
- Il RCU non è aggiornato con una scrittura generica: il portale SII elenca processi dedicati, tra cui VS, AE, SM/RT, DS, AV, VP, TDE e CP.
- La specifica pubblica `Aggiornamento On Condition RCU` aggiunge la catena operativa post-esecuzione: dopo l'ammissibilità del flusso VS1 il SII aggiorna il RCU entro 1 giorno lavorativo e notifica la nuova attivazione alla controparte commerciale tramite `VS2.0200`.
- Dopo la notifica di attivazione, l'UDD deve integrare entro 3 giorni i dati RCU di propria competenza tramite `VS2.0201`; se il flusso non viene inviato, la CC abbinata deve trasmettere gli stessi dati tramite `AE1.0050`.

### Minima anagrafica tecnica del POD
- Lato operatore, la minima anagrafica tecnica estraibile con fonte ufficiale oggi consolidata comprende almeno: tipologia di misuratore, trattamento del punto ai sensi del TIS, data di messa a regime del misuratore 2G e stato di attivazione del POD.
- Lato cliente, la bolletta sintetica deve riportare almeno i dati identificativi del punto, cioè indirizzo del punto, codice POD e potenza impegnata.
- Negli Elementi informativi essenziali della stessa bolletta devono comparire, per il settore elettrico, la tipologia di cliente e la tensione nominale di alimentazione.

### Obblighi minimi di reporting direttamente rilevanti
- Il TIME impone che i dati di misura siano messi a disposizione del SII con tempi regolati e con qualificazione del dato come effettivo, autolettura o stimato; per i misuratori 2G messi a regime la disponibilità è giornaliera.
- Il TIF e la disciplina della bolletta impongono al venditore di mostrare separatamente letture, autoletture, letture stimate, consumi effettivi, consumi stimati e consumi fatturati, oltre alla finestra di autolettura nei casi previsti e all’avviso di possibile ricalcolo quando si usano dati stimati.
- Il TIQV impone di registrare per ogni chiamata pervenuta al call center i dati necessari a rendere verificabili almeno TMA, LS e AS e, sopra la soglia di 50.000 clienti finali TIQV al 31 dicembre, di comunicare ad ARERA entro il 28 febbraio i dati mensili dell’anno precedente su chiamate e indicatori del call center.
- Lo stesso TIQV chiude anche la logica di intake e reporting delle pratiche: reclami scritti e richieste scritte di informazioni vanno classificati secondo la tabella A con criteri prudenziali, trattando come reclamo ogni caso dubbio prima e indipendentemente dal merito.
- Il TIQV impone inoltre di mantenere un registro verificabile di reclami scritti, richieste scritte di informazioni, rettifiche di fatturazione e doppia fatturazione, con classificazione, POD o PDR, date rilevanti, eventuali cause di mancato rispetto e indennizzi; la relativa documentazione deve restare ordinata, accessibile e verificabile per almeno 3 anni solari successivi alla registrazione.
- Entro il 28 febbraio il venditore comunica ad ARERA i dati annuali su volumi, esiti, cause di mancato rispetto, tempi medi, pratiche ancora aperte e indennizzi, e entro il 30 giugno pubblica sul proprio sito standard, indennizzi e performance annuali.
- Il layer ARERA non si esaurisce nella comunicazione annuale: il TIQV prevede anche indagini annuali selettive su call center e risposte ai reclami, nonché pubblicazione annuale ARERA di dati su qualità telefonica e qualità commerciale, anche con logiche comparative.

### Accesso documentale lato venditore e disponibilità post-cessazione
- Il TIQV impone che il sito del venditore, nella pagina dei canali di contatto, metta a disposizione una funzionalità che consenta di inviare reclami scritti o richieste di informazioni anche senza necessità di registrazione, con ricevuta che attesti data di invio e codice pratica.
- Se il venditore offre un’area personale, il TIQV impone una funzionalità di invio semplificato che consenta di selezionare la fornitura interessata e di scaricare la copia della comunicazione inviata.
- Se il venditore offre un’area personale online, il TIQV impone che dopo la cessazione il cliente possa continuare ad accedervi per almeno 6 mesi, almeno per reclami, richieste di informazioni, archivio delle bollette emesse e archivio delle notifiche.
- Quando il reclamo riguarda importi fatturati, la risposta motivata deve allegare gli `Elementi di dettaglio` della bolletta e, nel mercato libero, anche la `Scheda sintetica` dell’offerta e gli eventuali preavvisi rilevanti su variazioni unilaterali, evoluzioni automatiche o rinnovi con modifica delle condizioni economiche.
- Sul lato cliente, il corpus primario già verificato chiude ora anche il boundary dei documenti customer-facing ulteriori rispetto a bollette, notifiche e allegati reclamo: CCC24 e Codice del consumo impongono che copia del contratto e, nei casi previsti, `Scheda sintetica` o conferma contrattuale siano consegnate o trasmesse su supporto cartaceo o altro mezzo durevole; questa disponibilità documentale resta diversa da un archivio online generalizzato del venditore dopo la cessazione.

### Privacy minima e limiti di accesso
- L’informativa privacy del Portale Consumi chiarisce che il trattamento riguarda almeno dati identificativi del cliente, POD o PDR, indirizzi di ubicazione, misure dei consumi e tracciatura degli accessi, con conservazione dichiarata non oltre 36 mesi dalla data cui i dati si riferiscono.
- La stessa informativa riconosce almeno accesso, portabilità, rettifica e opposizione, distinguendo la rettifica di nome e cognome, da chiedere all’Identity Provider, dagli altri dati per cui Acquirente Unico indirizza verso i soggetti competenti.
- La politica privacy del SII chiarisce che i dati personali dei clienti finali scambiati tra Utenti e Gestore sono usati esclusivamente per i processi del SII e non per ricerche di mercato, promozione, pubblicità o vendita diretta; al cliente resta inoltre la possibilità di chiedere verifica e correzione delle informazioni che lo riguardano.

### Retention lato venditore fuori Portale Consumi
- Sul piano civilistico generale, l’articolo 2220 c.c. impone di conservare per dieci anni dalla data dell’ultima registrazione le scritture contabili e, per lo stesso periodo, fatture e corrispondenza rilevante; la conservazione può avvenire anche su supporti di immagini purché leggibili.
- Sul piano fiscale, l’articolo 22 del DPR 600/1973 impone di conservare le scritture obbligatorie fino a quando non siano definiti gli accertamenti del corrispondente periodo d’imposta, anche oltre il termine dell’articolo 2220 c.c., e fino allo stesso termine anche le fatture ricevute ed emesse e la corrispondenza rilevante per ciascun affare.
- L’articolo 39 del DPR 633/1972 coordina la conservazione IVA di registri, fatture e altri documenti con l’articolo 22 del DPR 600/1973, impone la conservazione elettronica delle fatture elettroniche e richiede, per finalità di controllo, accesso automatizzato all’archivio e documenti stampabili e trasferibili su altro supporto informatico.
- Il boundary SSOT ora è netto: Portale Consumi copre online dati e informazioni della fornitura entro i propri limiti, il TIQV copre il minimo di area personale e di allegati documentali nel reclamo billing, CCC24 e Codice del consumo coprono le copie customer-side su supporto durevole, mentre articolo 2220 c.c., DPR 600/1973 articolo 22 e DPR 633/1972 articolo 39 chiudono la retention legale lato venditore senza trasformarla in un diritto generale di archivio online del cliente.

## Evidenze estratte
- `EXTRACTED/SRC-NORMATTIVA-DL-105-2010-ART1BIS.extracted.md`
- `EXTRACTED/SRC-GU-L-205-2017-ART1-C6-C8.extracted.md`
- `EXTRACTED/SRC-ARERA-PORTALE-CONSUMI-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-PORTALE-CONSUMI-HOMEPAGE-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-PORTALE-CONSUMI-TERZE-PARTI-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-PORTALE-CONSUMI-PRIVACY-PAGE.extracted.md`
- `EXTRACTED/SRC-AU-SII-TRATTAMENTO-DATI-PERSONALI-PAGE.extracted.md`
- `EXTRACTED/SRC-SII-EE-INTERROGAZIONE-RCU-PAGE.extracted.md`
- `EXTRACTED/SRC-SII-EE-PRECHECK-SPEC-2019.extracted.md`
- `EXTRACTED/SRC-SII-EE-CDT-SPEC-2020.extracted.md`
- `EXTRACTED/SRC-SII-EE-POPOLAMENTO-RCU-PAGE.extracted.md`
- `EXTRACTED/SRC-SII-EE-AOC-RCU-2025.extracted.md`
- `EXTRACTED/SRC-ARERA-BOLLETTA-2025-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIF-2025-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIME-2024-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIQV-2026-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-CCC24-PDF.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DLGS-206-2005.extracted.md`
- `EXTRACTED/SRC-GU-CC-ART2220.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DPR-600-1973-ART22.extracted.md`
- `EXTRACTED/SRC-NORMATTIVA-DPR-633-1972-ART39.extracted.md`

## Regole collegate
- RULE-EE-RCU-001
- RULE-EE-RCU-002
- RULE-EE-RCU-003
- RULE-EE-RCU-004
- RULE-EE-RCU-005
- RULE-EE-TIF-003
- RULE-EE-TIME-003
- RULE-EE-BOLL-001
- RULE-EE-POD-001
- RULE-EE-POD-002
- RULE-EE-POD-003
- RULE-EE-POD-004
- RULE-EE-POD-005
- RULE-EE-POD-006
- RULE-EE-POD-007
- RULE-EE-POD-008
- RULE-EE-POD-009
- RULE-EE-POD-010
- RULE-EE-POD-011
- RULE-EE-POD-014
- RULE-EE-POD-012
- RULE-EE-POD-013
- RULE-EE-CCC24-003
- RULE-EE-CDCONS-001
- RULE-EE-TIQV-007
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

## Open questions
- Non resta un'open question SSOT attiva sul boundary documentale o di availability di questo slice: il repo separa ora in modo source-backed documenti su supporto durevole, minimo di area personale TIQV e layer online data-centric del Portale Consumi.
- La mancanza di una fonte primaria unica ed esaustiva su tutti i campi della "anagrafica tecnica POD" non è più un gap aperto: il boundary chiuso resta il set minimo customer-facing di `RULE-EE-POD-007` e il set minimo operator-facing di `RULE-EE-POD-005`, salvo futura fonte ufficiale che ampli il perimetro.
- Nel corpus ufficiale verificato al `2026-04-15` non emerge una fonte customer-facing vigente che renda obbligatoria, per l'ordinario domestico, l'esposizione uniforme di ulteriori dati tecnici del punto o del contatore come matricola, potenza disponibile o altri campi oltre il minimo già consolidato; riaprire solo se emergerà un atto ARERA/AU/SII più specifico.

## Stato avanzamento
- Coperti: set minimo customer-facing e operator-facing del POD, accesso cliente e terze parti ai dati, boundary tra Portale Consumi, area personale TIQV, documenti su supporto durevole, retention lato venditore e reporting minimo collegato al punto.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15. Restano solo futuri ampliamenti ufficiali di ARERA, AU o SII che dovessero espandere il perimetro.

## Vedi anche
- [reporting-regolatorio.md](reporting-regolatorio.md)
- [attori-mercato.md](attori-mercato.md)
- [misure.md](misure.md)
- [fatturazione.md](fatturazione.md)
- [../OPEN-QUESTIONS.md](../OPEN-QUESTIONS.md)
