# Master, luce domestica: baseline SSOT finale al 2026-04-15

Snapshot SSOT: 2026-04-15

## Scopo
Questo documento riunisce in un solo testo leggibile il baseline domestico elettrico già chiuso nel repo, senza aggiungere fonti nuove e senza trasformare in fatti eventuali estensioni future fuori boundary.

## Perimetro
- settore: energia elettrica, clienti domestici in Italia
- taglio: sintesi di settore, customer-facing e operativo
- fonti: solo materiale ufficiale già consolidato in `DOMAINS/`, `RULES/`, `EXTRACTED/` e `CITATIONS/`
- esclusioni: nessuna formula numerica unica del mercato libero cross-vendor, nessuna generalizzazione di clausole commerciali vendor-specific, nessuna estensione A→Z oltre i boundary già chiusi nel repo

## Stato sintetico
Al `2026-04-15` il repo consente una lettura finale del domestico luce su prezzi, fiscalità, bonus e vulnerabili, contratti e trasparenza, switching e voltura, subentro e cessazione, boundary della prima attivazione domestica BT, billing e misure, pagamenti e morosità, dati e accessi, reporting minimo e qualità documentale collegata. Dentro questo perimetro non resta più alcuna open question SSOT attiva: i boundary rilevanti sono chiusi e i follow-up residui sono solo di monitoraggio futuro o manutenzione editoriale.

## 1) Regimi di servizio e segmentazione minima
Il baseline cross-domain usato nel repo è ormai chiuso come baseline composita ufficiale: `TIV` per regimi di servizio e vendita di ultima istanza, `DL 19/2025` e `ARERA 110/2025/R/eel` per il quadro transitorio rilevante, `ARERA 96/2026/R/eel` come checkpoint vigente del trimestre, `TIT` per rete e `TIDE` per dispacciamento quando servono nel raccordo economico. Nel perimetro domestico vanno tenuti distinti almeno `clienti vulnerabili`, `clienti non vulnerabili in STG`, `clienti nel mercato libero` e, nelle more del servizio vulnerabili aggiudicato, il presidio della `maggior tutela` per i vulnerabili.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-GU-DL-19-2025-ART2`
- `SRC-ARERA-110-25-PDF`
- `SRC-ARERA-96-26-PAGE`
- `SRC-ARERA-TIT-2024-2027-PDF`
- `SRC-ARERA-TIDE-REV4-2025-PDF`
- `SRC-NORMATTIVA-DLGS-210-2021-ART11`

## 2) Prezzi, componenti e struttura economica customer-facing
Dal 2025 la bolletta elettrica lato cliente aggrega gli importi almeno in quattro aree leggibili: `Spesa per la vendita di energia elettrica`, `Spesa per la tariffa per l'uso della rete elettrica`, `Spesa per gli oneri generali di sistema`, `imposte`. Nel repo restano distinti anche i tre layer documentali `Bolletta sintetica`, `Elementi di dettaglio`, `Glossario bolletta`.

Nel perimetro regolato già chiuso nel repo:
- la `Spesa per la vendita di energia elettrica` può includere approvvigionamento, commercializzazione, dispacciamento, sconti e altri importi contrattuali di vendita
- la macro-voce rete, per il domestico nel perimetro TIV consolidato, è riconducibile a `σ1`, `σ2`, `σ3`, `UC3`, `UC6`
- gli oneri generali di sistema sono rappresentabili lato cliente con `ARIM` e `ASOS`
- in maggior tutela domestica la rappresentazione minima chiusa è `PE + PD + PPE` sulla quota consumi e `PCV + DISPBT` sulla quota fissa per `POD/anno`
- in `STG` domestico non vulnerabile la rappresentazione minima chiusa è `CELD + CDISPD + CSED + CPSTGD` sulla quota consumi e `γ` sulla quota fissa per `POD/anno`

I valori customer-facing già verificati nel repo sono:
- maggior tutela, trimestre `aprile-giugno 2026`: `0,15811 euro/kWh` monorario e `44,7311 euro/anno` di quota fissa
- `STG` domestico non vulnerabile, `marzo 2026`: `0,174479 euro/kWh` monorario e `-73,1637 euro/anno` di quota fissa

Dal `2026-04-01`, nel `mercato libero domestico`, ARERA non impone una formula numerica unica cross-vendor ma una struttura standardizzata dei corrispettivi:
- offerte non onnicomprensive: `quota annua venditore + quota consumo venditore + dispacciamento/capacità + rete + oneri + imposte`
- offerte onnicomprensive: `quota annua + quota consumo` comprensive di tutte le voci di spesa

