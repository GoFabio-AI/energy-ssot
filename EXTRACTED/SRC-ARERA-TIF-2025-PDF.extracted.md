# EXTRACTED - SRC-ARERA-TIF-2025-PDF

## Metadata
- Source ID: SRC-ARERA-TIF-2025-PDF
- URL: https://www.arera.it/fileadmin/allegati/docs/16/TIF_All_a_aggiornato_dal_1__luglio_2025__463-16_.pdf
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf)
- Relevance: molto alta per fatturazione retail, autoletture, stime, ricalcoli, bolletta di chiusura e indennizzi nel domestico elettrico

## Fatti chiave ad alta confidenza
1. Il documento è il TIF, in versione in vigore dall’1 luglio 2025.
2. Per i clienti domestici elettrici la frequenza di emissione delle bollette di periodo è bimestrale e ciascuna bolletta deve essere emessa entro 45 giorni solari dall’ultimo giorno di consumo addebitato.
3. Per il computo dei consumi il venditore deve usare i dati di misura nel seguente ordine: dati effettivi, autoletture validate, dati stimati.
4. Se il venditore usa proprie stime, deve determinarle sulla base dei consumi storici effettivi del cliente forniti dal distributore, integrabili con altre informazioni utili; sul settore elettrico si applica anche uno standard generale semestrale di qualità delle stime con soglia `≤ 0,50`.
5. Per i punti monorari o non dotati di smart meter il venditore deve offrire almeno un canale di autolettura, indicare in bolletta la finestra temporale, comunicare la presa o non presa in carico del dato immediatamente o entro 4 giorni lavorativi e trasmettere il dato al distributore entro 4 giorni lavorativi.
6. La non presa in carico dell’autolettura in finestra è ammessa solo quando il dato è palesemente errato perché diverso dall’ultimo dato effettivo disponibile di almeno un ordine di grandezza.
7. Il venditore procede al ricalcolo di importi precedentemente determinati sulla base di dati di misura stimati solo quando divengono disponibili dati di misura effettivi messi a disposizione dall’impresa di distribuzione, comprese le autoletture.
8. La bolletta di chiusura deve essere recapitata entro sei settimane dalla cessazione; se mancano i dati di misura il venditore deve emettere una bolletta stimata entro i termini, restituire il deposito cauzionale e poi emettere la vera bolletta di chiusura quando il dato sarà disponibile.
9. Nei casi di cambio venditore o voltura, per i punti trattati monorari il cliente può comunicare l’autolettura nel periodo compreso tra il quinto giorno lavorativo precedente e il terzo giorno lavorativo successivo alla decorrenza.
10. Se la bolletta di periodo è emessa in ritardo, il cliente ha diritto a un indennizzo automatico da 6 euro fino a 60 euro a seconda dell’entità del ritardo.

## Citazioni utili
- "Versione in vigore dall’1 luglio 2025"
- "Clienti domestici Bimestrale"
- "Ciascuna bolletta deve essere emessa entro il termine di 45 giorni solari"
- "dati di misura effettivi ... autoletture ... validate ... dati di misura stimati"
- "il venditore determina il dato di misura stimato sulla base dei consumi storici effettivi del cliente"
- "Energia elettrica ≤ 0,50"
- "mettere a disposizione almeno una modalità di raccolta dell’autolettura"
- "comunicare la presa in carico o l’eventuale non presa in carico"
- "palesemente errato"
- "il venditore procede al ricalcolo di importi precedentemente determinati sulla base di dati di misura stimati"
- "entro sei settimane decorrenti dal giorno della cessazione della fornitura"
- "quinto giorno lavorativo precedente ed il terzo giorno lavorativo successivo"
- "il venditore riconosce un indennizzo automatico"

## Uso nel SSOT
- fonte primaria per periodicità, emissione e chiusura della bolletta
- fonte primaria per ordine d’uso di letture, autoletture e stime
- fonte primaria per autolettura retail e indennizzi da ritardo di emissione
- fonte primaria per il trigger regolatorio dei ricalcoli su importi fatturati inizialmente in stima
