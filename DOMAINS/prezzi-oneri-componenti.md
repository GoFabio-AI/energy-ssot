# Dominio: Prezzi, oneri e componenti

## Scopo
Raccogliere la scomposizione economica customer-facing della fornitura elettrica domestica e le formule regolatorie che risultano rappresentabili in modo rigoroso da fonti ufficiali al 2026-04-15.

## Perimetro coperto in questo pacchetto
- energia elettrica domestica, non gas
- etichette customer-facing della bolletta e loro aggregazione regolata
- dispacciamento, sia come funzione di sistema sia come componente economica rilevante per il cliente
- struttura della spesa per la vendita / materia energia
- trasporto, distribuzione, misura e gestione contatore nella misura rappresentabile da fonti ufficiali customer-facing
- oneri generali di sistema rilevanti per la scomposizione verso il cliente finale
- formule regolatorie chiuse per maggior tutela e servizio a tutele graduali domestico non vulnerabile
- valori customer-facing pubblicati da ARERA e vigenti al 2026-04-15, quando verificabili da fonte ufficiale

## Regola di separazione
- Fonte: citazione o riferimento puntuale a fonte ufficiale/quasi-ufficiale.
- Fatto: solo ciò che la fonte consente di affermare senza salto interpretativo.
- Interpretazione minima: solo chiarimento necessario per usare il fatto senza ambiguità.
- Decisione prodotto: qualsiasi alias, UX copy o semplificazione oltre il testo regolatorio va marcata come scelta di prodotto e non come fatto SSOT.

## Fatti chiusi da fonte

### 1) Aggregazione customer-facing vigente della bolletta elettrica
- Fonte primaria: `SRC-ARERA-BOLLETTA-2025-PDF`
- Dal testo ARERA valido dall’1 luglio 2025, gli importi fatturati per l’energia elettrica sono aggregati nello Scontrino e negli Elementi di dettaglio almeno nelle voci:
  - `Spesa per la vendita di energia elettrica`
  - `Spesa per la tariffa per l’uso della rete elettrica`
  - `Spesa per gli oneri generali di sistema`
- Le imposte sono riportate separatamente in un riquadro dedicato.
- Interpretazione minima: questa è la nomenclatura regolatoria customer-facing vigente verificata in fonte primaria per il 2026-04-15.

### 2) Rapporto con le etichette legacy ARERA lato consumatore
- Fonte ufficiale di supporto: `SRC-ARERA-GUIDA-VOCI-SPESA`
- La guida consumatori ARERA continua a descrivere le voci con i label legacy:
  - `Spesa per la materia energia`
  - `Spesa per il trasporto e la gestione del contatore`
  - `Spesa per oneri di sistema`
- Per i clienti in maggior tutela, la guida esplicita che la `Spesa per la materia energia` comprende `PE`, `PD`, `PPE`, `PCV` e `DispBT`.
- Interpretazione minima: nel SSOT i label legacy possono essere trattati come alias esplicativi, ma non devono sostituire senza nota la nomenclatura regolatoria vigente della Bolletta 2025.

### 2-bis) La decomposizione customer-facing 2025 passa dallo Scontrino, ma i prezzi puntuali restano negli Elementi di dettaglio
- Fonti: `SRC-ARERA-BOLLETTA-2025-PDF`, `SRC-ARERA-12-2025-R-COM`, `SRC-ARERA-204-2025-R-COM`, `SRC-ARERA-204-2025-R-COM-ALLEGATO-A`
- La deliberazione 12/2025/R/com chiarisce che lo `Scontrino dell’energia` espone gli importi fatturati in sostituzione della classificazione in voci di spesa `per destinazione`.
- La deliberazione 315/2024/R/com precisa che il `prezzo medio` dello Scontrino è un valore medio di sintesi e che i singoli prezzi e corrispettivi applicati ai quantitativi consumati sono negli `Elementi di dettaglio`.
- La stessa deliberazione 12/2025/R/com chiarisce che gli `Elementi di dettaglio` non sono stati modificati rispetto alla precedente disciplina della `Bolletta 2.0`.
- La deliberazione 204/2025/R/com dispone inoltre che, dal 2025-10-31, il Glossario sia integrato dai venditori con il dettaglio degli importi della `spesa per la vendita di energia elettrica` nelle righe del `Box dell’offerta` e degli `Elementi di dettaglio`.
- Interpretazione minima: nel SSOT vanno distinti almeno tre layer, `bucket sintetici di Scontrino`, `dettaglio analitico dei corrispettivi`, `descrizione glossariale`, evitando di trattarli come un unico livello informativo.