Restano vendor-specific il valore dei corrispettivi definiti dal venditore, gli indici usati, l'eventuale adder, le articolazioni per fasce, scaglioni o potenza e gli eventuali sconti o servizi aggiuntivi. Anche il `dispacciamento` non va ridotto a un solo caso: il repo chiude `CDISPD` separato come default, l'eccezione `capacità Terna + dispacciamento TIDE` per offerte variabili almeno orarie e l'inclusione totale nelle offerte `onnicomprensive`.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-ARERA-TIT-2024-2027-PDF`
- `SRC-ARERA-TIDE-REV4-2025-PDF`
- `SRC-GU-DL-19-2025-ART5`
- `SRC-ARERA-386-2025-R-COM-PDF`
- `SRC-ARERA-MT-VALORI-2026-XLSX`
- `SRC-ARERA-STG-VALORI-2026-XLSX`
- `SRC-ARERA-ONERI-SISTEMA-PAGE`
- `SRC-TERNA-DISPACCIAMENTO-PAGE`

## 3) Fiscalità domestica
Sul lato accisa il repo chiude il quadro minimo su abitazioni e agevolazione residente. L'energia elettrica è soggetta ad accisa al momento della fornitura al consumatore finale e, per le abitazioni, il prospetto ADM aggiornato al `2026-01-01` riporta un'accisa base di `0,0227 euro/kWh`. L'agevolazione residente vale per abitazioni di residenza anagrafica dell'utente, con potenza impegnata fino a `3 kW`, fino a `150 kWh` mensili, con i meccanismi di recupero previsti dalla disciplina ADM.

