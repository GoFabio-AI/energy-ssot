# RULE-EE-PRESC-004

## Metadata
- ID: RULE-EE-PRESC-004
- Titolo: Nel quadro vigente i consumi elettrici oltre due anni seguono due flussi informativi distinti, a seconda che la prescrizione risulti maturata o no
- Dominio: fatturazione
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-569-18ALL-TI-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/18/569-18all_ti.pdf
- Riferimento preciso: Articolo 3, commi 3.1, 3.2 e 3.3; articolo 4, comma 4.1
- Data pubblicazione: 2021-12-21 per la versione 603 richiamata nel consolidato; consolidato verificato al 2026-04-15
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel quadro ARERA vigente sulla prescrizione biennale, se il venditore fattura importi elettrici riferiti a consumi risalenti a più di due anni deve seguire due percorsi informativi diversi. Se la prescrizione risulta maturata, deve dare separata evidenza degli importi, inserire una pagina iniziale aggiuntiva con avviso che tali importi possono non essere pagati, indicare l'ammontare interessato, fornire un format per eccepire la prescrizione e non assoggettare quegli importi a incasso preautorizzato SDD. Se invece ritiene non maturata la prescrizione per presunte cause ostative, deve integrare la fattura con avviso dedicato, ammontare, motivazione e canali per reclamo.

## Citazione
"che possono non essere pagati"; "format che il cliente finale può utilizzare al fine di eccepire la prescrizione"; "Gli importi oggetto di prescrizione sono esclusi dall’ambito di applicazione di eventuali clausole contrattuali che prevedano metodi di pagamento ... SEPA Direct Debit"; "per i quali si ritiene non sia maturata la prescrizione"

## Interpretazione minima
Questa regola chiude il minimo customer-facing del coordinamento post-sentenze sul lato bolletta: il repo può distinguere in modo verificabile il caso di prescrizione maturata dal caso in cui il venditore ritenga sussistano cause ostative.

## Impatto operativo
Billing e care devono generare template diversi per le due casistiche e, nel caso di prescrizione maturata, bloccare l'incasso automatico degli importi ultra-biennali oggetto di eccezione potenziale.

## Eccezioni e limiti
La valutazione circa la sussistenza delle cause ostative non viene definita in modo autonomo da questa fonte; va letta insieme al chiarimento ARERA 2024 sul fatto che il venditore procede con le sole informazioni fattuali a sua disposizione.

## Conflitti o dipendenze
Si coordina con RULE-EE-PRESC-001, RULE-EE-PRESC-002 e RULE-EE-PRESC-003.

## Note
Il consolidato ufficiale riporta anche la soppressione dell'articolo 5 e del comma 6.4, utile per leggere correttamente il quadro successivo alle sentenze del Consiglio di Stato del 2023.
