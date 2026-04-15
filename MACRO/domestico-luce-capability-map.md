# Macro, capability map domestico luce (ponte verso SUPER)

Snapshot SSOT: 2026-04-15

## Scopo
Questa nota riorganizza il repo `energia-ssot` come mappa di capability per uso prodotto. Non aggiunge fatti nuovi. Usa solo materiale già chiuso o chiaramente delimitato nel repo e lo traduce in tre domande pratiche:
- cosa il prodotto può `sapere`
- cosa il prodotto può `fare`
- cosa il prodotto può `decidere` con guardrail chiari

## Regola di separazione
### Layer normativo SSOT
- Vale solo ciò che è già chiuso o dichiarato come baseline nel repo, soprattutto in `DOMAINS/`, `RULES/`, `EXTRACTED/` e `CITATIONS/`.
- Se una regola è ancora aperta o solo parziale, qui resta marcata come boundary o gap.

### Layer di interpretazione prodotto
- Traduce il perimetro SSOT in capability operative riusabili per `SUPER` o per altri layer prodotto.
- Non crea nuove regole normative.
- Non sostituisce una `DECISION` di prodotto. Se bisogna scegliere UX copy, policy interna, fallback o automazioni più spinte, va aperta una decisione separata in `DECISIONS/`.

## Oggetti minimi già modellabili dal repo
Questa è una lettura prodotto, non normativa.
- `cliente_domestico`, con segmentazione minima `vulnerabile / non_vulnerabile`
- `regime_servizio`, almeno `mercato_libero / maggior_tutela / STG` nei boundary chiusi del repo
- `POD`, con set minimo customer-facing e operator-facing già consolidato
- `offerta_contratto`, con documenti, corrispettivi e regole di rinnovo/modifica nei limiti SSOT
- `processo_fornitura`, almeno `switching / voltura / subentro / disattivazione / attivazione`
- `dato_misura` e `dato_fatturato`, con ordine d'uso e tracciabilità minima
- `pagamento_garanzia_rateizzazione`
- `evento_morosita`, con stati di mora, sospensione, riattivazione e raccordo con `CMOR`
- `pratica_supporto_compliance`, con reclami, richieste, SLA, indennizzi, registri e reporting minimo

Nota: il repo non impone ancora un modello dati unico o un vocabolario applicativo finale. Impone però un perimetro minimo di oggetti e relazioni già sufficientemente stabile per un bridge prodotto.

## Capability map

### 1. Onboarding e segmentazione iniziale
#### Baseline normativa già chiusa nel repo
- Il repo distingue cliente domestico `vulnerabile` e `non vulnerabile` e collega i regimi di servizio rilevanti tramite `DOMAINS/tutele-graduali.md` e `DOMAINS/attori-mercato.md`.
- Il repo chiude il ruolo del `SII`, del `RCU`, del venditore, del distributore, della controparte commerciale e dell'`UdD` nel minimo necessario a classificare i processi rilevanti.
- Il repo chiude il requisito del titolo sull'immobile per `stipulazione`, `voltura` e `rinnovo`, con esclusione dello `switching puro`.
- Il repo chiude la disclosure minima precontrattuale e contrattuale su documenti, frequenza di fatturazione, pagamenti, garanzie e ripensamento.

#### Interpretazione prodotto
**SUPER può sapere**
- se il caso ricade nel perimetro `vulnerabile / non vulnerabile`
- quale regime di servizio è normativamente rilevante nel baseline del repo
- se il caso dichiarato dal cliente assomiglia a `switching`, `voltura`, `subentro`, `attivazione` o `disattivazione`
- se il titolo immobile è normativamente richiesto oppure no
- quali documenti minimi il cliente deve ricevere o poter consultare

**SUPER può fare**
- guidare un intake iniziale con domande di classificazione affidabili
- mostrare documenti e disclosure minime coerenti con il perimetro SSOT
- instradare il journey corretto prima di entrare nei flussi specialistici