### 3) Che cosa entra nella spesa per la vendita di energia elettrica
- Fonte primaria: `SRC-ARERA-BOLLETTA-2025-PDF`
- La `Spesa per la vendita di energia elettrica` comprende i corrispettivi a copertura di:
  - approvvigionamento
  - commercializzazione
  - dispacciamento
  - eventuali sconti
  - altri importi di vendita previsti dal contratto che non rientrano nella tariffa rete né negli oneri generali di sistema
- Interpretazione minima: questa macro-voce non ha una formula uniforme per tutto il mercato libero, perché una parte dei corrispettivi dipende dal contratto e dal Box dell’offerta.

### 4) Che cosa entra nella tariffa per l’uso della rete elettrica per il domestico TIV
- Fonte primaria: `SRC-ARERA-BOLLETTA-2025-PDF`
- La legenda della bolletta chiarisce che la spesa per la rete comprende gli importi per:
  - trasporto dell’energia elettrica sulla rete di trasmissione nazionale
  - distribuzione locale
  - attività di misura
- Per i clienti di cui all’articolo 2.3 lettera a) del TIV, la Tabella 1 indica che nella `Spesa per la tariffa per l’uso della rete elettrica` possono essere ricompresi solo ed esclusivamente:
  - `σ1`
  - `σ2`
  - `σ3`
  - `UC3`
  - `UC6`
- Interpretazione minima: nel perimetro domestico TIV questa è la scomposizione customer-facing rigorosamente supportata per la bucket rete.

### 5) Che cosa entra negli oneri generali di sistema e quale struttura domestica è verificata
- Fonti: `SRC-ARERA-BOLLETTA-2025-PDF`, `SRC-ARERA-ONERI-SISTEMA-PAGE`
- Nella bolletta elettrica, la `Spesa per gli oneri generali di sistema` può ricomprendere solo `ARIM` e `ASOS`.
- La pagina ARERA sugli oneri chiarisce che, dal 2018, le aliquote sono distinte in:
  - `ASOS`, a copertura del sostegno alle rinnovabili e alla cogenerazione
  - `ARIM`, a copertura dei rimanenti oneri generali
- La stessa fonte specifica che per i clienti domestici:
  - non si applica la quota potenza
  - la quota energia è applicata per scaglioni di consumo
  - per i domestici in residenza anagrafica non si applica la quota fissa
- Interpretazione minima: la macro-voce oneri è chiusa lato bucket, ma la formula dettagliata per ogni elemento interno ARIM/ASOS non è stata estesa in questo pacchetto oltre il livello customer-facing.

### 6) Dispacciamento: funzione di sistema e traduzione economica customer-facing
- Fonti: `SRC-TERNA-DISPACCIAMENTO-PAGE`, `SRC-ARERA-TIDE-REV4-2025-PDF`, `SRC-ARERA-TIV-2026-PDF`
- Terna definisce il dispacciamento come l’attività svolta in ogni istante per garantire l’equilibrio tra domanda e offerta di energia sulla rete, tramite controllo dei flussi, mantenimento dell’equilibrio e gestione del mercato per il servizio di dispacciamento.
- Il TIDE chiarisce che il servizio di dispacciamento regola l’accesso e le modalità di erogazione del servizio e include anche l’attribuzione del diritto di immettere o prelevare energia al fine di alimentare i clienti finali.
- Nel TIV 2026, lato maggior tutela, il dispacciamento customer-facing non coincide con una sola voce:
  - `PD` è l’elemento del `PED` a copertura dei costi di dispacciamento
  - `DISPBT` resta una componente distinta tra i corrispettivi unitari della maggior tutela
- Nel TIV 2026, lato STG domestico non vulnerabile, la traduzione economica customer-facing del dispacciamento è `CDISPD`, determinato a partire dai corrispettivi applicati da Terna e dal corrispettivo di capacità, con esclusioni espresse.
- Interpretazione minima: nel SSOT il dispacciamento va modellato su tre livelli distinti, funzione di sistema `Terna/TIDE`, traduzione economica regolata in maggior tutela `PD + DISPBT` e traduzione economica regolata in STG `CDISPD`; resta non uniforme il lato mercato libero.

