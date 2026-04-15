# Macro, switching e voltura

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa il materiale consolidato su `POD attivo`, distinzione `switching/voltura`, raccordo con `subentro` e `cessazione/disattivazione` nel domestico BT.
- Include ora anche il boundary concreto della `prima attivazione` quando significa nuova connessione o attivazione con lavori o preventivi minimi.
- Non presenta come chiuso l'intero perimetro A→Z delle connessioni complesse, temporanee, MT o con nuova cabina.

## La distinzione da tenere ferma
- `Switching`: cambia il fornitore su un POD attivo, senza interruzione della fornitura.
- `Voltura`: cambia l'intestatario di un POD attivo.
- `Subentro`: riattiva o attiva la fornitura per un nuovo cliente su un POD disattivo dopo la cessazione del precedente contratto.
- `Cessazione/disattivazione`: chiude la fornitura su richiesta del cliente e porta il POD verso stato disattivo.
- `Nuova connessione / allacciamento`: crea o completa il collegamento fisico alla rete e può richiedere preventivo, lavori semplici o lavori complessi.

## Switching, quadro breve
- Il regime vigente nel repo al 2026-04-15 resta quello fondato su `ARERA 487/2015`.
- La riforma reseller a `24 ore` approvata con `ARERA 58/2026` non è ancora applicabile: entra dal `1 dicembre 2026`.
- Nel perimetro SII lo switching è trattato sui punti attivi e si lega ai processi `SE`, `RC` e `UI`.
- Sul piano contrattuale il cliente ha diritto a cambiare fornitore senza discriminazioni legate a costi, oneri o tempi: l'eventuale `onere di recesso anticipato` non è un costo ordinario di switching, ma una stretta eccezione contrattuale ammessa solo nei casi fixed-price fixed-term e con disclosure rafforzata.
- Se il caso è puro cambio fornitore su POD attivo, non si applica l'obbligo del titolo di disponibilità dell'immobile previsto per voltura o stipula o rinnovo.

## Voltura, quadro breve
- La voltura riguarda l'acquisizione della titolarità di un punto di prelievo attivo, senza disalimentazione.
- Il repo copre sia la voltura con fornitore già presente sia la voltura con cambio fornitore.
- Per la voltura il venditore deve raccogliere i dati del richiedente e il titolo che attesta proprietà, regolare possesso o regolare detenzione dell'immobile, anche tramite autodichiarazione quando ammessa.
- Nel quadro ARERA già consolidato nel repo, la risposta commerciale al cliente ha riferimento primario di `3 giorni lavorativi` e il tempo massimo di esecuzione della voltura è `5 giorni lavorativi`.
- Il quadro `398/2014 + 135/2021` mantiene anche verifiche SII o RCU entro `1 giorno lavorativo` e gestione dei dati di misura entro `5 giorni lavorativi` dalla data di attivazione contrattuale.

## Subentro e cessazione, baseline ora chiusa
- Il `subentro` è trattato nel repo come attivazione su punto `disattivo`, non come voltura e non come switching.
- In linguaggio customer-facing ARERA lo descrive come attivazione da parte di un nuovo cliente dopo cessazione e disattivazione del precedente contratto, equivalente a una prestazione di `riattivazione`.
- La richiesta di subentro va al `venditore prescelto`, che la inoltra al distributore entro `2 giorni lavorativi`; il distributore deve attivare entro `5 giorni lavorativi`.
- La `cessazione/disattivazione` su richiesta cliente ha tempo massimo di `5 giorni lavorativi` e include anche la semplice chiusura contrattuale con lettura finale che protegga il cliente da ulteriori addebiti.
- Se il distributore ritarda per cause a lui imputabili, il cliente BT domestico ha diritto a un indennizzo automatico base di `40,25 euro`.

