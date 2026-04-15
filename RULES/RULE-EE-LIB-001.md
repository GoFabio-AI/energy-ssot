# RULE-EE-LIB-001

## Metadata
- ID: RULE-EE-LIB-001
- Titolo: Nel mercato libero elettrico la rateizzazione retail uniforme ARERA resta formalmente limitata a periodicità mancata e importi anomali
- Dominio: pagamenti-garanzie-rateizzazioni
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-63-2025-R-COM
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/25/63-2025-R-com.pdf
- Riferimento preciso: considerando, pagine 2-4; dispositivo punto 1
- Data pubblicazione: 2025-02-27
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Nel mercato libero elettrico, per i clienti finali domestici del perimetro retail qui rilevante, il rinvio regolatorio uniforme ARERA alla rateizzazione degli importi fatturati resta formalmente limitato ai casi di mancato rispetto della periodicità di fatturazione e di fatturazione di importi anomali. La deliberazione 63/2025/R/com riallinea infatti l'articolo 11 della deliberazione 463/2016/R/com al riferimento vigente dell'articolo 11 PLACET, ma solo ai numeri iv e v del comma 11.2, senza introdurre un diritto generale alla rateizzazione di ogni maxiconguaglio o di ogni importo elevato nel libero non-PLACET.

## Citazione
"estendere l’obbligo di rateizzazione ... anche ai clienti finali serviti nel mercato libero"; "nei casi di fatturazione di importi anomali e nei casi di ritardo di emissione della fattura per un periodo superiore alla periodicità di fatturazione"; "opportuno ridefinire formalmente il riferimento"; "all’articolo 11, comma 2, lettera a., numeri iv. e v."

## Interpretazione minima
La fonte chiude il residuo SSOT sul libero non-PLACET relativo alla rateizzazione retail uniforme: esiste un aggancio regolatorio verificato, ma è circoscritto a due trigger customer-facing già tipizzati, non a un diritto generalizzato su tutti i maxiconguagli.

## Impatto operativo
I flussi billing e care del libero non-PLACET devono attivare il percorso minimo di rateizzazione regolata quando ricorrono i casi di periodicità mancata o importi anomali. Per gli altri conguagli elevati, il repo non deve inferire automaticamente un diritto uniforme alla rateizzazione se manca un diverso titolo contrattuale o regolatorio specifico.

## Eccezioni e limiti
La regola non sostituisce il dettaglio operativo dell'articolo 11 PLACET su soglie, tempi, numero minimo di rate e interessi, che resta la matrice tecnica richiamata. Non disciplina inoltre rimborsi o accrediti extra-standard fuori dal perimetro TIQV già atomizzato nel repo.

## Conflitti o dipendenze
Si coordina con RULE-EE-PLACET-004, RULE-EE-TIQV-011, RULE-EE-TIQV-012, RULE-EE-TIF-001, RULE-EE-TIF-007 e RULE-EE-PRESC-005.

## Note
La regola serve anche a evitare overclaim nel SSOT: il pacchetto post-sentenze 569/603/604 e il riallineamento 63/2025 non autorizzano a trasformare ogni maxiconguaglio del libero non-PLACET in rateizzazione retail generalizzata.