**SUPER può decidere**
- quando bloccare un intake che confonde `switching` con `voltura` o `subentro`
- quando chiedere il titolo immobile e quando non chiederlo
- quando il caso va trattato come percorso libero, tutela o STG nel perimetro già chiuso

**Boundary da non superare**
- la vista editoriale unica della segmentazione esiste ora in `MACRO/domestico-luce-segmentazione-regimi.md`, ma non sostituisce le fonti dominio o le future decisioni prodotto
- non esiste ancora una decisione prodotto registrata su UX, copy o policy di intake

### 2. Contratti, offerte e trasparenza commerciale
#### Baseline normativa già chiusa nel repo
- `DOMAINS/contratti-offerte-trasparenza.md` chiude `Scheda sintetica`, contenuti minimi del contratto, supporto durevole, diritto di ripensamento, preavvisi, rinnovi, modifiche unilaterali, PLACET e boundary dell'onere di recesso anticipato.
- Il repo chiude anche il layer 2026 di disclosure domestica del libero, inclusi bucket dei corrispettivi, offerte onnicomprensive, siti venditore e rapporto con Portale Offerte.

#### Interpretazione prodotto
**SUPER può sapere**
- quali campi documentali e informativi devono comparire in `Scheda sintetica` e contratto
- quando scatta il ripensamento del consumatore e quando si parla invece di recesso ordinario o recesso anticipato con onere ammesso
- se un'offerta ricade nel perimetro `PLACET`, `libero non onnicomprensivo` o `onnicomprensivo`
- quali disclosure sul recesso devono restare separate dalla spesa annua stimata

**SUPER può fare**
- validare checklist documentali e precontrattuali
- rendere leggibile il boundary tra ripensamento, cambio fornitore e onere di recesso anticipato
- separare nel packaging offerta i layer `corrispettivi`, `sconti/bonus`, `servizi aggiuntivi`, `recesso`

**SUPER può decidere**
- se una disclosure è obbligatoria, opzionale o fuori perimetro SSOT
- se un onere di recesso anticipato può essere rappresentato solo come presenza separata e non come voce della spesa annua stimata
- se un'offerta richiede trattamento `generalizzato`, `non generalizzato` o `comparabilità derogatoria` nel perimetro già descritto dal repo

**Boundary da non superare**
- il repo non autorizza formule commerciali cross-vendor oltre quelle chiuse da ARERA
- clausole commerciali specifiche del singolo venditore non vanno trasformate in regola SSOT generale

### 3. Pricing e architettura economica
#### Baseline normativa già chiusa nel repo
- `DOMAINS/prezzi-oneri-componenti.md` chiude i bucket customer-facing della Bolletta 2025, la distinzione tra `Scontrino`, `Box dell'offerta`, `Elementi di dettaglio` e `Glossario`, e le componenti regolatorie minime per `maggior tutela` e `STG`.
- Il repo chiude anche il boundary strutturale del libero domestico, incluse offerte non onnicomprensive, onnicomprensive, trattamento del dispacciamento, eccezione oraria e rapporto con Portale Offerte.
- Fiscalità domestica elettrica minima è chiusa nel repo tramite accisa e IVA ed è ora separata anche nel dominio `DOMAINS/fiscalita.md`.

#### Interpretazione prodotto
**SUPER può sapere**
- quali bucket economici possono essere mostrati con nomenclatura regolatoria vigente
- quali componenti sono ricostruibili in modo rigoroso per `MT` e `STG`
- che nel libero esiste una `architettura regolata della disclosure`, ma non una formula numerica unica cross-vendor
- quando imposte, bonus, ricalcoli o altre partite vanno tenuti separati dai bucket principali

**SUPER può fare**
- costruire un layer di pricing spiegabile e coerente con la bolletta 2025
- separare prezzo medio sintetico, corrispettivi puntuali e glossario
- confrontare correttamente ciò che è confrontabile e marcare ciò che resta solo descrittivo

