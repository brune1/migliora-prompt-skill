# migliora-prompt-v3

🇮🇹 [Italiano](#italiano) · 🇬🇧 [English](#english)

---

## Italiano

### Descrizione
Skill per Claude che riscrive un prompt applicando le best practice ufficiali di Anthropic. Gratuita e open source.

### Cosa fa
- Prende un prompt scritto in modo vago o disordinato e lo riscrive in modo più chiaro, strutturato ed efficace, senza eseguirlo.
- Prima di riscrivere, verifica che ci siano obiettivo, ruolo, contesto e formato; se manca qualcosa, ti fa domande mirate invece di inventare.
- Mantiene la lingua e l'intento del prompt originale.
- Restituisce il prompt migliorato in un blocco da copiare e spiega in pochi punti cosa ha cambiato e perché.
- Dentro un progetto Claude, usa istruzioni, file e chat del progetto come contesto.

### Installazione

**Claude.ai (consigliato)**
1. Scarica `migliora-prompt-v3.zip` dalla [pagina Release](https://github.com/brune1/migliora-prompt-skill/releases/latest).
2. Su Claude.ai vai in **Settings → Capabilities → Skills** (il percorso può variare).
3. Carica lo ZIP e attiva la skill.

**Claude Code**
1. Scarica e decomprimi lo ZIP.
2. Copia la cartella `migliora-prompt-v3` in `~/.claude/skills/`.

**Solo copia-incolla (senza installare)**
Apri [`prompt/migliora-prompt-v3.md`](prompt/migliora-prompt-v3.md), copia il testo e incollalo all'inizio di una chat con Claude.

### Esempio d'uso
Scrivi in chat:
```
migliora questo prompt: scrivimi un riassunto sul cambiamento climatico
```
La skill non riscrive subito: prima chiede le informazioni mancanti (ruolo dell'AI, a cosa serve e chi lo leggerà, formato e lunghezza). Dopo le tue risposte restituisce il prompt migliorato in un blocco di codice, seguito dai principali cambiamenti.

### Licenza
MIT. Vedi [LICENSE](LICENSE). Autore: Alessandro ([profilo GitHub](https://github.com/brune1)).

---

## English

### Description
A Claude skill that rewrites a prompt using Anthropic's official best practices. Free and open source.

### What it does
- Takes a vague or messy prompt and rewrites it to be clearer, better structured and more effective, without executing it.
- Before rewriting, it checks that goal, role, context and output format are present; if something is missing, it asks targeted questions instead of making things up.
- Keeps the language and intent of the original prompt.
- Returns the improved prompt in a copyable block and explains in a few points what changed and why.
- Inside a Claude project, it uses the project's instructions, files and chats as context.

> Note: the skill's instructions are written in Italian, and it replies in the language of your prompt.

### Installation

**Claude.ai (recommended)**
1. Download `migliora-prompt-v3.zip` from the [Releases page](https://github.com/brune1/migliora-prompt-skill/releases/latest).
2. On Claude.ai go to **Settings → Capabilities → Skills** (the path may vary).
3. Upload the ZIP and enable the skill.

**Claude Code**
1. Download and unzip the file.
2. Copy the `migliora-prompt-v3` folder into `~/.claude/skills/`.

**Copy and paste only (no install)**
Open [`prompt/migliora-prompt-v3.md`](prompt/migliora-prompt-v3.md), copy the text and paste it at the start of a chat with Claude.

### Usage example
Type in chat:
```
migliora questo prompt: scrivimi un riassunto sul cambiamento climatico
```
The skill does not rewrite right away: it first asks for the missing information (the AI's role, purpose and audience, format and length). After your answers it returns the improved prompt in a code block, followed by the main changes.

### License
MIT. See [LICENSE](LICENSE). Author: Alessandro ([GitHub profile](https://github.com/brune1)).