Sul lato IVA, al `2026-04-15`, l'energia elettrica per uso domestico rientra nell'aliquota del `9%`. Nel repo il criterio chiuso è l'`uso domestico`, non una distinzione autonoma residente/non residente. Le parti comuni dei condomini non rientrano nell'uso domestico IVA.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-NORMATTIVA-DLGS-504-ART52`
- `SRC-ADM-ALIQUOTE-NAZIONALI-2026`
- `SRC-ADM-EE-ISTRUZIONI-2026`
- `SRC-NORMATTIVA-DPR-633-TABELLA-A-2026`
- `SRC-AE-RISOLUZIONE-8E-2017`
- `SRC-AE-RISPOSTA-3-2018`

## 4) Bonus sociale e clienti vulnerabili
Il bonus sociale elettrico per disagio economico è coperto nel repo come sconto automatico in bolletta, di durata `12 mesi`, applicabile su una sola fornitura elettrica agevolabile. Le soglie ISEE consolidate nel repo al `2026-04-15` sono:
- `9.796 euro` per nuclei con massimo `3` figli a carico
- `20.000 euro` per nuclei con almeno `4` figli a carico

Gli importi ordinari `2026` già verificati sono:
- `146,00 euro/anno` per nuclei di `1-2 componenti`
- `186,15 euro/anno` per nuclei di `3-4 componenti`
- `204,40 euro/anno` per nuclei oltre `4 componenti`

Per la fornitura diretta la bolletta deve essere intestata a un componente del nucleo ISEE, per uso domestico, attiva o sospesa per morosità. Il diritto nasce nel flusso `DSU/ISEE -> INPS -> SII -> venditore`, non da una richiesta commerciale diretta al venditore. In bolletta il bonus deve comparire come voce separata `bonus sociale` in detrazione e deve essere indicata anche la data di scadenza del bonus per disagio economico.

Sul lato vulnerabilità, il repo tratta come normative e tassative le categorie già consolidate: condizioni economicamente svantaggiate, gravi condizioni di salute o apparecchiature elettromedicali, disabilità ai sensi della legge `104/92`, utenze in isole minori non interconnesse, utenze in strutture abitative di emergenza per eventi calamitosi, clienti con più di `75` anni. Nelle more del servizio di vulnerabilità aggiudicato, il cliente vulnerabile può essere servito dall'esercente di maggior tutela competente per territorio. Se un cliente già in `STG` diventa vulnerabile, non esce automaticamente dallo `STG`: resta nel servizio fino a fine assegnazione, ma può scegliere maggior tutela o mercato libero.

**Fonti SSOT consolidate dietro questa sezione**
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

## 5) Contratti, offerte e trasparenza commerciale
Il baseline contrattuale e di trasparenza è chiuso nel repo su `CCC24`, `PLACET`, `Codice del consumo`, `Portale Offerte`, `DL 19/2025`, deliberazione `386/2025/R/com` e deliberazione `250/2023/R/com` sul recesso anticipato.

Nel perimetro già consolidato:
- prima della conclusione del contratto il cliente deve ricevere la `Scheda sintetica`
- il contratto deve indicare almeno condizioni economiche, durata, rinnovo, garanzie, uso dei dati di lettura, frequenza di fatturazione, metodi e termini di pagamento, eventuale rateizzazione e conseguenze del ritardo nei pagamenti
- la copia integrale del contratto deve essere consegnata o trasmessa entro `10 giorni lavorativi`
- nei contratti a distanza o fuori sede il cliente domestico ha `14 giorni` di diritto di ripensamento

Le offerte `PLACET` restano obbligatorie in variante `Fissa` e `Variabile`, con pari visibilità rispetto alle altre offerte di mercato libero. Non possono essere dual fuel, non possono includere servizi aggiuntivi e hanno documentazione standard ARERA su supporto durevole. Il contratto `PLACET` ha durata indeterminata e rinnovo delle condizioni economiche ogni `12 mesi` con preavviso di `3 mesi`.

Dal `2026-04-01`, per le offerte domestiche del libero:
- le offerte non onnicomprensive devono esporre con pari evidenza i `Corrispettivi definiti dal venditore`, `Sconti e/o bonus`, `Prodotti e/o servizi aggiuntivi`, rete, oneri generali di sistema e link o QR ai corrispettivi regolati vigenti
- le offerte onnicomprensive usano una tabella `Corrispettivi onnicomprensivi` e una dicitura che chiarisce che i corrispettivi includono tutte le voci di spesa
- per le offerte variabili la `Scheda sintetica` deve riportare indice, criterio di aggiornamento, periodicità e, quando applicabile, grafico a `12 mesi` dell'indice
- i venditori devono pubblicare sui propri siti tutte le offerte in corso di validità presenti sul `Portale Offerte`, con codice offerta, documentazione contrattuale, sezione condizioni economiche e relativa `Scheda sintetica`

Nel `Portale Offerte`, le offerte generalizzate sono il perimetro ufficiale di comparabilità per `spesa annua stimata`; le offerte non generalizzate restano fuori da quel perimetro, mentre i casi `art. 10.8` restano con comparabilità derogatoria fino ad adeguamento. Il repo chiude anche la distinzione tra `sconti automatici dei primi 12 mesi`, che entrano nella `spesa annua stimata`, e altre promozioni, che restano descritte solo nel dettaglio dell'offerta.

Sul recesso, il baseline ormai chiuso è tripartito:
- `ripensamento` del consumatore entro `14 giorni` nei contratti a distanza o fuori sede
- `recesso/cambio fornitore` ordinariamente senza oneri
- eventuale `onere di recesso anticipato` ammesso solo nei casi fixed-price fixed-term o fixed-price con condizioni economiche a termine, solo fino alla prima scadenza del periodo fixed, con specifica approvazione del cliente, importo massimo ex ante, ricalcolo alla perdita economica diretta effettiva se inferiore e decadenza in caso di variazione unilaterale del venditore

Nel `Portale Offerte` l'onere di recesso anticipato resta informazione di presenza separata dalla `spesa annua stimata`.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-CCC24-PDF`
- `SRC-ARERA-PLACET-2017-PDF`
- `SRC-NORMATTIVA-DLGS-206-2005`
- `SRC-GU-DL-19-2025-ART5`
- `SRC-ARERA-386-2025-R-COM-PDF`
- `SRC-ARERA-PORTALE-OFFERTE-2024-PDF`
- `SRC-NORMATTIVA-DLGS-210-2021-ART7`
- `SRC-ARERA-250-23-PDF`
- `SRC-ARERA-ATLANTE-RECESSO-COSA-E`

## 6) Switching, voltura, subentro, cessazione e boundary della prima attivazione
Nel repo la distinzione da tenere ferma è questa:
- `switching`: cambio fornitore su `POD` attivo, senza interruzione della fornitura
- `voltura`: cambio intestatario di un `POD` attivo
- `subentro`: attivazione o riattivazione per un nuovo cliente su `POD` disattivo dopo cessazione del precedente contratto
- `cessazione/disattivazione`: chiusura della fornitura su richiesta del cliente, con passaggio del `POD` a stato disattivo
- `nuova connessione/allacciamento`: creazione o completamento del collegamento fisico alla rete, con eventuale preventivo o lavori