### 7) Formula regolatoria chiusa per il cliente domestico in maggior tutela
- Fonte primaria: `SRC-ARERA-TIV-2026-PDF`
- Le condizioni economiche della maggior tutela si articolano nei corrispettivi unitari:
  - `PED`
  - `PCV`
  - `PPE`
  - `DISPBT`
- Il TIV stabilisce che `PED = PE + PD`.
- Il TIV definisce inoltre:
  - `PE` come elemento a copertura dei costi di acquisto dell’energia
  - `PD` come elemento a copertura dei costi di dispacciamento
  - `PPE` come corrispettivo di perequazione dei costi di acquisto e dispacciamento
  - `PCV` come corrispettivo di commercializzazione vendita
  - `DISPBT` come componente di dispacciamento a copertura dei meccanismi degli articoli 18-21 del TIV
- Il TIV valido dall’1 gennaio 2026 precisa anche che:
  - per i punti domestici trattati per fasce o orari, `PE = λ × PEbio` e `PD = λ × PDbio`
  - per i punti domestici monorari, `PE = λ × PEM` e `PD = λ × PDM`
  - `PE`, `PD` e `PED` sono pubblicati dall’Autorità prima dell’inizio di ciascun trimestre
  - `DISPBT` ha valore tabellare autonomo e dal 2025-07-01 è pari a `123,11` centesimi di euro/punto di prelievo per anno nella versione verificata
- Rappresentazione minima SSOT consentita:
  - quota energia regolata maggior tutela: `PED + PPE = PE + PD + PPE`
  - quota fissa / per POD maggior tutela: `PCV + DISPBT`
- Interpretazione minima aggiuntiva: nel customer-facing della maggior tutela il dispacciamento economico resta scisso in `PD` e `DISPBT`; il SSOT non deve collassarli in una singola variabile.
- Limite: questa rappresentazione vale per il regime regolato di maggior tutela e non va estesa automaticamente al mercato libero.

### 8) Valori customer-facing ARERA della maggior tutela verificati al 2026-04-15
- Fonti: `SRC-ARERA-MT-VALORI-2026-PAGE`, `SRC-ARERA-MT-VALORI-2026-XLSX`
- ARERA pubblica lato consumatore il prezzo per la vendita del trimestre aprile-giugno 2026 come:
  - monorario `0,15811 euro/kWh`
  - biorario `0,15837 euro/kWh` in `F1` e `0,15799 euro/kWh` in `F23`
  - quota fissa annua `44,7311 euro/anno`
- Il foglio ARERA di dettaglio consente la scomposizione rigorosa, per abitazioni di residenza anagrafica, in:
  - quota energia monoraria `0,15811 = PE 0,15086 + PD 0,01752 + PPE -0,01027`
  - quota fissa annua `44,7311 = PCV 43,5 + DISPBT 1,2311`
- Interpretazione minima: al 2026-04-15 esiste una rappresentazione customer-facing ufficiale del prezzo di vendita in maggior tutela, raccordabile senza salto interpretativo alle componenti TIV.
- Limite: i fogli ARERA sono dichiarati informativi dalla stessa Autorità; in caso di conflitto prevalgono TIV e provvedimenti.

### 9) Formula regolatoria chiusa per il cliente domestico non vulnerabile in STG
- Fonte primaria: `SRC-ARERA-TIV-2026-PDF`
- Le condizioni economiche STG domestico non vulnerabile si articolano nei corrispettivi unitari:
  - `CELD`
  - `CDISPD`
  - `CSED`
  - `CPSTGD`
  - `γ`
- Il TIV stabilisce che:
  - `CELD = λ × media aritmetica mensile del PUN Index GME`, distinta per fasce o monoraria secondo il trattamento del punto
  - `CDISPD = λ × (corrispettivo di capacità + corrispettivi applicati da Terna per il servizio di dispacciamento, al netto delle esclusioni espresse)`
  - `CSED` è il corrispettivo di sbilanciamento efficiente domestici
  - `CPSTGD` è il corrispettivo di perequazione STG domestici
  - `γ` è il parametro in centesimi di euro/POD/anno determinato dall’Autorità sulla base dei prezzi di aggiudicazione delle aree
- Il TIV aggiunge che l’esercente STG applica inoltre ai clienti i corrispettivi del distributore per:
  - trasporto
  - distribuzione
  - misura
  - aliquote A e UC e altri eventuali ulteriori oneri applicati dal distributore