**SUPER può decidere**
- quale livello informativo usare per una UX specifica, `bucket sintetico`, `dettaglio`, `glossario`, senza confonderli
- quando il prezzo è `regolato e scomponibile` e quando è solo `strutturalmente descrivibile`
- quando un alias legacy è ammissibile come supporto esplicativo e quando va mantenuto il label Bolletta 2025

**Boundary da non superare**
- non si può costruire una formula unica del mercato libero che ARERA non ha imposto
- il dominio `fiscalita` chiude il baseline fiscale domestico di base, ma non estende il repo a casistiche extra-perimetro o business

### 4. Billing e documenti di fatturazione
#### Baseline normativa già chiusa nel repo
- `DOMAINS/fatturazione.md` chiude frequenza bimestrale domestica, termine ordinario di emissione entro 45 giorni, ordine d'uso tra dato effettivo, autolettura validata e stima, bolletta di chiusura, prescrizione biennale, ricalcoli, `Elementi di dettaglio`, pacchetto documentale minimo dei reclami e archivio post-cessazione nel minimo TIQV.
- `MACRO/domestico-luce-billing-misure.md` rende già leggibile il tratto misura → fattura.

#### Interpretazione prodotto
**SUPER può sapere**
- quando una fattura è di periodo, di chiusura, di rettifica o di doppia fatturazione
- quale dato di misura ha priorità normativa
- quando un conguaglio o una contestazione entra nel perimetro prescrizione o nel perimetro delle cause ostative
- quali allegati sono minimi in una risposta a reclamo su importi fatturati

**SUPER può fare**
- spiegare in modo coerente perché una fattura usa dato effettivo, autolettura o stima
- generare checklist di controllo della bolletta 2025 e dei relativi allegati
- separare archivio cliente, supporto durevole e retention interna del venditore

**SUPER può decidere**
- quando un caso va instradato verso `rettifica`, `reclamo importi fatturati`, `prescrizione`, `chiusura`
- quando un credito deve restare in compensazione e quando il TIQV impone `rimessa diretta`
- quando il venditore può parlare di archivio online minimo e quando no

**Boundary da non superare**
- il repo non autorizza a generalizzare diritti retail uniformi extra-standard del libero non `PLACET`
- la retention legale lato venditore non coincide con un diritto generale del cliente a un archivio online esteso

### 5. Pagamenti, garanzie e rateizzazioni
#### Baseline normativa già chiusa nel repo
- `DOMAINS/pagamenti-garanzie-rateizzazioni.md` chiude metodi di pagamento, termini minimi, deposito cauzionale, domiciliazione, sconto PLACET per e-bill + domiciliazione, rateizzazione regolata in `MT`, `PLACET` e `STG`, rinvio uniforme del libero ai casi di periodicità mancata o importi anomali, accrediti TIQV e restituzione del deposito in chiusura.

#### Interpretazione prodotto
**SUPER può sapere**
- quali canali di pagamento e garanzie devono essere esposti in documenti e contratto
- quando il deposito è ammesso, esente o equivalente alla domiciliazione
- in quali casi il cliente ha diritto a rateizzazione regolata uniforme
- quando un accredito va trattato come compensazione oppure come rimessa diretta

**SUPER può fare**
- validare offerte e contratti lato pagamenti e garanzie
- spiegare al cliente se una richiesta di rateizzazione ricade in un caso regolato o in sola pattuizione contrattuale
- gestire il boundary tra regole uniformi e condizioni vendor-specific

**SUPER può decidere**
- se una richiesta di rateizzazione entra nel perimetro regolato o va classificata come extra-standard
- se un deposito può essere richiesto o va disapplicato per domiciliazione
- se una promessa commerciale è rappresentabile come diritto SSOT oppure no

**Boundary da non superare**
- oltre i casi chiusi nel repo, il libero non `PLACET` non ha ulteriori diritti uniformi da assumere come baseline SSOT

