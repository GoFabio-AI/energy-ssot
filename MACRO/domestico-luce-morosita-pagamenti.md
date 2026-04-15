# Macro, morosità e pagamenti

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo il baseline già consolidato nel repo su `pagamenti`, `garanzie`, `rateizzazione regolata`, `mora`, `sospensione` e `CMOR`.
- Non generalizza come diritti uniformi le sole clausole contrattuali extra-standard del `mercato libero non-PLACET`, che nel repo restano fuori dal boundary SSOT generale.

## A colpo d'occhio
Nel repo è già presente un baseline leggibile su come il cliente paga, quali garanzie minime possono essere richieste nei regimi regolati o semi-standardizzati, come funzionano gli accrediti minimi da rettifica reclamo e come si sviluppano mora, sospensione, riattivazione e CMOR.

## Pagamenti e garanzie, quadro breve
- `Scheda sintetica` e `contratto` devono rendere visibili metodi e canali di pagamento, periodicità di fatturazione, eventuali garanzie richieste, termini di pagamento e informazioni sulla rateizzazione.
- Nelle offerte `PLACET` la garanzia ammessa è solo il deposito cauzionale, salvo equivalenza della domiciliazione bancaria, postale o su carta di credito per i clienti domestici.
- Nelle `PLACET` il termine di pagamento non può essere inferiore a `20 giorni` dalla data di emissione e la fattura deve indicare almeno una modalità di pagamento gratuita.
- Nelle `PLACET` il cliente che sceglie bolletta non cartacea più domiciliazione ha diritto a uno sconto in fattura.
- In maggior tutela il `TIV` disciplina ammontare del deposito, esenzione in caso di domiciliazione e rateizzazione in casi tipizzati.
- Nel servizio a tutele graduali il `TIV` richiama la disciplina `PLACET` su garanzie, modalità di pagamento, rateizzazione e interessi di mora.
- Nel mercato libero la deliberazione `63/2025/R/com` ripristina il rinvio regolatorio uniforme alla rateizzazione solo per i casi di periodicità di fatturazione non rispettata e di importi anomali.
- Se un reclamo scritto corregge una bolletta già pagata o già rateizzata, il `TIQV` impone accredito entro `60 giorni solari` e `rimessa diretta` se il credito supera la bolletta utilizzata per la compensazione.
- Le fonti ARERA post-sentenze su prescrizione biennale, `569/2018` consolidata, `603/2021` e `604/2021`, aiutano a chiudere il coordinamento tra bolletta e compensazioni a monte della filiera, ma non aggiungono nel corpus verificato diritti retail uniformi ulteriori su rimborsi o accrediti extra-standard del libero non `PLACET`.

## Morosità, quadro breve
- Prima della sospensione serve costituzione in mora scritta tramite raccomandata A/R o PEC.
- Il repo riporta questi termini minimi: `3 giorni lavorativi` tra scadenza e richiesta di sospensione, `25 giorni solari` per clienti BT e `40 giorni` per gli altri rispetto alla notifica della mora.
- Nei punti BT tecnicamente idonei la sospensione è preceduta da riduzione della potenza al `15%` della potenza disponibile per `15 giorni`.
- Dopo la prova del pagamento il venditore deve inoltrare `immediatamente` la richiesta al distributore e la riattivazione deve avvenire entro `1 giorno feriale`; se c'è stato solo ripristino della potenza il riferimento diventa `1 giorno lavorativo`.
- Se la riattivazione supera lo standard, per il cliente BT domestico scatta un rimborso automatico di `35`, `70` o `105 euro`.
- Se la sospensione non riesce ma il distributore dichiara fattibile l'interruzione dell'alimentazione ex articolo `9 TIMOE`, serve una raccomandata dedicata con stima di massima dei costi; la richiesta può partire solo dopo `10 giorni lavorativi`, il distributore programma l'intervento entro il venerdì della stessa settimana e la data non può superare `15 giorni utili` dalla richiesta.
- Nell'articolo `9` i costi customer-facing non sono un importo fisso ARERA predefinito: il TIMOE consente l'addebito dei costi effettivi sostenuti dal distributore per l'intervento di interruzione.
- Dopo un'interruzione ex articolo `9`, per tornare ad avere fornitura non basta la normale riattivazione da pagamento: serve una nuova richiesta di attivazione; se il cliente ha ancora importi pendenti per precedenti interruzioni, l'articolo `9bis` subordina l'attivazione al pagamento e fa decorrere il tempo regolatorio dal relativo incasso.
- Sul lato rete il `TIC` prevede un contributo fisso per sospensione, riattivazione o riduzione di potenza da morosità, ridotto del `50%` con telegestione e applicato `una sola volta` all'atto della disattivazione o riduzione.
- In maggior tutela il `TIV` aggiunge un contributo venditore di `23 euro`, comprensivo di eventuale riduzione/ripristino di potenza e anch'esso non duplicabile tra riduzione e disattivazione.
- Se la disciplina di mora o sospensione viene violata, scattano indennizzi automatici di `30` o `20 euro` e il venditore non può addebitare ulteriori corrispettivi di sospensione o riattivazione.
- Se il cliente è `non disalimentabile`, la morosità nel libero segue un percorso speciale: niente sospensione ordinaria del punto, ma risoluzione contrattuale e passaggio al servizio di ultima istanza applicabile.