- Nella versione TIV valida dall’1 gennaio 2026 risultano verificati:
  - `CSED = 0,056` centesimi di euro/kWh
  - `CPSTGD = -0,033` centesimi di euro/kWh dal `2026-01-01`
  - `γ = -7.316,37` centesimi di euro/POD/anno dal `2025-07-01`
- Rappresentazione minima SSOT consentita:
  - quota consumo STG: `CELD + CDISPD + CSED + CPSTGD`
  - quota per POD/anno STG: `γ`
  - componenti ulteriori separate: rete e oneri applicati dal distributore, più imposte

### 10) Valori customer-facing ARERA dello STG verificati al 2026-04-15
- Fonti: `SRC-ARERA-STG-VALORI-2026-PAGE`, `SRC-ARERA-STG-VALORI-2026-XLSX`
- ARERA pubblica lato consumatore il prezzo per la vendita del mese di marzo 2026 come:
  - monorario `0,174479 euro/kWh`
  - multiorario `0,174062 euro/kWh` in `F1`, `0,186038 euro/kWh` in `F2`, `0,168636 euro/kWh` in `F3`
  - quota fissa annua `-73,1637 euro/anno`
- Il foglio ARERA di dettaglio consente la scomposizione rigorosa, per abitazioni di residenza anagrafica, in:
  - quota energia monoraria `0,174479 = CELD 0,15774 + CDISPD 0,016509 + CSED 0,00056 + CPSTGD -0,00033`
  - quota fissa annua `-73,1637 = γ`
- Interpretazione minima: al 2026-04-15 esiste una rappresentazione customer-facing ufficiale del prezzo di vendita STG, raccordabile senza salto interpretativo alle componenti TIV.
- Limite: i fogli ARERA sono dichiarati informativi dalla stessa Autorità; in caso di conflitto prevalgono TIV e provvedimenti.

### 11) Baseline consolidata TIV/TIT/TIDE chiusa al 2026-04-15
- Fonti primarie: `SRC-ARERA-TIV-2026-PDF`, `SRC-GU-DL-19-2025-ART2`, `SRC-ARERA-110-25-PDF`, `SRC-ARERA-TIT-2024-2027-PDF`, `SRC-ARERA-TIDE-REV4-2025-PDF`, `SRC-ARERA-586-25-PAGE`, `SRC-ARERA-96-26-PAGE`
- La baseline trasversale da assumere al 2026-04-15 non è un singolo testo unico, ma una catena ufficiale di rinvii composta da:
  - `TIV` come fonte primaria per perimetro e formule dei servizi di vendita di ultima istanza, inclusi maggior tutela domestica vulnerabili e STG domestico
  - `DL 19/2025`, articolo 2, comma 3, come fonte legislativa primaria della permanenza nello STG dei clienti che diventano vulnerabili
  - `ARERA 110/2025/R/eel` come atto di attuazione che inserisce nel TIV il comma 47.3 e coordina maggior tutela e STG post DL 19/25
  - `TIT 2024-2027` come baseline primaria per tariffe di distribuzione, trasmissione e misura lato infrastrutture domestiche (`TD`, `σ1`, `σ2`, `σ3`)
  - `TIDE` revisione 4 come baseline primaria del dispacciamento, cui il TIV rinvia espressamente per il calcolo del `CDISPD`
- Le delibere `586/2025/R/eel` e `96/2026/R/eel` confermano che il TIV resta il contenitore regolatorio trimestralmente aggiornato per maggior tutela e STG anche nel periodo che include il 2026-04-15.
- Interpretazione minima: la baseline "unica" da usare nel SSOT è quindi una baseline composita ma chiusa, in cui vendita ultima istanza = `TIV` (più legge/atti modificativi), rete = `TIT`, dispacciamento = `TIDE`.

### 12) Mercato libero domestico elettrico: boundary SSOT chiuso sul piano strutturale, non su una formula numerica unica
- Fonti primarie: `SRC-GU-DL-19-2025-ART5`, `SRC-ARERA-386-2025-R-COM-PDF`, `SRC-ARERA-PORTALE-OFFERTE-2024-PDF`
- L’articolo 5 del decreto-legge 19/2025 non impone una formula di prezzo unica del libero, ma impone ad ARERA di aumentare trasparenza e confrontabilità con documenti tipo, riduzione e semplificazione dei componenti dei corrispettivi e razionalizzazione dei parametri di riferimento.
- La deliberazione `386/2025/R/com`, efficace dall’`2026-04-01`, chiude il perimetro strutturale delle offerte domestiche di energia elettrica del mercato libero distinguendo due famiglie:
  - offerte non onnicomprensive, con `quota_annua_venditore €/POD/anno` + `quota_consumo_venditore €/kWh` + `corrispettivo_dispacciamento_capacita €/kWh` + `rete` + `oneri_generali` + `imposte`
  - offerte con corrispettivi onnicomprensivi, con `quota_annua_onnicomprensiva €/POD/anno` + `quota_consumo_onnicomprensiva €/kWh`, comprensive di tutte le voci di spesa