Per lo `switching`, il baseline vigente nel repo resta fondato su `ARERA 487/2015`; la riforma reseller a `24 ore` approvata con `ARERA 58/2026` non è ancora applicabile perché entra dal `1 dicembre 2026`. Sul piano contrattuale il cliente ha diritto a cambiare fornitore senza discriminazioni legate a costi, oneri o tempi. Se il caso è puro cambio fornitore su `POD` attivo, non si applica l'obbligo del titolo di disponibilità dell'immobile previsto per voltura o stipula o rinnovo.

Per la `voltura`, il venditore deve raccogliere dati del richiedente e titolo che attesta proprietà, regolare possesso o regolare detenzione dell'immobile, anche tramite autodichiarazione quando ammessa. Nel quadro ARERA già consolidato, la risposta commerciale al cliente ha riferimento primario di `3 giorni lavorativi` e il tempo massimo di esecuzione della voltura è `5 giorni lavorativi`. Il quadro `398/2014 + 135/2021` mantiene anche verifiche `SII/RCU` entro `1 giorno lavorativo` e gestione dei dati di misura entro `5 giorni lavorativi` dalla data di attivazione contrattuale.

Per `subentro` e `cessazione/disattivazione` il baseline è ora chiuso:
- la richiesta di subentro va al venditore prescelto, che la inoltra al distributore entro `2 giorni lavorativi`
- il distributore deve attivare entro `5 giorni lavorativi`
- la cessazione/disattivazione su richiesta cliente ha tempo massimo di `5 giorni lavorativi`
- se il distributore ritarda per cause a lui imputabili, il cliente BT domestico ha diritto a indennizzo automatico base di `40,25 euro`

Il boundary della `prima attivazione` è chiuso nel repo solo per il slice domestico BT corrente:
- se il cliente vuole solo l'`allacciamento` senza attivare subito la fornitura, si rivolge al distributore
- se vuole `allacciamento + attivazione`, si rivolge al venditore, che inoltra al distributore entro `2 giorni lavorativi`
- se il punto è già allacciato, il tempo standard di attivazione è `5 giorni lavorativi`
- se il punto non è ancora allacciato o richiede lavori, si applica il blocco `preventivo + lavori`: `15 giorni lavorativi` per il preventivo, poi `10 giorni lavorativi` per lavori semplici o `50 giorni lavorativi` per lavori complessi
- se servono lavori a cura del cliente o atti autorizzativi, il conteggio regolato non è una promessa calendario cieca: il tempo decorre dall'ultimazione dei lavori cliente e non comprende il tempo degli atti autorizzativi nei casi previsti
- per un allacciamento permanente ordinario BT il costo regolato si costruisce con `quota distanza + quota potenza`; per la residenza anagrafica fino a `3,3 kW` si applica la quota fissa prevista dal `TIC`
- al `2026-04-15` i valori vigenti `2026` verificati nel repo sono `209,62 euro` di quota fissa, `105,08 / 209,62 / 419,24 euro` per gli scaglioni distanza e `78,81 euro/kW` di quota potenza
- alcuni casi di connessione particolare sono a `spesa relativa` e richiedono anticipo di `100 euro` per progettazione o sopralluogo
- se il ritardo è imputabile al distributore, l'indennizzo automatico è `40,25 euro`, poi `80,50` o `120,75 euro` secondo gli scaglioni regolati

