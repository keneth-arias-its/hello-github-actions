## Step 2: Aggiungi un job al workflow

Ottimo lavoro! :tada: Hai aggiunto il file del workflow.

### 📖 Teoria: Introduzione ai job

Un [job](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions#jobs) è un gruppo di step che vengono eseguiti insieme sullo stesso [runner](https://docs.github.com/en/actions/using-github-hosted-runners/using-github-hosted-runners/about-github-hosted-runners), all'interno di un workflow. Ogni job è definito nella sezione `jobs` e, per impostazione predefinita, viene eseguito in modo indipendente e in parallelo.

I job ti aiutano a organizzare il workflow in unità logiche, per esempio build, test o deployment del codice.

> [!Tip]
> Puoi eseguire lo stesso job con più [variazioni usando una strategia a matrice](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/running-variations-of-jobs-in-a-workflow).

### ⌨️ Attività: Aggiungi un job al workflow

1. Nel branch `welcome-workflow`, apri il tuo file `.github/workflows/welcome.yml`.

1. Modifica il file aggiungendo la sezione `jobs` e un job chiamato `welcome`, che verrà eseguito sull'ultima versione disponibile di Ubuntu.

   ```yaml
   name: Post welcome comment
   on:
     pull_request:
       types: [opened]
   permissions:
     pull-requests: write
   jobs:
     welcome:
       name: Post welcome comment
       runs-on: ubuntu-latest
   ```

1. Fai il commit delle modifiche nel branch `welcome-workflow`.

1. Dopo aver aggiunto il job, Octocat esaminerà il tuo lavoro e sbloccherà lo step successivo dell'esercizio.

<details>
<summary>Hai problemi? 🤷</summary><br/>

- Assicurati che la sezione `jobs` sia indentata correttamente nel tuo file YAML.
- Verifica di stare modificando il file e il branch corretti.

</details>