- La stessa fonte chiarisce che resta vendor-specific il valore dei corrispettivi definiti dal venditore e la loro articolazione contrattuale: prezzo fisso, indice o indici di riferimento, eventuale adder unico, strutture miste, differenziazioni per fasce, scaglioni, potenza, giorni dell’anno o altre caratteristiche del cliente.
- Per le offerte di energia elettrica non onnicomprensive il dispacciamento e mercato capacità non vanno trattati come parte implicita indistinta della commodity: ARERA richiede una evidenza separata del corrispettivo relativo, normalmente valorizzato al `CDISPD` del TIV.
- La stessa deliberazione chiude l’edge case delle offerte variabili almeno orarie: in questi casi il venditore può sostituire il `CDISPD` con la combinazione tra corrispettivo capacità definito da Terna e corrispettivo di dispacciamento di cui alla sezione 4-25 del `TIDE`.
- Per le offerte onnicomprensive, invece, il venditore non è tenuto a scomporre nella tabella commerciale `dispacciamento`, `rete` e `oneri`; il SSOT deve quindi segnare che tali voci confluiscono nei corrispettivi onnicomprensivi e non sono separatamente ricostruibili dalla disclosure customer-facing dell’offerta.
- Il `Portale Offerte` rende confrontabili le offerte generalizzate tramite `spesa_annua_stimata`, ma non trasforma questa stima in una formula uniforme dell’intero libero. Quando un’offerta richiede adattamenti del Portale o del calcolo della stima, l’articolo `10.8` la mantiene nel perimetro regolato con pubblicazione derogatoria fino all’adeguamento, quindi come caso di comparabilità limitata e non di esclusione automatica.
- Nella `spesa_annua_stimata` entrano gli sconti applicati automaticamente nei primi 12 mesi, mentre le altre promozioni restano su un layer descrittivo separato della pagina di dettaglio; prodotti e servizi aggiuntivi restano a loro volta separati dal nucleo prezzo energia razionalizzato.
- La deliberazione `250/2023/R/com` chiarisce inoltre che l’eventuale onere di recesso anticipato non entra nel computo della `spesa_annua_stimata`, perché dipende dal verificarsi del recesso anticipato, e deve essere trattato nel Portale come informazione di presenza separata dal ranking economico dell’offerta.
- Interpretazione minima: al `2026-04-15` il boundary SSOT del libero domestico è chiuso come `architettura regolata + disclosure minima + comparabilità Portale`, con tre trattamenti minimi del dispacciamento lato offerta (`CDISPD`, eccezione oraria `Terna+TIDE`, inclusione onnicomprensiva), mentre non è legittimo costruire un’unica formula numerica cross-vendor che ARERA non ha imposto.

## Modello SSOT minimo raccomandato per il domestico elettrico

### Bucket customer-facing regolati
1. `spesa_vendita_energia_elettrica`
2. `spesa_tariffa_uso_rete_elettrica`
3. `spesa_oneri_generali_sistema`
4. `imposte`
5. `bonus_sociale` / `ricalcoli` / `altre_partite` solo se presenti in bolletta

### Layer documentali da non confondere
- `scontrino_energia`: layer sintetico customer-facing con quantità, prezzo medio e importo
- `box_offerta`: layer contrattuale per la ricostruzione dell’offerta applicata
- `elementi_dettaglio`: layer analitico dei prezzi e corrispettivi puntuali
- `glossario_bolletta`: layer descrittivo ufficiale, standard ARERA più eventuali integrazioni venditore post 2025-10-31

