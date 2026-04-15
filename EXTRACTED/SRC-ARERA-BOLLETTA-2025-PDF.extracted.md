# EXTRACTED - SRC-ARERA-BOLLETTA-2025-PDF

## Metadata
- Source ID: SRC-ARERA-BOLLETTA-2025-PDF
- URL: https://www.arera.it/fileadmin/allegati/docs/24/315-24___ti.pdf
- Date extracted: 2026-04-15
- Tool: local python extraction (pypdf)
- Relevance: molto alta per la rappresentazione customer-facing di letture, consumi, ricalcoli e voci di spesa in bolletta

## Fatti chiave ad alta confidenza
1. Il PDF ARERA "La bolletta dei clienti finali di energia" è valido dall’1 luglio 2025.
2. Per l’energia elettrica, la Tabella 1 disciplina l’aggregazione degli importi fatturati per `Spesa per la vendita di energia elettrica`, `Spesa per la tariffa per l’uso della rete elettrica` e `Spesa per gli oneri generali di sistema`, con imposte esposte separatamente.
3. La sezione `Letture e consumi` richiede l’indicazione separata di letture rilevate, autoletture, letture ricondotte e letture stimate, nonché di consumi effettivi, consumi stimati e consumi fatturati, con articolazione per fascia nel settore elettrico; per i punti del TIF art. 7.1 deve comparire anche la finestra temporale per comunicare l’autolettura.
4. Se in bolletta sono presenti letture o consumi stimati, deve essere indicato che gli importi fatturati potranno essere oggetto di successivo ricalcolo.
5. Nei ricalcoli di importi precedentemente fatturati in base a consumi stimati, la bolletta deve riportare il periodo del ricalcolo, i consumi e gli importi già contabilizzati in detrazione e l’importo finale da addebitare o accreditare.
6. Nei ricalcoli dovuti a modifica dei dati di misura, la bolletta deve riportare il periodo di riferimento, la lettura iniziale e finale, il consumo risultante, il motivo del ricalcolo e l’importo da addebitare o accreditare.
7. Il consumo annuo aggiornato deve essere determinato usando letture rilevate, autoletture o letture ricondotte; se tali dati non sono disponibili, il venditore usa la miglior stima basata sui dati in suo possesso.
8. La legenda del provvedimento chiarisce che la spesa per la rete comprende trasmissione nazionale, distribuzione locale e misura.
9. Nella pagina dello Scontrino dell’energia devono essere indicati almeno l’indirizzo del punto, il codice POD e, per l’energia elettrica, la potenza impegnata.
10. Negli Elementi informativi essenziali, alla sezione `Caratteristiche tecniche della fornitura`, per il settore elettrico devono comparire la tipologia di cliente e la tensione nominale di alimentazione.
11. Negli Elementi informativi essenziali la bolletta deve riportare anche la data di scadenza del bonus sociale per disagio economico.
12. Dopo le voci `quota fissa` e `quota per consumi` il modello di bolletta prevede una voce separata `bonus sociale` in detrazione, per i clienti che ne hanno titolo.
13. Il facsimile ARERA di bolletta bimestrale per cliente domestico residente con bonus sociale mostra la riga `Bonus sociale (2 mesi) - 30,00 €`, separata dalle altre voci di spesa.

## Citazioni utili
- "Valida dall’1 luglio 2025"
- "Spesa per la vendita di energia elettrica"
- "Spesa per la tariffa per l’uso della rete elettrica"
- "Spesa per gli oneri generali di sistema"
- "il dettaglio delle letture con l’indicazione separata tra letture rilevate, autoletture, letture ricondotte e letture stimate"
- "il dettaglio dei consumi, con l’indicazione separata tra consumi effettivi, consumi stimati e consumi fatturati"
- "l’indicazione della finestra temporale a disposizione del cliente per comunicare l’autolettura"
- "nel caso di letture e consumi stimati, che gli importi fatturati potranno essere oggetto di successivo ricalcolo"
- "i consumi e gli importi già contabilizzati nelle precedenti bollette, in detrazione"
- "ricalcolo per lettura precedentemente errata"
- "ricalcolo per ricostruzione dei consumi"
- "il consumo annuo è determinato rispetto alla miglior stima effettuata dal venditore in base ai dati in suo possesso"
- "l’indirizzo cui corrisponde il punto"
- "il codice POD"
- "la potenza impegnata"
- "la tipologia di cliente"
- "la tensione nominale di alimentazione"
- "la data di scadenza del bonus sociale per disagio economico"
- "a) “bonus sociale” in detrazione, per i clienti che ne hanno titolo"
- "Bonus sociale (2 mesi) - 30,00 €"

## Uso nel SSOT
- fonte primaria per la nomenclatura customer-facing vigente della bolletta elettrica
- fonte primaria per i contenuti obbligatori su letture, consumi, stime e ricalcoli
- fonte primaria per distinguere bucket di bolletta, ricalcoli e consumo annuo aggiornato
- fonte primaria per la minima anagrafica tecnica customer-facing del POD esposta in bolletta
- fonte primaria per confermare che il bonus sociale, in bolletta, è una detrazione esposta separatamente dai bucket di spesa

## Limiti noti
- Il provvedimento regola l’aggregazione customer-facing e i contenuti della bolletta, non sostituisce il TIF o il TIME per la formazione del dato di misura e delle tempistiche di fatturazione.