Il repo chiude anche due edge case importanti: il rifiuto commerciale della voltura non coincide con un rigetto tecnico `SII`, e la morosità pregressa del precedente intestatario non si trasferisce automaticamente al nuovo richiedente o al `POD`.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-487-15`
- `SRC-ARERA-58-26`
- `SRC-ARERA-398-14`
- `SRC-ARERA-135-21`
- `SRC-ARERA-617-23`
- `SRC-ARERA-616-23`
- `SRC-ARERA-TIC-VIGENTE-2026-PDF`
- `SRC-NORMATTIVA-DL-47-2014-ART5`
- `SRC-NORMATTIVA-DLGS-210-2021-ART7`
- `SRC-SII-EE-SWITCHING-SPEC-2025`
- `SRC-SII-EE-VOLTURA-SPEC-2025`
- `SRC-SII-EE-PRESTAZIONI-TECNICHE-2025`
- `SRC-SII-EE-AOC-RCU-2025`
- `SRC-ARERA-ATLANTE-VOLTURA-RIFIUTO`
- `SRC-ARERA-ATLANTE-VOLTURA-MOROSITA`
- `SRC-ARERA-ATLANTE-SUBENTRO-DEFINIZIONE`
- `SRC-ARERA-ATLANTE-SUBENTRO-TEMPI`
- `SRC-ARERA-ATLANTE-VOLTURA-SUBENTRO-COSTI`
- `SRC-ARERA-ATLANTE-ALLACCIAMENTO-RICHIESTA`
- `SRC-ARERA-ATLANTE-ALLACCIAMENTO-TEMPI`
- `SRC-ARERA-ATLANTE-ALLACCIAMENTO-COSTI-ORDINARIO`
- `SRC-ARERA-ATLANTE-ALLACCIAMENTO-COSTI-PARTICOLARE`
- `SRC-ARERA-ATLANTE-ATTIVAZIONE-COSTI`
- `SRC-ARERA-ATLANTE-ATTIVAZIONE-TEMPI`

## 7) Billing, bolletta e misure
Il repo chiude il tratto essenziale che va dalla misura alla fattura. Il `TIME` disciplina tentativi di rilevazione, autoletture, validazione, ricostruzioni e messa a disposizione dei dati; il `TIF` collega questi dati alla fatturazione retail e impone l'ordine di utilizzo `dato effettivo -> autolettura validata -> stima`.

Nel baseline già consolidato:
- per i clienti domestici elettrici la frequenza riportata nel repo è `bimestrale`
- la fattura ordinaria deve essere emessa entro `45 giorni` dall'ultimo giorno di consumo addebitato
- gli importi inizialmente fatturati in stima possono essere ricalcolati solo quando diventano disponibili dati di misura effettivi, comprese le autoletture
- la bolletta di chiusura deve essere emessa entro `sei settimane` dalla cessazione
- se al momento della cessazione manca ancora il dato di misura, la bolletta provvisoria deve comunque restituire il deposito cauzionale eventualmente versato

La `Bolletta 2025` impone la rappresentazione separata di letture e consumi effettivi o stimati, dei consumi fatturati e dei motivi di ricalcolo. Il repo chiude anche il minimo sugli `Elementi di dettaglio`: restano distinti dalla bolletta sintetica, continuano la Bolletta `2.0` e sono richiamabili dalla seconda pagina tramite `QR code` o link. Nei reclami sugli importi fatturati, il venditore deve allegare gli `Elementi di dettaglio` e, nel libero, anche `Scheda sintetica` e preavvisi commerciali rilevanti.

Sul post-cessazione, se il venditore offre area personale, deve lasciare accessibili per almeno `6 mesi` archivio bollette e archivio notifiche, oltre alle funzioni minime di reclamo o richiesta informazioni. Sul lato prescrizione, il repo chiude che il `dies a quo` della prescrizione biennale si lega al termine entro cui la fattura doveva essere emessa. Se una rettifica di misura viene resa disponibile nel `SII`, il venditore ha `45 giorni` per fatturare il relativo conguaglio.

Il `Portale Consumi` consente al cliente di consultare dati storici di consumo, letture e autoletture con profondità fino a `36 mesi`; per l'elettrico il dettaglio può arrivare al livello `quartorario` quando disponibile nel sistema.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-TIF-2025-PDF`
- `SRC-ARERA-TIME-2024-PDF`
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-ARERA-12-2025-R-COM`
- `SRC-ARERA-204-2025-R-COM`
- `SRC-ARERA-204-2025-R-COM-ALLEGATO-A`
- `SRC-ARERA-TIQV-2026-PDF`
- `SRC-ARERA-97-18-PDF`
- `SRC-ARERA-569-18ALL-TI-PDF`
- `SRC-ARERA-603-21-PDF`
- `SRC-ARERA-604-21-PDF`
- `SRC-ARERA-63-2025-R-COM`
- `SRC-ARERA-PRESCRIZIONE-BIENNALE-2024-PAGE`
- `SRC-ARERA-PORTALE-CONSUMI-PAGE`

## 8) Pagamenti, garanzie e rateizzazioni
Il baseline su pagamenti e garanzie è chiuso nel repo senza overclaim sul libero non `PLACET`. `Scheda sintetica` e contratto devono rendere visibili metodi e canali di pagamento, periodicità di fatturazione, eventuali garanzie richieste, termini di pagamento e informazioni sulla rateizzazione.

Nel perimetro già consolidato:
- nelle offerte `PLACET` la garanzia ammessa è solo il deposito cauzionale, salvo equivalenza della domiciliazione bancaria, postale o su carta di credito per i clienti domestici
- nelle `PLACET` il termine di pagamento non può essere inferiore a `20 giorni` dalla data di emissione
- la fattura deve indicare almeno una modalità di pagamento gratuita
- il cliente che sceglie bolletta non cartacea più domiciliazione ha diritto a uno sconto in fattura
- in maggior tutela il `TIV` disciplina ammontare del deposito, esenzione in caso di domiciliazione e rateizzazione in casi tipizzati
- nello `STG` il `TIV` richiama la disciplina `PLACET` su garanzie, modalità di pagamento, rateizzazione e interessi di mora
- nel mercato libero la deliberazione `63/2025/R/com` ripristina il rinvio regolatorio uniforme alla rateizzazione solo per i casi di periodicità di fatturazione non rispettata e di importi anomali

Se un reclamo scritto corregge una bolletta già pagata o già rateizzata, il `TIQV` impone accredito entro `60 giorni solari` e `rimessa diretta` se il credito supera la bolletta utilizzata per la compensazione. Oltre questo perimetro, le ulteriori pattuizioni del libero non `PLACET` restano clausole contrattuali non generalizzabili nel SSOT.

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-CCC24-PDF`
- `SRC-ARERA-PLACET-2017-PDF`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-ARERA-63-2025-R-COM`
- `SRC-ARERA-TIF-2025-PDF`
- `SRC-ARERA-TIQV-2026-PDF`
- `SRC-ARERA-569-18ALL-TI-PDF`
- `SRC-ARERA-603-21-PDF`
- `SRC-ARERA-604-21-PDF`

## 9) Morosità, sospensione, riattivazione e CMOR
Il repo chiude ormai quasi tutto il baseline su mora, sospensione, riattivazione, articolo `9 TIMOE`, clienti non disalimentabili, ultima istanza e `CMOR`.

Nel perimetro già consolidato:
- prima della sospensione serve costituzione in mora scritta tramite raccomandata `A/R` o `PEC`
- il repo riporta questi termini minimi: `3 giorni lavorativi` tra scadenza e richiesta di sospensione, `25 giorni solari` per clienti `BT` e `40 giorni` per gli altri rispetto alla notifica della mora
- nei punti `BT` tecnicamente idonei la sospensione è preceduta da riduzione della potenza al `15%` della potenza disponibile per `15 giorni`
- dopo la prova del pagamento il venditore deve inoltrare immediatamente la richiesta al distributore e la riattivazione deve avvenire entro `1 giorno feriale`; se c'è stato solo ripristino della potenza il riferimento diventa `1 giorno lavorativo`
- se la riattivazione supera lo standard, per il cliente `BT` domestico scatta rimborso automatico di `35`, `70` o `105 euro`

Se la sospensione non riesce ma il distributore dichiara fattibile l'interruzione dell'alimentazione ex articolo `9 TIMOE`, serve una raccomandata dedicata con stima di massima dei costi. La richiesta può partire solo dopo `10 giorni lavorativi`, il distributore programma l'intervento entro il venerdì della stessa settimana e la data non può superare `15 giorni utili` dalla richiesta. I costi customer-facing di questo intervento non hanno nel corpus verificato un importo fisso ARERA predefinito: il `TIMOE` consente l'addebito dei costi effettivi sostenuti dal distributore.

Dopo un'interruzione ex articolo `9`, per tornare ad avere fornitura serve una nuova richiesta di attivazione; se il cliente ha ancora importi pendenti per precedenti interruzioni, l'articolo `9bis` subordina l'attivazione al pagamento e fa decorrere il tempo regolatorio dal relativo incasso. Sul lato rete, il `TIC` prevede un contributo fisso per sospensione, riattivazione o riduzione di potenza da morosità, ridotto del `50%` con telegestione e applicato una sola volta all'atto della disattivazione o riduzione. In maggior tutela il `TIV` aggiunge un contributo venditore di `23 euro`.

Se la disciplina di mora o sospensione viene violata, scattano indennizzi automatici di `30` o `20 euro` e il venditore non può addebitare ulteriori corrispettivi di sospensione o riattivazione. Se il cliente è `non disalimentabile`, nel libero la morosità segue un percorso speciale: niente sospensione ordinaria del punto, ma risoluzione contrattuale e passaggio al servizio di ultima istanza applicabile.

Sul `CMOR`, il repo chiude questi punti minimi:
- il `CMOR` copre crediti riferiti agli ultimi `5 mesi`
- la richiesta cade nella finestra `6-12 mesi` prevista dal `TISIND`
- il `SII` verifica la richiesta entro `2 giorni`
- il corrispettivo viene applicato nella prima fatturazione utile successiva alla comunicazione del `SII`
- l'utente entrante può sospendere il flusso `CMOR` se sul punto è in corso una morosità del rapporto entrante e il corrispettivo non è già stato incassato

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-ARERA-TIMOE-2024-PDF`
- `SRC-ARERA-TISIND-2026-PDF`
- `SRC-ARERA-TIQE-646-15-PDF`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-ARERA-487-15`
- `SRC-ARERA-CCC24-PDF`
- `SRC-ARERA-PLACET-2017-PDF`
- `SRC-ARERA-TIF-2025-PDF`
- `SRC-ARERA-TIQV-2026-PDF`
- `SRC-ARERA-616-23`
- `SRC-ARERA-ATLANTE-RIATTIVAZIONE-MOROSITA`
- `SRC-ARERA-ATLANTE-COSTI-SOSPENSIONE-RIATTIVAZIONE`

## 10) POD, accessi ai dati, privacy minima e reporting
Nel repo è chiuso un baseline minimo ma solido su identificazione tecnica del punto, accesso del cliente o di terze parti ai dati, limiti di privacy o finalità dichiarati nei canali ufficiali e reporting minimo collegato alla fornitura. Il package editoriale dedicato a questo layer end-to-end è ora anche `DOMAINS/reporting-regolatorio.md`.

Sul `POD` e sui dati tecnici minimi:
- lato cliente, la bolletta deve riportare almeno `indirizzo del punto`, `codice POD` e `potenza impegnata`
- negli `Elementi informativi essenziali` devono comparire anche `tipologia di cliente` e `tensione nominale di alimentazione`
- lato operatore, il canale `CDT` del `SII` rende consultabili almeno `tipologia di misuratore`, `trattamento del punto ai sensi del TIS`, `data di messa a regime del misuratore 2G` e `stato di attivazione del POD`
- il processo `PK` non espone il dato tecnico del punto, ma verifica l'abbinamento tra `POD` e cliente finale e può supportare integrazioni anagrafiche nel `RCU`

Sul lato accesso e privacy:
- il cliente finale ha nel `Portale Consumi` un canale self-service gratuito con accesso a dati storici di consumo, letture, autoletture e principali informazioni tecniche e contrattuali
- la homepage ufficiale del Portale lo descrive come servizio previsto dalla legge per accedere almeno a `anagrafiche`, `contratti` e `misure`, confermando un layer online data-centric distinto dall'archivio documentale del venditore
- il Portale arriva fino a `36 mesi` di storico e, per l'elettrico, fino al dettaglio `quartorario` quando disponibile
- dal `1 ottobre 2025` il cliente può autorizzare e revocare dal Portale Consumi l'accesso ai dati di consumo da parte di terze parti qualificate accreditate al `SII`
- la finestra massima autorizzabile a terzi è di `48 mesi`, con `24` mesi precedenti e `24` successivi alla data di autorizzazione
- l'informativa del Portale chiarisce il trattamento di dati identificativi, `POD/PDR`, indirizzi di ubicazione, misure dei consumi e tracciatura degli accessi
- la stessa informativa dichiara conservazione non oltre `36 mesi` dalla data cui i dati si riferiscono
- sul lato `SII`, i dati personali scambiati tra utenti e gestore sono usati solo per i processi del sistema e non per marketing, promozione o vendita diretta

Sul lato reporting, il repo chiude due layer diversi:
- `TIME/TIF`: messa a disposizione al `SII` dei dati di misura e loro rappresentazione distinta in bolletta tra letture, autoletture, dati stimati, consumi effettivi, consumi stimati e consumi fatturati
- `TIQV`: classificazione prudenziale di reclami e richieste, registro verificabile, causalizzazione dei mancati rispetto, reporting annuale ad `ARERA`, pubblicazione annuale lato venditore e pubblicazioni o survey lato `ARERA` quando previste

**Fonti SSOT consolidate dietro questa sezione**
- `SRC-NORMATTIVA-DL-105-2010-ART1BIS`
- `SRC-GU-L-205-2017-ART1-C6-C8`
- `SRC-ARERA-PORTALE-CONSUMI-PAGE`
- `SRC-AU-PORTALE-CONSUMI-HOMEPAGE-PAGE`
- `SRC-AU-PORTALE-CONSUMI-TERZE-PARTI-PAGE`
- `SRC-AU-PORTALE-CONSUMI-PRIVACY-PAGE`
- `SRC-AU-SII-TRATTAMENTO-DATI-PERSONALI-PAGE`
- `SRC-SII-EE-PRECHECK-SPEC-2019`
- `SRC-SII-EE-CDT-SPEC-2020`
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-ARERA-TIF-2025-PDF`
- `SRC-ARERA-TIME-2024-PDF`
- `SRC-ARERA-TIQV-2026-PDF`
- `SRC-GU-CC-ART2220`
- `SRC-NORMATTIVA-DPR-600-1973-ART22`
- `SRC-NORMATTIVA-DPR-633-1972-ART39`

