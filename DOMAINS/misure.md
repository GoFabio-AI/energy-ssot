# Dominio: Misure

## Perimetro attivo
- settore: energia elettrica
- segmento: clienti domestici
- data di riferimento SSOT: 2026-04-15
- focus: letture, autoletture, stime, ricostruzioni, messa a disposizione dei dati e supporto ai conguagli di fatturazione

## Scopo
Raccogliere le regole minime su come i dati di misura vengono rilevati, validati, corretti e messi a disposizione quando servono per la bolletta del cliente domestico elettrico.

## Copre
- tentativi di rilevazione e frequenze minime
- autolettura ordinaria e in occasione di cambio venditore o voltura
- validazione e tacita validazione delle autoletture
- classificazione dei dati come effettivi, autoletture o stimati
- rettifiche e ricostruzioni dei dati di misura
- disponibilità cliente dei dati tramite Portale Consumi

## Fonti principali
### Primarie
- SRC-ARERA-TIME-2024-PDF
- SRC-ARERA-TIF-2025-PDF

### Ufficiali di supporto
- SRC-ARERA-PORTALE-CONSUMI-PAGE
- SRC-AU-SII-PORTALE

## Fatti regolatori primari
- Il TIME disciplina tentativi di rilevazione, validazione delle autoletture, ricostruzione dei dati e messa a disposizione al SII e agli utenti del trasporto.
- Il TIF collega questi dati alla fatturazione retail, fissando l'ordine d'uso tra dato effettivo, autolettura validata e stima.
- Le rettifiche dei dati di misura possono essere trasmesse anche successivamente e alimentare conguagli e contestazioni di prescrizione; i ricalcoli di importi inizialmente stimati si innestano solo sulla successiva disponibilità di dati effettivi.

## Fatti operativi di supporto
- Il Portale Consumi consente al cliente di consultare dati storici di consumo, letture e autoletture con profondità fino a 36 mesi, coerentemente con la disponibilità nel SII.
- Per il settore elettrico il dettaglio può arrivare fino al livello quartorario quando disponibile nel sistema.

## Evidenze estratte
- `EXTRACTED/SRC-ARERA-TIME-2024-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-TIF-2025-PDF.extracted.md`
- `EXTRACTED/SRC-ARERA-PORTALE-CONSUMI-PAGE.extracted.md`

## Regole collegate
- RULE-EE-POD-003
- RULE-EE-TIF-002
- RULE-EE-TIF-003
- RULE-EE-TIF-004
- RULE-EE-TIF-006
- RULE-EE-TIF-008
- RULE-EE-TIME-001
- RULE-EE-TIME-002
- RULE-EE-TIME-003
- RULE-EE-TIME-004

## Open questions
- Nessuna open question aperta nel perimetro attivo `TIME/TIF + Portale Consumi` usato in questo dominio.
- Restano fuori pacchetto, e quindi non bloccano la chiusura di questo slice, eventuali sviluppi ulteriori sul rollout 2G non tradotti in regole retail customer-facing e la rateizzazione dei maxiconguagli, trattata nel dominio pagamenti/tutele.

## Stato avanzamento
- Coperti: frequenze minime di rilevazione, autoletture, validazione, priorità d'uso in bolletta, disponibilità dati a SII e cliente, ricostruzioni per malfunzionamento e ponte regolatorio tra stima e successivo ricalcolo.
- Chiusura del dominio: chiuso al boundary SSOT al 2026-04-15 nel perimetro customer-facing `TIME/TIF + Portale Consumi`, già atomizzato in regole nel repo.
