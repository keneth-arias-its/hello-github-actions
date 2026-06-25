## Step 4: Attiva il workflow

_Ora hai aggiunto un workflow completamente funzionante al tuo repository! :smile:_

### 📖 Teoria: Vedere il workflow in azione

Puoi vedere tutti i workflow in esecuzione e completati nella scheda **Actions** del tuo repository.

Poiché hai configurato il workflow per essere eseguito sull'evento `pull_request`, si attiverà automaticamente quando viene aperta una pull request.

> [!TIP]
> I workflow associati alla pull request sono visibili anche nel log della pull request, vicino al pulsante di merge. Puoi anche [creare una regola](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/available-rules-for-rulesets#require-status-checks-to-pass-before-merging) che impedisce il merge se il workflow fallisce.

### ⌨️ Attività: Attiva il workflow

1. Nella scheda **Pull requests**, crea una pull request dal branch `welcome-workflow` verso `main`.

1. Controlla il commento che il workflow aggiunge alla pull request.

1. Controlla l'area vicino al pulsante di merge: dovrebbe mostrare "All checks have passed" (Tutti i controlli sono stati superati).

1. Dopo la creazione della pull request e l'attivazione del workflow, Octocat sbloccherà lo step successivo dell'esercizio.

### ⌨️ Attività: Ispeziona il workflow

1. Nella parte superiore del repository, seleziona la scheda **Actions**.

1. Nella barra laterale sinistra, seleziona il workflow chiamato **Post welcome comment**.

  > 💡 **Suggerimento:** Puoi ignorare le altre Action: servono solo a gestire questo esercizio.

1. Fai clic sulla prima esecuzione intitolata **Welcome workflow** per visualizzare il diagramma dei job.

1. Fai clic sul job chiamato **Post welcome comment** per vedere i log completi.


<details>
<summary>Hai problemi? 🤷</summary><br/>

- Controlla la scheda **Actions** per i dettagli e gli errori dell'esecuzione del workflow.

</details>