## CMOR, quadro breve
- Il `CMOR` copre crediti riferiti agli ultimi `5 mesi`.
- La richiesta di indennizzo cade nella finestra `6-12 mesi` prevista dal `TISIND`.
- Il `SII` verifica la richiesta entro `2 giorni`.
- Il corrispettivo viene applicato nella prima fatturazione utile successiva alla comunicazione del SII.
- L'utente entrante può sospendere il flusso `CMOR` se sul punto è in corso una morosità del rapporto entrante e il corrispettivo non è già stato incassato.

## Cosa resta aperto
## Cosa resta da monitorare o tenere esplicito
- Sul routing dei clienti domestici `non disalimentabili` non vulnerabili il boundary SSOT è chiuso dal `TIV 2026`: oltre all'instradamento generale verso `STG`, gli articoli `48.14` e `50.1` disciplinano espressamente i casi di attivazione ai sensi del Titolo III del `TIMOE`; il mancato allineamento redazionale del comma `24.3` nel testo consolidato del `TIMOE` resta solo nota di monitoraggio editoriale.
- Sul lato pagamenti il residuale normativo uniforme del mercato libero domestico non `PLACET` è chiuso: oltre i minimi già coperti e il riallineamento `63/2025`, le pattuizioni ulteriori restano clausole contrattuali non generalizzabili nel SSOT.
- Per l'interruzione fisica ex articolo `9` non emerge nel corpus verificato un prezzo ARERA customer-facing numerico e uniforme: questa non è una lacuna aperta del repo, ma il boundary chiuso sul rinvio ai costi effettivi dell'intervento.

## Dove approfondire
- [../DOMAINS/morosita-cmor.md](../DOMAINS/morosita-cmor.md)
- [../DOMAINS/pagamenti-garanzie-rateizzazioni.md](../DOMAINS/pagamenti-garanzie-rateizzazioni.md)
- `RULE-EE-TIMOE-001..007`
- `RULE-EE-TISIND-001..003`
- `RULE-EE-CCC24-001..002`
- `RULE-EE-PLACET-001..005`
- `RULE-EE-TIV-004..007`
- `RULE-EE-STG-004..006`
- `RULE-EE-TIQE-001..002`
- `RULE-EE-TIC-001`
- `RULE-EE-SWI-002`
- `RULE-EE-TIQV-011`

## Fonti SSOT già consolidate dietro questa sintesi
- `SRC-ARERA-TIMOE-2024-PDF`
- `SRC-ARERA-TISIND-2026-PDF`
- `SRC-ARERA-CCC24-PDF`
- `SRC-ARERA-TIV-2026-PDF`
- `SRC-ARERA-487-15`
- `SRC-ARERA-PLACET-2017-PDF`
- `SRC-ARERA-63-2025-R-COM`
- `SRC-ARERA-TIF-2025-PDF`
- `SRC-ARERA-TIQV-2026-PDF`
- `SRC-ARERA-TIQE-646-15-PDF`
- `SRC-ARERA-616-23`