### 6. Morosità, sospensione, riattivazione e CMOR
#### Baseline normativa già chiusa nel repo
- `DOMAINS/morosita-cmor.md` chiude costituzione in mora, termini minimi, riduzione di potenza, sospensione, riattivazione, indennizzi automatici, interruzione fisica ex articolo 9 TIMOE, effetti dell'articolo 9bis, clienti non disalimentabili, raccordo con i servizi di ultima istanza e flusso `CMOR`.
- `MACRO/domestico-luce-morosita-pagamenti.md` già sintetizza il baseline customer-facing principale.

#### Interpretazione prodotto
**SUPER può sapere**
- in che stato del ciclo morosità si trova il cliente, `mora`, `riduzione potenza`, `sospensione`, `interruzione fisica`, `riattivazione`, `CMOR`
- quali termini minimi e quali indennizzi automatici sono rilevanti
- quando il cliente è `non disalimentabile` e va instradato sul percorso speciale
- quando il ritorno alla fornitura è una semplice riattivazione e quando serve una nuova attivazione

**SUPER può fare**
- spiegare i passaggi obbligatori prima della sospensione
- controllare il rispetto del flusso post-pagamento e dei tempi di riattivazione
- separare il recupero credito retail ordinario dal meccanismo di sistema `CMOR`

**SUPER può decidere**
- quando un'azione di sospensione sarebbe prematura o fuori regola
- quando il caso ricade nella disciplina speciale di non disalimentabilità o ultima istanza
- quando il costo è numericamente standardizzato e quando resta solo `costo effettivo` senza tariffario uniforme

**Boundary da non superare**
- sul comma `24.3` TIMOE resta solo una nota redazionale di monitoraggio rispetto al routing STG già chiuso dal TIV 2026
- per l'interruzione fisica ex articolo 9 il boundary SSOT è chiuso sul rinvio ai costi effettivi, non su un tariffario customer-facing uniforme ARERA

### 7. Switching, voltura, subentro, cessazione e prima attivazione
#### Baseline normativa già chiusa nel repo
- `DOMAINS/switching.md` chiude il baseline vigente al 2026-04-15 sul cambio fornitore su punto attivo, inclusa la separazione rispetto a `RC/UI` e la non applicabilità anticipata della riforma switching 24h.
- `DOMAINS/voltura-subentro-cessazione.md` chiude voltura, subentro, disattivazione, nuova connessione o prima attivazione con preventivo o lavori, costi TIC correnti, routing venditore/distributore, stati POD nel RCU e precedenze tra pratiche.

#### Interpretazione prodotto
**SUPER può sapere**
- se il POD è da trattare come `attivo`, `disattivo`, `da allacciare`, `in disattivazione`, `sospeso per morosità`
- quale journey corretto si applica, `switching`, `voltura`, `subentro`, `disattivazione`, `allacciamento con attivazione`
- quali tempi customer-facing sono quelli giusti, evitando di usare i 5 giorni dell'attivazione standard nei casi di lavori o preventivo
- quali costi sono regolati e quali dipendono dal contratto

**SUPER può fare**
- guidare il routing corretto tra venditore, distributore e processi SII
- prevenire intake errati su `prima attivazione`, che spesso nascondono `subentro` o `allacciamento`
- spiegare differenza tra cessazione con disattivazione, cessazione senza disattivazione e switching puro

**SUPER può decidere**
- se il titolo immobile è richiesto
- se una pratica è compatibile o incompatibile con una disattivazione imminente
- quando il caso resta in switching e quando esce verso attivazione o cessazione

**Boundary da non superare**
- lo switching reseller a 24 ore è roadmap regolatoria approvata ma non ancora efficace al 2026-04-15
- eventuali estensioni A→Z su temporanee, MT o casi infrastrutturali speciali restano fuori scope

### 8. Misure, letture, consumi e profiling minimo
#### Baseline normativa già chiusa nel repo
- `DOMAINS/misure.md`, `DOMAINS/fatturazione.md` e `DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md` chiudono il pacchetto customer-facing `TIME/TIF + Portale Consumi` nel perimetro già consolidato del repo.
- Il repo chiude ordine d'uso del dato, disponibilità dei dati al SII, letture/autoletture/stime, ricalcoli da rettifica e accesso storico cliente ai consumi.