## 11) Boundary chiuso e follow-up non bloccanti
Dentro il perimetro di questo master document, al `2026-04-15`, non restano gap SSOT attivi. Restano solo note di boundary già chiuso e possibili follow-up futuri.

### 11.1 Morosità, articolo 9 TIMOE
Il boundary è chiuso anche su questo tratto:
- il routing sostanziale dei domestici non vulnerabili non disalimentabili verso `STG` è chiuso dal `TIV 2026`
- il mancato allineamento testuale del `TIMOE` articolo `24.3` rispetto a questo routing ormai esplicito nel `TIV` resta solo nota editoriale di monitoraggio
- nel corpus verificato non emerge un tariffario `ARERA` numerico uniforme per i costi customer-facing dell'interruzione fisica ex articolo `9`; il baseline chiuso resta il rinvio ai costi effettivi dell'intervento

### 11.2 Dati, documenti customer-facing ulteriori e set esteso dei campi POD
Il boundary è chiuso anche su questo tratto:
- il repo separa in modo stabile il self-service dati del `Portale Consumi`, il minimo di area personale del `TIQV`, i documenti da consegnare o trasmettere su `supporto durevole` e la retention interna lato venditore
- oltre a bollette, notifiche e allegati reclamo, i documenti customer-facing ulteriori verificati in modo uniforme restano copia del contratto, `Scheda sintetica` e conferme contrattuali, senza prova di un archivio documentale online generale del venditore
- per l'ordinario domestico il set tecnico/customer-facing chiuso resta quello minimo già estratto da bolletta `ARERA`; i campi ulteriori del `SII/CDT` restano operator-facing e non emerge una fonte customer-facing vigente che imponga ulteriori campi tecnici uniformi del punto

