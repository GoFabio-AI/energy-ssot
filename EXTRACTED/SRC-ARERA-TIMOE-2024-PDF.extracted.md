# EXTRACTED - SRC-ARERA-TIMOE-2024-PDF

## Metadata
- Source ID: SRC-ARERA-TIMOE-2024-PDF
- URL: https://www.arera.it/fileadmin/allegati/docs/15/258-15TIMOE_new.pdf
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf)
- Relevance: molto alta per morosità elettrica retail, costituzione in mora, sospensione, riduzione di potenza, indennizzi e clausole contrattuali minime

## Fatti chiave ad alta confidenza
1. Il PDF è il TIMOE e riporta in frontespizio `Valido dal 1 luglio 2024`.
2. Prima di richiedere la sospensione della fornitura per morosità, la controparte commerciale deve costituire in mora il cliente con comunicazione scritta a mezzo raccomandata A/R o PEC, indicando almeno termini di pagamento, termine per la richiesta di sospensione, modalità di comunicazione dell’avvenuto pagamento, diritto all’indennizzo automatico e, se del caso, avviso sulla prescrizione di importi oltre due anni.
3. I termini minimi sono regolati dal TIMOE: almeno 3 giorni lavorativi tra il termine ultimo di pagamento e la richiesta di sospensione; per i clienti in bassa tensione almeno 25 giorni solari dalla ricezione della costituzione in mora per la richiesta che porta alla riduzione di potenza; per gli altri almeno 40 giorni solari.
4. Per i clienti finali connessi in bassa tensione, quando il misuratore lo consente, la sospensione è anticipata da una riduzione della potenza al 15% della potenza disponibile per 15 giorni.
5. Se la disciplina di costituzione in mora o dei termini minimi non viene rispettata, il cliente ha diritto a un indennizzo automatico di 30 euro o 20 euro a seconda della violazione, e non può essergli richiesto alcun ulteriore corrispettivo di sospensione o riattivazione.
6. I contratti di vendita devono contenere espressa indicazione dei termini minimi di mora e sospensione, del diritto di richiedere riduzione di potenza o sospensione, del diritto di addebitare i corrispettivi di sospensione/riattivazione nei limiti ARERA e degli indennizzi automatici; per i clienti BT devono anche specificare la riduzione preliminare al 15% per 15 giorni.
7. L’articolo 9 disciplina l’interruzione fisica dell’alimentazione quando la sospensione non è andata a buon fine ma l’intervento è tecnicamente fattibile: serve una raccomandata specifica con stima di massima dei costi, indicazione dell’addebito dei costi effettivi sostenuti dal distributore, avviso di risoluzione del contratto di vendita e avviso che per tornare ad avere fornitura occorre un preventivo lavori per il ripristino dell’alimentazione.
8. La richiesta di interruzione ex articolo 9 può essere presentata solo dopo almeno 10 giorni lavorativi dalla raccomandata; il distributore comunica entro il venerdì della stessa settimana le date di esecuzione, non successive a 15 giorni utili dalla richiesta, ed entro 7 giorni lavorativi dall’intervento comunica l’esito all’utente del trasporto. Se il cliente paga prima dell’intervento, la richiesta deve essere revocata immediatamente.
9. Dopo un intervento di interruzione ex articolo 9, il punto viene rimosso dal contratto di trasporto e dispacciamento dell’utente e la successiva fornitura può essere riattivata solo tramite richiesta di attivazione ai sensi dell’Allegato D alla deliberazione 487/2015/R/eel.
10. L’articolo 9bis stabilisce che, se il distributore ha già eseguito in passato uno o più interventi ex articolo 9 a carico dello stesso cliente finale, una nuova richiesta di attivazione deve essere accompagnata dal pagamento degli importi non ancora saldati segnalati dal distributore; in questi casi il tempo di attivazione decorre dal ricevimento del pagamento da parte del distributore.
11. L’articolo 23 individua tassativamente i clienti finali non disalimentabili e impone al distributore di mantenere e aggiornare un elenco dedicato con POD e codice fiscale o partita IVA, con possibilità per il cliente di chiedere l’inserimento o di rinunciare per iscritto alla qualifica; la richiesta di inserimento ricevuta dall’utente del trasporto va inoltrata al distributore entro il giorno lavorativo successivo.
12. Per i clienti finali non disalimentabili nel mercato libero, in caso di morosità non si applica la sospensione ordinaria della fornitura: l’utente del trasporto può risolvere i contratti e il punto viene trasferito al servizio di ultima istanza applicabile, con attivazione secondo le medesime tempistiche previste per le altre variazioni dell’utente del dispacciamento.

## Citazioni utili
- "Valido dal 1 luglio 2024"
- "mediante comunicazione scritta a mezzo di raccomandata con avviso di ricevimento o PEC"
- "non può essere inferiore a 3 giorni lavorativi"
- "non può essere, inferiore a 25 giorni solari"
- "non può essere inferiore a 40 giorni solari"
- "la potenza sarà ridotta ad un livello pari al 15% della potenza disponibile"
- "euro 30 (trenta)"
- "euro 20 (venti)"
- "al cliente finale non può essere richiesto il pagamento di alcun ulteriore corrispettivo"
- "i contratti di vendita di energia elettrica ... dovranno contenere espressa indicazione"
- "stima di massima dei costi per l’esecuzione dell’intervento"
- "per fruire nuovamente della fornitura dovrà essere formulata una richiesta di preventivo lavori"
- "decorsi non meno di 10 giorni lavorativi"
- "non successive a 15 giorni utili"
- "entro 7 giorni lavorativi successivi"
- "Clienti finali non disalimentabili"
- "l’utente del trasporto può risolvere i relativi contratti di dispacciamento e di trasporto"
- "l’attivazione dei servizi di ultima istanza"
- "entro il giorno lavorativo successivo al suo ricevimento"
- "dell’Acquirente unico"
- "dell’esercente la salvaguardia"

## Uso nel SSOT
- fonte primaria per la sequenza regolata mora > eventuale riduzione di potenza > sospensione
- fonte primaria per indennizzi automatici in caso di mora o sospensione illegittima
- fonte primaria per clausole minime contrattuali in materia di morosità elettrica
- fonte primaria per l’interruzione fisica dell’alimentazione ex articolo 9 e per i relativi costi e tempi minimi customer-facing
- fonte primaria per il trattamento dei clienti non disalimentabili
- fonte primaria per il raccordo tra morosità dei clienti non disalimentabili, risoluzione contrattuale e passaggio al servizio di ultima istanza
- fonte primaria per i tempi minimi di inoltro delle richieste di qualifica non disalimentabile e per il routing TIMOE verso Acquirente Unico o salvaguardia

## Limiti noti
- Il TIMOE disciplina la morosità elettrica e i relativi flussi di sospensione/riattivazione, ma non esaurisce da solo il tema del CMOR, che resta disciplinato dal TISIND.
- Le regole su deposito cauzionale e rateizzazione in maggior tutela richiedono coordinamento con il TIV.
