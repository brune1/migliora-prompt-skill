# migliora-prompt-v3

🇮🇹 [Italiano](#italiano) · 🇬🇧 [English](#english)

---

## Italiano

### Descrizione
Skill per Claude che riscrive un prompt applicando le best practice ufficiali di Anthropic. Gratuita e open source.

### Cosa fa
- Prende un prompt scritto in modo vago o disordinato e lo riscrive in modo più chiaro, strutturato ed efficace, senza eseguirlo.
- Chiede solo ciò che non può dedurre (obiettivo e contesto d'uso), al massimo 3 domande a scelta. Ruolo, formato e tono li sceglie lui e te li dichiara; se il prompt è già completo, non fa domande.
- Gestisce anche prompt per task pianificati, skill e istruzioni di progetto, che vengono eseguiti senza supervisione.
- Mantiene la lingua e l'intento del prompt originale.
- Restituisce il prompt migliorato in un blocco da copiare e spiega in pochi punti cosa ha cambiato e perché.
- Dentro un progetto Claude, usa istruzioni, file e chat del progetto come contesto, solo quando il prompt ne dipende.
- Non si attiva per email, post o testi destinati a persone.

### Installazione

**Claude.ai (consigliato)**
1. Scarica `migliora-prompt-v3.zip` dalla [pagina Release](https://github.com/brune1/migliora-prompt-skill/releases/latest).
2. Su Claude.ai vai in **Settings → Capabilities → Skills** (il percorso può variare).
3. Carica lo ZIP e attiva la skill.

**Claude Code**
1. Scarica e decomprimi lo ZIP.
2. Copia la cartella `migliora-prompt-v3` in `~/.claude/skills/`.

**Solo copia-incolla (senza installare)**
Apri [`prompt/migliora-prompt-v3.md`](prompt/migliora-prompt-v3.md), copia il testo e incollalo all'inizio di una chat con Claude, poi scrivi il prompt da migliorare. Questa versione contiene tutte le regole in un unico testo.

### Struttura del repository
- `skill/migliora-prompt-v3/`: la skill (`SKILL.md` e `references/`).
- `skill/migliora-prompt-v3/evals/`: casi di test per verificare la skill, non servono per usarla (lo ZIP delle Release non li include).
- `prompt/`: versione copia-incolla.

### Esempio d'uso
Scrivi in chat:
```
migliora questo prompt: scrivimi un riassunto sul cambiamento climatico
```
Il prompt è vago, quindi la skill chiede prima le informazioni mancanti (a cosa serve e chi lo leggerà, limite di lunghezza), con domande a scelta. Dopo le tue risposte restituisce il prompt migliorato in un blocco di codice, seguito dai principali cambiamenti e dalle scelte fatte al posto tuo. Se il prompt è già completo, la riscrittura arriva subito.

### Licenza
MIT. Vedi [LICENSE](LICENSE). Autore: Alessandro ([profilo GitHub](https://github.com/brune1)).

---

## English

### Description
A Claude skill that rewrites a prompt using Anthropic's official best practices. Free and open source.

### What it does
- Takes a vague or messy prompt and rewrites it to be clearer, better structured and more effective, without executing it.
- It only asks what it cannot infer (goal and usage context), at most 3 multiple-choice questions. Role, format and tone are chosen by the skill and declared to you; if the prompt is already complete, it asks nothing.
- It also handles prompts for scheduled tasks, skills and project instructions, which run without supervision.
- Keeps the language and intent of the original prompt.
- Returns the improved prompt in a copyable block and explains in a few points what changed and why.
- Inside a Claude project, it uses the project's instructions, files and chats as context, only when the prompt depends on them.
- It does not trigger for emails, posts or texts meant for people.

> Note: the skill's instructions are written in Italian, and it replies (including headings and questions) in the language of your prompt.

### Installation

**Claude.ai (recommended)**
1. Download `migliora-prompt-v3.zip` from the [Releases page](https://github.com/brune1/migliora-prompt-skill/releases/latest).
2. On Claude.ai go to **Settings → Capabilities → Skills** (the path may vary).
3. Upload the ZIP and enable the skill.

**Claude Code**
1. Download and unzip the file.
2. Copy the `migliora-prompt-v3` folder into `~/.claude/skills/`.

**Copy and paste only (no install)**
Open [`prompt/migliora-prompt-v3.md`](prompt/migliora-prompt-v3.md), copy the text and paste it at the start of a chat with Claude, then write the prompt to improve. This version contains all the rules in a single text.

### Repository structure
- `skill/migliora-prompt-v3/`: the skill (`SKILL.md` and `references/`).
- `skill/migliora-prompt-v3/evals/`: test cases to check the skill, not needed to use it (the release ZIP does not include them).
- `prompt/`: copy-and-paste version.

### Usage example
Type in chat:
```
migliora questo prompt: scrivimi un riassunto sul cambiamento climatico
```
The prompt is vague, so the skill first asks for the missing information (purpose and audience, length limit) with multiple-choice questions. After your answers it returns the improved prompt in a code block, followed by the main changes and the choices made on your behalf. If the prompt is already complete, the rewrite comes immediately.

### License
MIT. See [LICENSE](LICENSE). Author: Alessandro ([GitHub profile](https://github.com/brune1)).