## Il boundary ora chiuso della prima attivazione
- Il repo non usa più `prima attivazione` come sinonimo automatico di subentro.
- Se il cliente vuole solo l'`allacciamento` senza attivare subito la fornitura, si rivolge al `distributore`.
- Se vuole `allacciamento + attivazione`, si rivolge al `venditore`, che inoltra la richiesta al distributore entro `2 giorni lavorativi`.
- Se il punto è `già allacciato`, il tempo standard di attivazione è `5 giorni lavorativi` dal ricevimento della richiesta completa da parte del distributore.
- Se il punto `non è ancora allacciato` o richiede lavori sulla presa o sulla rete, si applica il blocco `preventivo + lavori`: `15 giorni lavorativi` per il preventivo, poi `10 giorni lavorativi` per lavori semplici oppure `50 giorni lavorativi` per lavori complessi.
- Se il preventivo indica `lavori a cura del cliente` o servono `atti autorizzativi`, il tempo regolato non si legge come una promessa calendario cieca: il conteggio parte dall'ultimazione dei lavori cliente e non comprende il tempo degli atti autorizzativi nei casi previsti dal TIQC.
- Il preventivo deve valorizzare separatamente l'eventuale attivazione e ricordare che la richiesta di attivazione passa dal `venditore`.
- Per un allacciamento permanente ordinario BT il costo regolato si costruisce con `quota distanza + quota potenza`; per la `residenza anagrafica` fino a `3,3 kW` si applica la quota fissa prevista dal TIC. Al `2026-04-15`, i valori vigenti 2026 verificati sul TIC consolidato sono `209,62 euro` di quota fissa, `105,08 / 209,62 / 419,24 euro` per gli scaglioni distanza e `78,81 euro/kW` di quota potenza.
- Alcuni casi di `connessione particolare` non seguono il forfait: sono a `spesa relativa` e richiedono un anticipo di `100 euro` per progettazione o sopralluogo.
- Se il ritardo è imputabile al distributore, il cliente BT domestico ha diritto a un indennizzo automatico di `40,25 euro`, che sale a `80,50` o `120,75 euro`; non è dovuto se il caso è fermo per forza maggiore, atti autorizzativi, cause cliente/terzi o insoluti della prestazione.

## Due edge case già ben chiusi
- Il rifiuto commerciale della voltura non coincide con un rigetto tecnico SII.
- La morosità pregressa del precedente intestatario non si trasferisce automaticamente al nuovo richiedente o al POD; restano solo verifiche separate di eventuale non estraneità al debito.

## Cosa resta fuori, non più come blocker di questo slice
- L'eventuale perimetro A→Z completo della `prima attivazione` quando implica connessioni temporanee, MT, nuove cabine, pluralità di unità immobiliari o altri casi infrastrutturali e autorizzativi più ampi.
- Il coordinamento tra futura riforma switching 24h, pre-check e domini limitrofi come morosità o CMOR resta solo monitoraggio evolutivo fino all'entrata in vigore della riforma, non gap SSOT attivo.
- Il residuo sugli atti ARERA relativi agli oneri di recesso anticipato non è più aperto nel baseline SSOT: la deliberazione `250/2023/R/com` ha chiuso il perimetro attuativo minimo rilevante anche per i casi di cambio fornitore.
- Nel mercato libero il costo customer-facing di voltura, subentro o attivazione è chiarito come dipendente dal contratto, ma non è trasformato nel repo in una mappa esaustiva di tutte le varianti commerciali possibili.

## Dove approfondire
- [../DOMAINS/switching.md](../DOMAINS/switching.md)
- [../DOMAINS/voltura-subentro-cessazione.md](../DOMAINS/voltura-subentro-cessazione.md)
- `RULE-EE-SWI-001..004`
- `RULE-EE-VOL-001..026`

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-ARERA-487-15`
- `SRC-ARERA-58-26`
- `SRC-ARERA-398-14`
- `SRC-ARERA-135-21`
- `SRC-ARERA-617-23`
- `SRC-ARERA-616-23`
- `SRC-ARERA-TIC-VIGENTE-2026-PDF`
- `SRC-NORMATTIVA-DL-47-2014-ART5`
- `SRC-NORMATTIVA-DLGS-210-2021-ART7`
- `SRC-ARERA-250-23-PDF`
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
