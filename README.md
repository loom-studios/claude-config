Claude Config

Repository centrale per la configurazione di Claude Code.

Contiene tutte le risorse condivise utilizzate durante lo sviluppo assistito dall'AI, come prompt, skills, documentazione, strumenti e linee guida di sviluppo. L'obiettivo è mantenere un'unica fonte di verità, evitando duplicazioni tra i vari progetti e garantendo uno stile di sviluppo coerente.

Struttura
.claude/
├── skills/      # Competenze e workflow riutilizzabili.
├── prompts/     # Prompt pronti all'uso.
├── docs/        # Documentazione e linee guida generali.

Utilizzo

Questo repository non contiene codice applicativo, ma esclusivamente configurazioni condivise.

Per ogni nuovo progetto è consigliato:

Creare un file CLAUDE.md nella root del repository con le istruzioni specifiche del progetto.
Collegare oppure copiare la cartella .claude da questo repository.
Personalizzare solo la documentazione relativa al progetto, mantenendo skills e prompt centralizzati.
Obiettivo
Centralizzare la configurazione di Claude Code.
Standardizzare il processo di sviluppo.
Riutilizzare prompt e workflow tra progetti diversi.
Ridurre la duplicazione delle configurazioni.
Migliorare progressivamente le capacità dell'assistente AI.
Manutenzione

Ogni modifica effettuata in questo repository rappresenta la configurazione di riferimento per tutti i progetti che utilizzano queste risorse.
