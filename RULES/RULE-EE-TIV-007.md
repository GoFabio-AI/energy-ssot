# RULE-EE-TIV-007

## Metadata
- ID: RULE-EE-TIV-007
- Titolo: Se un domestico resta senza venditore sul mercato libero, il servizio di ultima istanza è maggior tutela per i vulnerabili e STG per i non vulnerabili, con comunicazione entro 3 o 7 giorni
- Dominio: morosita-cmor
- Stato: vigente
- Giurisdizione: Italia
- Ambito: energia elettrica
- Fonte primaria: SRC-ARERA-TIV-2026-PDF
- URL fonte: https://www.arera.it/fileadmin/allegati/docs/23/Allegato_A_TIV_valido__dal_1_gennaio_2026.pdf
- Riferimento preciso: Articolo 1, definizioni; Articolo 4, commi 4.4, 4.7, 4.8 e 4.9; Articolo 8.2; Articolo 47.2; Articolo 48.14; Articolo 50.1
- Data pubblicazione: 2026-01-01
- Data ultima verifica: 2026-04-15

## Testo normalizzato
Quando un cliente domestico resta senza venditore sul mercato libero e quindi senza contratto di trasporto e dispacciamento in vigore sul punto, il SII inserisce il POD nel servizio di ultima istanza coerente con la sua qualifica regolatoria. Per i clienti domestici vulnerabili aventi diritto alla maggior tutela il punto è inserito nel contratto di dispacciamento dell'Acquirente Unico; per i clienti domestici non vulnerabili aventi diritto allo STG domestico il punto è inserito nel contratto di dispacciamento dell'esercente le tutele graduali per i clienti domestici non vulnerabili. Dal momento dell'inserimento il cliente è servito fuori dal mercato libero. L'esercente la maggior tutela deve comunicare l'attivazione del servizio entro 3 giorni lavorativi; l'esercente STG deve comunicarla entro 7 giorni lavorativi e, tra le altre informazioni, deve esplicitare la funzione di ultima istanza del servizio e che l'attivazione è dovuta all'assenza di un contratto di fornitura nel mercato libero. Per i clienti il cui ingresso nello STG avviene a seguito di risoluzione dei contratti di dispacciamento e trasporto ai sensi del Titolo III del TIMOE, il TIV disciplina inoltre espressamente il caso: il parametro `γ`, se positivo, si applica in misura pari a zero fino all'ultimo giorno del mese successivo all'attivazione e l'esercente STG ha titolo a un meccanismo di compensazione dedicato.

## Citazione
"cliente dei servizi di ultima istanza è, alternativamente, il cliente in maggior tutela, il cliente in tutele graduali o il cliente in salvaguardia"; "per i clienti di cui al comma 8.2, nel contratto di dispacciamento dell’Acquirente unico"; "per i clienti di cui al comma 47.2, nel contratto di dispacciamento dell’esercente le tutele graduali per i clienti domestici non vulnerabili"; "A partire dall’inserimento dei punti di prelievo ... è attivato il corrispondente servizio di ultima istanza"; "entro 3 giorni lavorativi"; "entro 7 (sette) giorni lavorativi"; "la funzione di ultima istanza del servizio medesimo"; "In riferimento ai clienti per i quali l’attivazione del servizio a tutele graduali ha luogo a seguito di risoluzione dei contratti di dispacciamento e trasporto ai sensi del Titolo III del TIMOE"; "il parametro γ, se positivo, è applicato ... in misura pari a zero"; "Nei casi di attivazione del servizio a tutele graduali a seguito di risoluzione dei contratti di dispacciamento e trasporto ai sensi del Titolo III del TIMOE"

## Interpretazione minima
Nel domestico elettrico 2026 il raccordo ultima istanza non è più binario maggior tutela versus salvaguardia: i non vulnerabili lasciati senza venditore libero ricadono nello STG domestico, mentre i vulnerabili ricadono nella maggior tutela. Questo non è più solo inferito dal combinato disposto tra articoli 4.4 e 47.2, perché gli articoli 48.14 e 50.1 rendono espresso il raccordo con i casi di attivazione ai sensi del Titolo III del TIMOE.

## Impatto operativo
Nel SSOT e nei flussi customer care bisogna usare la qualifica di vulnerabilità per instradare correttamente il cliente al servizio di ultima istanza e applicare il diverso SLA informativo verso cliente finale, 3 giorni per maggior tutela e 7 giorni per STG. Nei casi di ingresso nello STG per risoluzione ex Titolo III del TIMOE va inoltre considerato il regime economico dedicato con `γ` temporaneamente azzerato se positivo e con compensazione a favore dell'esercente.

## Eccezioni e limiti
La regola riguarda il caso in cui il cliente si trovi senza venditore sul mercato libero. Non disciplina la permanenza dei clienti già in STG che acquisiscono vulnerabilità, regolata separatamente, né dettaglia le comunicazioni del servizio di salvaguardia per clienti non domestici o residuali. Resta un disallineamento redazionale nel TIMOE 24.3, che nel consolidato continua a nominare solo Acquirente Unico e salvaguardia, ma il routing sostanziale domestico non vulnerabile verso STG è esplicitato dal TIV 2026.

## Conflitti o dipendenze
Si coordina con RULE-EE-TIV-003, RULE-EE-STG-003, RULE-EE-VUL-002 e RULE-EE-VUL-003. Per il raccordo con la risoluzione contrattuale da morosità dei clienti non disalimentabili si combina con RULE-EE-TIMOE-007 e con RULE-EE-SWI-002.

## Note
Il testo customer-facing più ricco è quello del comma 4.9 per lo STG, che impone anche informazioni su diritti dei vulnerabili, Portale Offerte e recesso senza oneri verso il libero mercato.
