# Macro, billing e misure

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo il tratto già leggibile e ben ancorato che va da `misura` a `fatturazione`: letture, autoletture, stime, emissione, chiusura, ricalcoli, dettaglio bolletta, accrediti minimi TIQV e prescrizione.
- Non generalizza come diritti uniformi le sole clausole commerciali extra-standard del mercato libero non `PLACET`, che nel repo restano fuori dal boundary SSOT generale.

## A colpo d'occhio
Nel repo è già leggibile il tratto più importante che va dal dato di misura alla bolletta: ordine d'uso dei dati, frequenza di fatturazione, tempi di emissione, bolletta di chiusura, ricalcoli, prescrizione biennale e accesso del cliente ai dati di consumo.

## Dalla misura alla fattura
- Il `TIME` disciplina tentativi di rilevazione, autoletture, validazione, ricostruzioni e messa a disposizione dei dati.
- Il `TIF` collega questi dati alla fatturazione retail e impone l'ordine di utilizzo: dato effettivo, poi autolettura validata, poi stima.
- Le rettifiche dei dati di misura possono arrivare anche dopo e generare conguagli o contestazioni sulla prescrizione; i ricalcoli di importi stimati si appoggiano solo a successivi dati effettivi.

## Fatturazione minima già chiusa nel repo
- Per i clienti domestici elettrici il repo riporta frequenza `bimestrale` e termine ordinario di emissione entro `45 giorni` dall'ultimo giorno di consumo addebitato.
- Gli importi inizialmente fatturati in stima possono essere ricalcolati solo quando diventano disponibili dati di misura effettivi, comprese le autoletture.
- La bolletta di chiusura deve essere emessa entro `sei settimane` dalla cessazione.
- Se al momento della cessazione manca ancora il dato di misura, la bolletta provvisoria deve comunque restituire il deposito cauzionale eventualmente versato.
- La Bolletta 2025 impone rappresentazione separata di letture e consumi effettivi o stimati e dei motivi di ricalcolo.
- Il repo chiude anche il minimo sugli `Elementi di dettaglio`: restano distinti dalla bolletta sintetica 2025, continuano la Bolletta 2.0 e sono richiamabili dalla seconda pagina tramite QR code o link.
- Nei reclami sugli importi fatturati il venditore deve allegare gli `Elementi di dettaglio` e, nel libero, anche `Scheda sintetica` e preavvisi commerciali rilevanti.
- Se il venditore offre area personale, dopo la cessazione deve lasciare accessibili per almeno `6 mesi` archivio bollette e archivio notifiche, oltre alle funzioni minime di reclamo o richiesta informazioni.
- Il repo distingue ora in modo esplicito tra `cessazione con disattivazione` nel dominio voltura-subentro-cessazione e `cessazione senza disattivazione` rilevante per specifiche finestre di autolettura e per la fattura di chiusura.

## Prescrizione e conguagli
- Il repo chiude che il dies a quo della prescrizione biennale si lega al termine entro cui la fattura doveva essere emessa.
- Se una rettifica di misura viene resa disponibile nel SII, il venditore ha `45 giorni` per fatturare il relativo conguaglio.
- Sul lato bolletta il quadro post-sentenze è ora più stretto e leggibile: il repo distingue il caso in cui la prescrizione risulti maturata dal caso in cui il venditore ritenga esistano cause ostative, mentre il layer di compensazione della `604/2021` resta a monte della filiera.

## Accesso cliente ai dati
- Il Portale Consumi consente al cliente di consultare dati storici di consumo, letture e autoletture con profondità fino a `36 mesi`.
- Per l'elettrico il dettaglio può arrivare fino al livello `quartorario` quando disponibile nel sistema.

## Cosa resta aperto
- Il pacchetto `TIME/TIF + Portale Consumi` sul tratto customer-facing tra misura e bolletta è ora chiuso nel repo.
- Anche il residuo normativo uniforme del libero non `PLACET` è ora chiuso nel suo boundary SSOT: `63/2025/R/com` riallinea la rateizzazione retail ai casi di periodicità mancata e importi anomali, mentre oltre questo perimetro non emergono nel corpus verificato ulteriori diritti retail uniformi su rimborsi o accrediti extra-standard.
- Restano fuori solo clausole commerciali o contrattuali vendor-specific, da non elevare a regole SSOT generali senza fonte ufficiale dedicata.

## Dove approfondire
- [../DOMAINS/fatturazione.md](../DOMAINS/fatturazione.md)
- [../DOMAINS/misure.md](../DOMAINS/misure.md)
- [../DOMAINS/voltura-subentro-cessazione.md](../DOMAINS/voltura-subentro-cessazione.md)
- `RULE-EE-TIF-001..008`
- `RULE-EE-BOL-001..006`
- `RULE-EE-TIQV-011..014`
- `RULE-EE-TIME-001..004`
- `RULE-EE-PRESC-001..005`

## Fonti SSOT già consolidate dietro questa sintesi
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