### 11.3 Cosa non è più gap, in questo perimetro
Non risultano più gap SSOT attivi, al `2026-04-15`, su:
- prezzi e struttura economica minima customer-facing
- fiscalità domestica di base
- bonus sociale e vulnerabili
- contratti, offerte, `PLACET`, trasparenza e boundary del recesso anticipato
- switching, voltura, subentro, cessazione e boundary domestico BT della prima attivazione con lavori o preventivi
- billing, misure, `Elementi di dettaglio`, prescrizione e rateizzazione retail uniforme del libero nel perimetro `63/2025`
- pagamenti, garanzie e accrediti minimi `TIQV`

## Dove approfondire nel repo
- `MACRO/domestico-luce-prezzi.md`
- `MACRO/domestico-luce-fiscalita.md`
- `MACRO/domestico-luce-bonus-vulnerabili.md`
- `MACRO/domestico-luce-segmentazione-regimi.md`
- `MACRO/domestico-luce-switching-voltura.md`
- `MACRO/domestico-luce-billing-misure.md`
- `MACRO/domestico-luce-morosita-pagamenti.md`
- `MACRO/domestico-luce-pod-accessi-reporting.md`
- `MACRO/domestico-luce-reporting-regolatorio.md`
- `DOMAINS/contratti-offerte-trasparenza.md`
- `DOMAINS/tutele-graduali.md`
- `DOMAINS/reporting-regolatorio.md`
- `OPEN-QUESTIONS.md`