### Componenti regolatorie minime tracciabili
- Vendita / commodity regolata:
  - maggior tutela: `PE`, `PD`, `PPE`, `PCV`, `DISPBT`
  - maggior tutela, formule utili: `quota_consumi = PE + PD + PPE`, `quota_fissa = PCV + DISPBT`
  - STG domestico non vulnerabile: `CELD`, `CDISPD`, `CSED`, `CPSTGD`, `γ`
  - STG domestico non vulnerabile, formule utili: `quota_consumi = CELD + CDISPD + CSED + CPSTGD`, `quota_fissa = γ`
- Rete:
  - domestico TIV customer-facing: `σ1`, `σ2`, `σ3`, `UC3`, `UC6`
- Oneri generali di sistema:
  - `ARIM`, `ASOS`

### Alias legacy customer-facing verificati
- `materia_energia` in maggior tutela, nelle fonti ARERA lato consumatore: `PE + PD + PPE + PCV + DISPBT`
- `trasporto_e_gestione_contatore`: `σ1 + σ2 + σ3 + UC3 + UC6`
- `oneri_di_sistema`: `ASOS + ARIM`
- Nota: questi alias sono utili per interoperare con materiale consumatori e storico, ma non sostituiscono i bucket primari della Bolletta 2025.

## Regole collegate
- `RULE-EE-PRC-001`
- `RULE-EE-PRC-002`
- `RULE-EE-PRC-003`
- `RULE-EE-PRC-004`
- `RULE-EE-PRC-005`
- `RULE-EE-PRC-006`
- `RULE-EE-PRC-007`
- `RULE-EE-PRC-008`
- `RULE-EE-PRC-009`
- `RULE-EE-PRC-010`
- `RULE-EE-PRC-011`
- `RULE-EE-PRC-012`
- `RULE-EE-PRC-014`
- `RULE-EE-BOL-001`
- `RULE-EE-BOL-003`
- `RULE-EE-BOL-004`
- `RULE-EE-BOL-005`
- `RULE-EE-BOL-006`
- `RULE-EE-DISP-001`
- `RULE-EE-DISP-002`
- `RULE-EE-DISP-003`
- `RULE-EE-DISP-004`
- `RULE-EE-TIV-002`
- `RULE-EE-TIV-003`
- `RULE-EE-STG-002`
- `RULE-EE-STG-003`
- `RULE-EE-FISC-ACCISA-001`
- `RULE-EE-FISC-ACCISA-002`
- `RULE-EE-FISC-ACCISA-003`
- `RULE-EE-FISC-IVA-001`
- `RULE-EE-FISC-IVA-002`
- `RULE-EE-FISC-IVA-003`

