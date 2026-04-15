# Glossario Energia SSOT

Definizioni solo da fonti ufficiali.

## Template voce
- Termine
- Definizione ufficiale
- Fonte
- Citazione
- Note d'uso

## Regola di uso
- una voce è "coperta" solo se esiste almeno una fonte ufficiale già registrata e richiamabile nel SSOT
- la tabella sotto è una mappa di copertura terminologica, non sostituisce le future voci definitorie complete
- quando un termine è solo parzialmente coperto, usare il link al dominio o alla regola esistente invece di improvvisare una definizione

## Mappa di copertura terminologica al 2026-04-15

| Termine | Stato | Ancora SSOT attuale | Note |
| --- | --- | --- | --- |
| cliente finale domestico | parziale | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [RULE-EE-TIV-001](RULES/RULE-EE-TIV-001.md) | esiste un'ancora normativa sul perimetro domestico TIV, manca ancora una voce glossario completa |
| cliente vulnerabile | copertura parziale forte | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [DOMAINS/tutele-graduali.md](DOMAINS/tutele-graduali.md), [RULE-EE-VUL-001](RULES/RULE-EE-VUL-001.md) | categorie normative già coperte, manca voce glossario dedicata |
| venditore | parziale | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [DOMAINS/qualita-commerciale-reclami.md](DOMAINS/qualita-commerciale-reclami.md) | termine usato in molte regole ma non ancora definito con una regola lessicale autonoma |
| distributore | parziale | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md) | ruolo presente nei domini, manca una definizione atomica dedicata |
| SII | copertura parziale forte | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [RULE-EE-SII-001](RULES/RULE-EE-SII-001.md) | il ruolo infrastrutturale è già chiuso, manca voce glossario completa |
| RCU | parziale | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [RULE-EE-RCU-001](RULES/RULE-EE-RCU-001.md) | coperta la funzione, manca voce glossario autonoma |
| UdD | parziale | [DOMAINS/switching.md](DOMAINS/switching.md), [RULE-EE-SWI-001](RULES/RULE-EE-SWI-001.md) | compare nella definizione di switching, manca voce dedicata |
| POD | parziale | [DOMAINS/attori-mercato.md](DOMAINS/attori-mercato.md), [DOMAINS/switching.md](DOMAINS/switching.md) | perimetro operativo presente, manca definizione glossario autonoma |
| switching | copertura parziale forte | [DOMAINS/switching.md](DOMAINS/switching.md), [RULE-EE-SWI-001](RULES/RULE-EE-SWI-001.md) | definizione operativa disponibile da fonte SII |
| voltura | copertura parziale forte | [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md), [RULE-EE-VOL-001](RULES/RULE-EE-VOL-001.md) | definizione operativa disponibile da fonte SII |
| subentro | gap | [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md), [OPEN-QUESTIONS.md](OPEN-QUESTIONS.md) | dominio mappato ma nessuna regola ancora chiusa |
| cessazione | gap | [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md), [OPEN-QUESTIONS.md](OPEN-QUESTIONS.md) | dominio mappato ma nessuna regola ancora chiusa |
| autolettura | gap | [DOMAINS/misure.md](DOMAINS/misure.md), [OPEN-QUESTIONS.md](OPEN-QUESTIONS.md) | manca la fonte primaria di base per il dominio misure |
| conguaglio | gap | [DOMAINS/misure.md](DOMAINS/misure.md), [DOMAINS/fatturazione.md](DOMAINS/fatturazione.md) | ancora non c'è una regola atomica dedicata |
| bonus sociale elettrico | copertura parziale forte | [DOMAINS/bonus-sociale.md](DOMAINS/bonus-sociale.md), [RULE-EE-BONUS-001](RULES/RULE-EE-BONUS-001.md) | quadro requisiti, flusso, importi ordinari 2026 ed esposizione minima in bolletta chiusi |
| dispacciamento | copertura parziale forte | [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md), [RULE-EE-DISP-001](RULES/RULE-EE-DISP-001.md) | definizione di sistema e collocazione economica già coperte in parte |
| maggior tutela | parziale | [DOMAINS/tutele-graduali.md](DOMAINS/tutele-graduali.md), [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md) | regime presente nel repo ma non ancora in una voce glossario autonoma |
| servizio a tutele graduali (STG) | parziale | [DOMAINS/tutele-graduali.md](DOMAINS/tutele-graduali.md), [RULE-EE-STG-001](RULES/RULE-EE-STG-001.md) | perimetro e formula economica parzialmente coperti |
| CMOR | copertura parziale forte | [DOMAINS/morosita-cmor.md](DOMAINS/morosita-cmor.md), [RULE-EE-TISIND-001](RULES/RULE-EE-TISIND-001.md), [RULE-EE-TISIND-002](RULES/RULE-EE-TISIND-002.md), [RULE-EE-TISIND-003](RULES/RULE-EE-TISIND-003.md) | perimetro CMOR e sospensione del flusso già coperti; manca ancora una voce glossario completa |

## Etichette canoniche da riusare nel repo

| Etichetta canonica | Dove ancorarla | Evitare |
| --- | --- | --- |
| cliente vulnerabile | [DOMAINS/tutele-graduali.md](DOMAINS/tutele-graduali.md) e [RULE-EE-VUL-001](RULES/RULE-EE-VUL-001.md) | definizioni commerciali o descrizioni non tassative |
| switching | [DOMAINS/switching.md](DOMAINS/switching.md) | usarlo come sinonimo di voltura |
| voltura | [DOMAINS/voltura-subentro-cessazione.md](DOMAINS/voltura-subentro-cessazione.md) | usarlo come sinonimo di subentro |
| spesa per la vendita di energia elettrica | [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md) | sostituirla automaticamente con etichette legacy senza nota |
| spesa per la tariffa per l'uso della rete elettrica | [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md) | confonderla con oneri generali di sistema |
| spesa per gli oneri generali di sistema | [DOMAINS/prezzi-oneri-componenti.md](DOMAINS/prezzi-oneri-componenti.md) | includere UC3 o UC6 in questo bucket |
| bonus sociale elettrico | [DOMAINS/bonus-sociale.md](DOMAINS/bonus-sociale.md) | confonderlo con il contributo straordinario 2025 |

## Priorità glossario
1. chiudere le voci lessicali già coperte da regole forti: cliente vulnerabile, SII, switching, voltura, bonus sociale elettrico, dispacciamento
2. creare voci ponte per i termini strutturali già usati in più domini: cliente finale domestico, POD, RCU, UdD, maggior tutela, STG
3. lasciare come gap esplicito i termini ancora senza base normativa consolidata nel repo: subentro, cessazione, autolettura, conguaglio
