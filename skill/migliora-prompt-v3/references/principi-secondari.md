# Principi secondari

Leggi questo file solo se il prompt rientra in uno di questi casi. Per tutto il resto bastano i principi del SKILL.md.

## Indice
- Documenti lunghi
- Ricerca e verifica delle fonti
- Ancoraggio ai dati
- Ragionamento e autoverifica
- Design e frontend
- Prompt agentici (istruzioni di progetto, skill, task pianificati)

## Documenti lunghi (circa 20k+ token)
- Metti i dati lunghi **in alto**, sopra domanda, istruzioni ed esempi; la richiesta va **in fondo**. Può migliorare la qualità fino al 30%.
- Più documenti: ognuno in `<document>` con `<source>` e `<document_content>`.
- Chiedi di citare prima le parti rilevanti e poi di eseguire il compito: filtra il rumore.

## Ricerca e verifica delle fonti
- Definisci criteri di successo chiari e chiedi la verifica su più fonti.
- Per ricerche complesse chiedi ipotesi concorrenti, livello di confidenza e autocritica dell'approccio.

## Ancoraggio ai dati
- Se il prompt riguarda file o documenti, chiedi di leggerli prima di rispondere e di non fare affermazioni che non derivano da essi.

## Ragionamento e autoverifica
- Per problemi con più fattori usa istruzioni generali ("ragiona a fondo prima di rispondere") invece di piani passo-passo prescrittivi: il ragionamento del modello spesso supera quello che prescriveresti.
- Per compiti ripetibili, esempi nel formato problema → metodo → risposta attesa.
- Aggiungi un'autoverifica quando serve ("prima di concludere, verifica la risposta rispetto a [criteri]"). Non appesantire i compiti semplici.

## Design e frontend
- Per evitare l'estetica generica specifica: tipografia distintiva, palette coerente con colori dominanti e accenti netti, animazioni mirate, sfondi con profondità. Evita font e schemi di colore abusati.

## Prompt agentici (istruzioni di progetto, skill, task pianificati)
Qui il prompt verrà letto da un'AI che lavora senza supervisione o che lo riceve ogni volta come contesto fisso. Cambiano le priorità:
- **Esecuzione autonoma**: se nessuno può rispondere a domande durante l'esecuzione, indica cosa fare quando le informazioni mancano (scegliere il default più ragionevole e dichiararlo, oppure fermarsi). Senza questa regola l'AI si blocca o inventa.
- **Prompt senza memoria**: un task pianificato parte da una sessione nuova. Il prompt deve essere autosufficiente: obiettivo, fonti, criteri, formato e destinazione dell'output, senza riferimenti a "la chat precedente".
- **Criteri di completamento**: definisci cosa significa "finito" e cosa consegnare (file, tabella, messaggio), altrimenti il risultato è imprevedibile.
- **Istruzioni di progetto e skill**: sono lette molte volte, su richieste diverse. Descrivi principi e motivazioni invece di casi singoli; metti nella descrizione (non nel corpo) quando devono attivarsi; evita regole rigide in maiuscolo.
- **Azioni irreversibili**: se il compito può cancellare, inviare o modificare dati, esplicita cosa è permesso e cosa richiede conferma.
- **Parametri tecnici** (effort, budget_tokens, prefill, subagenti): non fanno parte del testo del prompt, quindi non inserirli e non suggerirli nella riscrittura.