## Fonti principali
- `SRC-ARERA-BOLLETTA-2025-PDF`
- `SRC-ARERA-12-2025-R-COM`
- `SRC-ARERA-204-2025-R-COM`
- `SRC-ARERA-204-2025-R-COM-ALLEGATO-A`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-GU-DL-19-2025-ART2`
- `SRC-GU-DL-19-2025-ART5`
- `SRC-ARERA-110-25-PDF`
- `SRC-ARERA-TIT-2024-2027-PDF`
- `SRC-ARERA-TIDE-REV4-2025-PDF`
- `SRC-ARERA-386-2025-R-COM-PDF`
- `SRC-ARERA-250-23-PDF`
- `SRC-ARERA-PORTALE-OFFERTE-2024-PDF`
- `SRC-ARERA-586-25-PAGE`
- `SRC-ARERA-96-26-PAGE`
- `SRC-ARERA-MT-VALORI-2026-PAGE`
- `SRC-ARERA-MT-VALORI-2026-XLSX`
- `SRC-ARERA-STG-VALORI-2026-PAGE`
- `SRC-ARERA-STG-VALORI-2026-XLSX`
- `SRC-ARERA-GUIDA-VOCI-SPESA`
- `SRC-ARERA-ONERI-SISTEMA-PAGE`
- `SRC-TERNA-DISPACCIAMENTO-PAGE`
- `SRC-NORMATTIVA-DLGS-504-ART52`
- `SRC-ADM-ALIQUOTE-NAZIONALI-2026`
- `SRC-ADM-EE-ISTRUZIONI-2026`
- `SRC-NORMATTIVA-DPR-633-TABELLA-A-2026`
- `SRC-AE-RISOLUZIONE-8E-2017`
- `SRC-AE-RISPOSTA-3-2018`

## Fiscalità elettrica domestica chiusa da fonte al 2026-04-15

### Fonte
- Accisa: `SRC-NORMATTIVA-DLGS-504-ART52`, `SRC-ADM-ALIQUOTE-NAZIONALI-2026`, `SRC-ADM-EE-ISTRUZIONI-2026`.
- IVA: `SRC-NORMATTIVA-DPR-633-TABELLA-A-2026`, `SRC-AE-RISOLUZIONE-8E-2017`, `SRC-AE-RISPOSTA-3-2018`.

### Fatti
- L'energia elettrica è sottoposta ad accisa al momento della fornitura al consumatore finale, con applicazione delle aliquote vigenti.
- Per le abitazioni, il prospetto ADM aggiornato al 2026-01-01 riporta l'aliquota di accisa pari a euro 0,0227 per ogni kWh.
- L'esenzione accisa domestica residente vale solo per abitazioni di residenza anagrafica degli utenti, con potenza impegnata fino a 3 kW e soglia base di 150 kWh mensili, secondo i criteri di recupero fissati dall'art. 52, comma 3, lettera e).
- Al 2026-04-15, la Tabella A, Parte III, del DPR 633/1972 colloca il n. 103 tra i beni e servizi soggetti all'aliquota del 9% e include l'energia elettrica per uso domestico.
- Le fonti Agenzia delle Entrate consultate qualificano l'uso domestico in base all'impiego nell'abitazione familiare o in strutture collettive residenziali analoghe.
- Le parti comuni dei condomini non soddisfano il requisito dell'uso domestico ai fini IVA.

### Interpretazione minima
- La distinzione residente/non residente è supportata dalle fonti solo sul lato accisa, perché l'esenzione dell'art. 52, comma 3, lettera e), è limitata alle abitazioni di residenza anagrafica.
- Per l'IVA non emerge, nelle fonti consultate, una distinzione residente/non residente autonoma. Il criterio rilevante è l'uso domestico.
- In assenza di residenza anagrafica, la fornitura domestica resta nel perimetro abitazioni per l'aliquota base di accisa, ma non accede all'esenzione residente.

### Decisioni SSOT
- Modellare separatamente `accisa_domestica_base`, `accisa_esenzione_residenza_anagrafica` e `iva_uso_domestico`.
- Non introdurre nel SSOT una regola IVA residente/non residente, perché non coperta da fonte primaria o quasi-ufficiale consultata.
- Trattare le parti comuni condominiali come caso escluso dall'uso domestico IVA.

## Cosa resta aperto
- Nessun open question SSOT attivo, al 2026-04-15, sul residuo prezzi/customer-facing qui trattato del libero domestico: il boundary è ora chiuso anche sul trattamento comparativo dell'onere di recesso anticipato nel Portale Offerte tramite `SRC-ARERA-250-23-PDF`. Restano solo manutenzione editoriale generale del dominio e futuri aggiornamenti regolatori.

## Stato avanzamento
- Coperti: bucket bolletta 2025, formule regolatorie MT/STG, rete, oneri, dispacciamento, boundary del libero domestico, promozioni automatiche vs detail-only, comparabilità Portale, recesso anticipato e fiscalità domestica di base richiamata nel dominio.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15. Restano solo manutenzione editoriale e futuri aggiornamenti regolatori ufficiali.

## Decisioni prodotto da NON trattare come fatti SSOT
- Non usare come fatto normativo l’equivalenza perfetta tra label legacy (`materia energia`, `trasporto e gestione del contatore`) e label della Bolletta 2025 senza marcarla come alias di presentazione.
- Non comprimere `dispacciamento` in un solo concetto, perché in fonte appare sia come funzione di sistema sia come componente economica con collocazione diversa nei regimi regolati.
- Non modellare una formula unica del domestico elettrico valida per tutti i contratti di mercato libero, perché la fonte primaria chiude solo struttura, disclosure e comparabilità minima, non i valori vendor-specific.

## Vedi anche
- [fiscalita.md](fiscalita.md)
- [fatturazione.md](fatturazione.md)
- [tutele-graduali.md](tutele-graduali.md)
- [bonus-sociale.md](bonus-sociale.md)
- [qualita-commerciale-reclami.md](qualita-commerciale-reclami.md)
- [../GLOSSARIO.md](../GLOSSARIO.md)
- [../OPEN-QUESTIONS.md](../OPEN-QUESTIONS.md)

## Glossario collegato
- dispacciamento
- ARIM
- ASOS
- PED
- PE
- PD
- PPE
- PCV
- DISPBT
- CELD
- CDISPD
- CSED
- CPSTGD
- γ
