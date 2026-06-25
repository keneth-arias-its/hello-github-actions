## Step 5: Esegui il merge e sperimenta

_Ottimo lavoro! Hai creato e testato il tuo primo workflow di GitHub Actions!_ :rocket:

### 📖 Teoria: Quando vengono eseguiti i workflow

Quando crei un workflow in un branch, il workflow è abilitato solo per quel branch finché non esegui il merge nel branch predefinito (`main`). Quando il workflow si trova nel branch predefinito, si applica all'intero repository.

Da questo momento, ogni nuova pull request attiverà automaticamente il workflow che hai creato, indipendentemente dal branch.

> [!TIP]
> Alcuni trigger di eventi, come [workflow_dispatch](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows#workflow_dispatch) e [schedule](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows#schedule), funzionano solo se il file del workflow esiste nel branch predefinito.

### ⌨️ Attività: Esegui il merge della tua pull request

1. Esegui il merge della tua pull request nel branch `main`.

1. Prova ad aprire un'altra pull request per vedere di nuovo il workflow in esecuzione.