#### Interpretazione prodotto
**SUPER può sapere**
- il tipo logico del dato usato, `effettivo`, `autolettura validata`, `stimato`
- quando il cliente può vedere dati storici e a quale profondità minima nel Portale Consumi
- quando una rettifica di misura può propagarsi in fatturazione
- quali dati quartorari esistono solo `quando disponibili`

**SUPER può fare**
- rendere spiegabile il percorso dal dato di misura alla fattura
- mostrare al cliente quali dati sono già definitivi e quali restano suscettibili di ricalcolo
- instradare richieste di ricostruzione, verifica o contestazione senza confondere misura e billing

**SUPER può decidere**
- quando il billing può usare un dato effettivo, quando può usare autolettura validata e quando resta una stima
- quando una spiegazione al cliente deve stare nel dominio misura e quando nel dominio fatturazione

**Boundary da non superare**
- il repo non chiude ancora un'estensione ampia sui temi 2G oltre il slice customer-facing già consolidato

### 9. Dati, accesso, privacy e retention
#### Baseline normativa già chiusa nel repo
- `DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md` chiude accesso cliente ai dati via SII/Portale Consumi, accesso di terze parti autorizzate, set minimo customer-facing e operator-facing del POD, privacy minima Portale/SII, accesso documentale TIQV, disponibilità post-cessazione, copie cliente su supporto durevole e retention legale lato venditore.

#### Interpretazione prodotto
**SUPER può sapere**
- quali dati il cliente può consultare direttamente, quali terze parti possono vedere previa autorizzazione e quali dati restano lato operatore
- il perimetro minimo dei dati POD esponibili lato cliente e lato operatore
- quali retention sono `customer-facing`, quali sono `legali interne`, quali sono proprie del Portale Consumi

**SUPER può fare**
- costruire policy di accesso e disponibilità documentale coerenti con SSOT
- distinguere tra archivio online, documenti su supporto durevole e archivi interni per controlli
- spiegare correttamente privacy e limiti d'uso dei dati SII/Portale

**SUPER può decidere**
- se una richiesta dati può essere soddisfatta in self-service, tramite autorizzazione terza parte, oppure solo come richiesta assistita
- se un dato rientra nel set minimo esponibile o se manca base SSOT per mostrarlo stabilmente
- se una retention promessa al cliente è supportata oppure eccede il minimo normativo chiuso

**Boundary da non superare**
- il repo non ha ancora una fonte primaria unica ed esaustiva su tutti i campi della anagrafica tecnica POD
- restano da verificare solo eventuali atti ARERA ulteriori sui layer richiamati dal TIQV

### 10. Supporto, reclami e compliance operativa
#### Baseline normativa già chiusa nel repo
- `DOMAINS/reporting-regolatorio.md` unifica ora in un package dedicato il layer end-to-end su intake senza registrazione, area personale minima, registri, call center, comunicazioni annuali ad ARERA, pubblicazioni annuali e reporting di misura, usando solo materiale già chiuso nel repo.
- `DOMAINS/qualita-commerciale-reclami.md` resta la fonte di dettaglio per SLA reclami e richieste, indennizzi automatici, classificazione prudenziale, tabella A, registri, verificabilità, retention minima triennale, call center, comunicazioni annuali ad ARERA e pubblicazioni annuali.
- Il repo collega questo dominio con billing, morosità, dati accesso e pagamenti.

#### Interpretazione prodotto
**SUPER può sapere**
- se un contatto va trattato come `reclamo` o `richiesta di informazioni`
- a quale bucket regolatorio appartiene la pratica
- quali date, cause di mancato rispetto e indennizzi devono essere registrati
- quali obblighi di reporting o pubblicazione derivano dalla pratica o dal perimetro annuale

**SUPER può fare**
- classificare intake e ticket con tassonomia coerente con il TIQV
- orchestrare la raccolta dei campi minimi di audit trail
- collegare una pratica a fatturazione, misura, morosità, contratto o bonus senza perdere il bucket regolatorio

