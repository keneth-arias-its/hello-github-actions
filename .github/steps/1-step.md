## Step 1: Crea il file del workflow

### 📖 Teoria: Introduzione ai workflow

Un **workflow** è un processo automatizzato che definisci nel tuo repository. I workflow sono descritti in file YAML salvati nella directory `.github/workflows`. Ogni workflow viene attivato da [eventi](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows) specifici che si verificano nel repository, come l'apertura di una pull request, il push del codice o la creazione di una issue.

I workflow ti permettono di automatizzare attività come la compilazione del codice (build), i test o il deployment. Possono rispondere a quasi tutte le attività del tuo progetto.

> [!NOTE]
> Per approfondire, consulta queste risorse:
> - [Comprendere GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions)
> - [Eventi che attivano i workflow](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows)
> - [Prezzi dei runner Actions](https://docs.github.com/en/billing/reference/actions-runner-pricing)

### ⌨️ Attività: Crea il file del workflow

1. Apri questo repository in una nuova scheda del browser: potrai lavorare sugli step mentre leggi le istruzioni in questa scheda.

1. Nella scheda **Code** del tuo repository, crea un nuovo branch chiamato `welcome-workflow`.

   <img width="400" alt="screenshot della creazione del branch" src="https://github.com/IDT-25-27/idt-25-27-classroom-173794-hello-github-actions-hello-github-actions/blob/main/.github/images/create-branch-screenshot.png?raw=true" />

1. Nel branch `welcome-workflow`, vai alla directory `.github/workflows`.

1. Crea un nuovo file chiamato `welcome.yml` nella directory `.github/workflows` con questo contenuto:

   ```yaml
   name: Post welcome comment
   on:
     pull_request:
       types: [opened]
   permissions:
     pull-requests: write
   ```

   > [!NOTE]
   > Questo file del workflow è ancora incompleto. È normale ricevere un messaggio di errore: procederai uno step alla volta. 😎

1. Fai il commit delle modifiche direttamente nel branch `welcome-workflow`.

1. Dopo il commit, Octocat verificherà il tuo lavoro e sbloccherà lo step successivo dell'esercizio.

<details>
<summary>Hai problemi? 🤷</summary><br/>

- Assicurati di essere nel branch `welcome-workflow` quando crei il file del workflow.
- Verifica con attenzione il percorso del file e l'indentazione YAML.

</details>
