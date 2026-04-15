# Macro, POD, accessi e reporting minimo

Snapshot SSOT: 2026-04-15

## Perimetro di questa nota
- Usa solo il materiale già consolidato nel repo su `POD`, `Portale Consumi`, `SII`, accesso ai dati, privacy minima dichiarata e reporting dei dati di misura direttamente collegato al punto.
- Chiude al boundary SSOT il residuo su documenti customer-facing ulteriori, disponibilità online oltre il minimo TIQV e set ordinario dei campi `POD` lato cliente.
- Il baseline TIQV su registri, classificazione prudenziale, causalizzazione, reporting annuale e pubblicazioni ARERA è ora chiuso, ma il dettaglio attuativo di eventuali survey o istruzioni ulteriori resta nel dominio `qualita-commerciale-reclami`.

## A colpo d'occhio
Nel repo è ora leggibile un baseline minimo ma solido su tre cose diverse che spesso vengono confuse: identificazione tecnica del punto, accesso del cliente o degli operatori ai dati della fornitura e limiti minimi di utilizzo o conservazione dichiarati nei canali ufficiali SII e Portale Consumi.

## POD e dati tecnici minimi
- Lato cliente, la bolletta deve riportare almeno `indirizzo del punto`, `codice POD` e `potenza impegnata`.
- Negli Elementi informativi essenziali devono comparire anche `tipologia di cliente` e `tensione nominale di alimentazione`.
- Lato operatore, il canale `CDT` del SII rende consultabili almeno `tipologia di misuratore`, `trattamento del punto ai sensi del TIS`, `data di messa a regime del misuratore 2G` e `stato di attivazione del POD`.
- Il processo `PK` non espone il dato tecnico del punto, ma verifica l'abbinamento tra `POD` e cliente finale e può supportare integrazioni anagrafiche nel `RCU`.

## Accesso cliente e accesso di terze parti
- Il cliente finale ha un canale ufficiale self-service nel `Portale Consumi`, con accesso gratuito ai dati storici di consumo, letture, autoletture e principali informazioni tecniche e contrattuali.
- La homepage ufficiale di `Acquirente Unico` qualifica inoltre il Portale come servizio gratuito previsto dalla legge per accedere alle informazioni sulle proprie utenze, cioè almeno `anagrafiche`, `contratti` e `misure`.
- Nel perimetro oggi consolidato nel repo, il Portale arriva fino a `36 mesi` di storico e, per l'elettrico, fino al dettaglio `quartorario` quando disponibile nel sistema.
- Dal `1 ottobre 2025` il cliente può anche autorizzare e revocare dal Portale Consumi l'accesso ai dati di consumo da parte di terze parti qualificate accreditate al `SII`.
- La finestra massima del dataset autorizzabile a terzi è di `48 mesi`, con `24` mesi precedenti e `24` successivi alla data di autorizzazione.

## Privacy minima e limiti d'uso
- L'informativa del Portale Consumi chiarisce che vengono trattati dati identificativi, POD o PDR, indirizzi di ubicazione, misure dei consumi e tracciatura degli accessi.
- La stessa informativa dichiara una conservazione non oltre `36 mesi` dalla data cui i dati si riferiscono e riconosce almeno accesso, portabilità, rettifica e opposizione nei limiti di legge.
- Sul lato `SII`, il repo chiude un limite minimo molto importante: i dati personali dei clienti finali scambiati tra Utenti e Gestore sono usati solo per i processi del sistema e non per marketing, promozione o vendita diretta.

## Reporting minimo già chiuso nel repo
- Il `TIME` impone la messa a disposizione al `SII` dei dati di misura con tempi e qualificazioni regolate.
- Il `TIF` e la disciplina bolletta impongono poi la rappresentazione distinta di letture, autoletture, dati stimati, consumi effettivi, consumi stimati e consumi fatturati.
- Sul layer `TIQV`, il repo chiude anche classificazione prudenziale di reclami e richieste, registro verificabile, causalizzazione dei mancati rispetto, reporting annuale ad `ARERA`, pubblicazione annuale lato venditore e pubblicazioni o survey ARERA dipendenti da selezione o determinazione.
- In pratica, il repo chiude già sia il reporting del dato di misura che collega `punto -> SII -> fatturazione -> visibilità cliente`, sia il baseline minimo del reporting qualità commerciale collegato alla fornitura.

## Cosa resta fuori dal boundary già chiuso
- Non esiste ancora una fonte primaria unica che elenchi in modo esaustivo tutti i campi dell'anagrafica tecnica `POD` tra vista cliente e vista operatore, ma questo non impedisce più la chiusura del baseline: il set minimo lato cliente resta quello di `RULE-EE-POD-007`, quello lato operatore resta quello di `RULE-EE-POD-005`.
- Oltre a bollette, notifiche e allegati reclamo, i documenti customer-facing ulteriori verificati in modo uniforme restano copie del contratto, `Scheda sintetica` e conferme contrattuali su `supporto durevole`; non emerge invece un obbligo generale di archivio documentale online del venditore più ampio del minimo `TIQV`.
- Restano fuori da questa macro solo eventuali futuri atti `ARERA/AU/SII` che amplino davvero i campi tecnici customer-facing ordinari del `POD` o la document availability online; fino ad allora il residual `OQ-DATI-001` è da considerare chiuso al boundary `SSOT`.

## Dove approfondire
- [../DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md](../DOMAINS/anagrafica-tecnica-pod-accessi-reporting.md)
- [../DOMAINS/misure.md](../DOMAINS/misure.md)
- [../DOMAINS/fatturazione.md](../DOMAINS/fatturazione.md)
- `RULE-EE-POD-001..010`
- `RULE-EE-RCU-001..003`
- `RULE-EE-TIF-003`
- `RULE-EE-TIME-003`
- `RULE-EE-TIQV-015..028`

## Fonti SSOT già consolidate dietro questa sintesi
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