**SUPER può decidere**
- quando, in dubbio, trattare il caso come reclamo e non come semplice richiesta
- quando scatta un indennizzo automatico o una verifica di SLA
- quali allegati e quali evidenze devono entrare nella risposta

**Boundary da non superare**
- il repo non incorpora ancora eventuali determinazioni ARERA ulteriori richiamate dal TIQV se non già esplicitamente verificate

## Sintesi capability-oriented per SUPER
Questa è ancora interpretazione prodotto, non normativa.

### Cosa è già abbastanza stabile per diventare capability di piattaforma
- `classificazione dei journey`, onboarding, switching, voltura, subentro, disattivazione, prima attivazione
- `segmentazione regolatoria minima`, vulnerabile/non vulnerabile e relativo regime di servizio nel perimetro chiuso
- `explainability economica`, bucket bolletta, layer di pricing, MT/STG, boundary del libero
- `billing intelligence`, uso del dato misura, ricalcoli, prescrizione, allegati, archivio minimo
- `guardrail pagamenti e recupero credito`, pagamenti, garanzie, rateizzazione, mora, riattivazione, CMOR
- `guardrail accesso dati`, Portale Consumi, terze parti autorizzate, boundary retention/privacy
- `ops supporto/compliance`, intake, classificazione TIQV, SLA, indennizzi, reporting minimo

### Cosa resta fuori dalle capability SSOT senza ulteriori decisioni o nuove fonti
- un modello dati esaustivo della anagrafica tecnica POD oltre il minimo già consolidato
- una formula numerica unica del mercato libero domestico cross-vendor
- un tariffario uniforme ARERA per il costo customer-facing dell'interruzione fisica ex articolo 9 TIMOE
- policy prodotto su UX, automazioni, fallback o copy finale, perché il repo `DECISIONS/` è ancora non avviato

## Dove approfondire nel repo
- [../ROADMAP-DOMESTICO-LUCE-2026-04-15.md](../ROADMAP-DOMESTICO-LUCE-2026-04-15.md)
- [../DOMAINS/attori-mercato.md](../DOMAINS/attori-mercato.md)
- [../DOMAINS/tutele-graduali.md](../DOMAINS/tutele-graduali.md)
- [../DOMAINS/contratti-offerte-trasparenza.md](../DOMAINS/contratti-offerte-trasparenza.md)
- [../DOMAINS/prezzi-oneri-componenti.md](../DOMAINS/prezzi-oneri-componenti.md)
- [../DOMAINS/fiscalita.md](../DOMAINS/fiscalita.md)
- [../DOMAINS/fatturazione.md](../DOMAINS/fatturazione.md)
- [../DOMAINS/pagamenti-garanzie-rateizzazioni.md](../DOMAINS/pagamenti-garanzie-rateizzazioni.md)
- [../DOMAINS/morosita-cmor.md](../DOMAINS/morosita-cmor.md)
- [../DOMAINS/switching.md](../DOMAINS/switching.md)
- [../DOMAINS/voltura-subentro-cessazione.md](../DOMAINS/voltura-subentro-cessazione.md)
- [../DOMAINS/misure.md](../DOMAINS/misure.md)
- [../DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md](../DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md)
- [../DOMAINS/qualita-commerciale-reclami.md](../DOMAINS/qualita-commerciale-reclami.md)
- [../DOMAINS/reporting-regolatorio.md](../DOMAINS/reporting-regolatorio.md)
- [../OPEN-QUESTIONS.md](../OPEN-QUESTIONS.md)

## Limiti strutturali da mantenere espliciti
- assenza di un modello dati esaustivo della anagrafica tecnica POD oltre il minimo già consolidato
- assenza di una formula numerica unica del mercato libero domestico cross-vendor
- assenza di un tariffario uniforme ARERA per il costo customer-facing dell'interruzione fisica ex articolo 9, con boundary SSOT già chiuso sul rinvio ai costi effettivi
