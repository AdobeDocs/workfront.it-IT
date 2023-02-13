---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli GitLab
description: Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.
author: Becky
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: d55ddd97a69f00a1f42d84dc55a12d2017855776
workflow-type: tm+mt
source-wordcount: '4370'
ht-degree: 0%

---


# [!UICONTROL GitLab] moduli

Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL GitLab], nonché collegarlo a più applicazioni e servizi di terze parti.

>[!NOTE]
>
>Questo articolo richiede una certa familiarità con la documentazione API e con [!DNL GitLab] in generale.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Connetti [!DNL GitLab] a [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. In qualsiasi [!DNL Workfront Fusion] [!DNL Gitlab] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al campo connessione.
1. Configura i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome connessione]</td> 
      <td> <p>Immettere un nome per la connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Inserisci l’URL del [!DNL GitLab] istanza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access Token]</td> 
      <td><p>Immetti il [!UICONTROL Private Token] o il [!UICONTROL Personal Access Token].</p><p>Per informazioni su come individuare o creare un token di accesso personale in [!DNL GitLab], consulta "Creare un token di accesso personale" in <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Token di accesso personale</a> in [!DNL GitLab] documentazione.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Fai clic su **[!UICONTROL Continua]**.
1. Fai clic su **[!UICONTROL Autorizzare]** per creare la connessione e tornare al modulo .

## [!DNL GitLab] moduli e relativi campi

Quando si configura [!DNL GitLab] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL GitLab] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

+++**[!UICONTROL Stato della build di controllo]**

Questo modulo di attivazione immediata avvia uno scenario in cui cambia lo stato di una build.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che desideri che il webhook controlli per verificare le modifiche dello stato della build</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda i commenti commit/MR/issue/snippet]**

Questo modulo di attivazione immediata avvia uno scenario in cui viene effettuato un commento su un commit, una richiesta di unione, un problema o un frammento di codice.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che si desidera venga controllato dal webhook per i commenti</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Commit dell&#39;orologio (push)]**

Questo modulo di attivazione immediata avvia uno scenario in cui un commit viene inviato a un archivio. Questo modulo non avvia uno scenario in cui un tag viene inviato.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Progetto che desideri che il webhook controlli per i commit</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osserva il commento del problema]**

Questo modulo di attivazione immediata avvia uno scenario in cui viene effettuato un commento su un problema.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che si desidera che il webhook controlli per i commenti dei problemi</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Problemi di controllo]**

Questo [!UICONTROL impulso immediato] Il modulo avvia uno scenario in cui viene creato un problema o quando un problema esistente viene aggiornato, chiuso o riaperto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che desideri che il webhook verifichi i problemi</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda le richieste di unione]**

Questo modulo di attivazione immediata avvia uno scenario in cui si verifica uno dei seguenti casi:

* Viene creata una nuova richiesta di unione
* Una richiesta di unione esistente viene aggiornata, unita o chiusa
* Viene aggiunto un commit nel ramo di origine


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Progetto che si desidera che il webhook controlli per le richieste di unione</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osservare i commenti della richiesta di unione]**

Questo modulo di attivazione immediata avvia uno scenario in cui viene effettuato un commento su una richiesta di unione.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Progetto che si desidera che il webhook controlli per i commenti della richiesta di unione</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Stato della pipeline di controllo]**

Questo modulo di attivazione immediata avvia uno scenario in cui lo stato di una pipeline cambia.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che si desidera che il webhook verifichi le modifiche dello stato della pipeline</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda i progetti]**

Questo modulo trigger pianificato avvia uno scenario in cui viene aggiunto un nuovo progetto, di cui l’utente autenticato è membro.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL GitLab] account a [!DNL Workfront] Fusion, vedi <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connetti [!DNL GitLab] a [!DNL Workfront] Fusion</a> in questo articolo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Risultati Max</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo visualizzi durante ogni ciclo di esecuzione degli scenari.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda i rami dell’archivio]**

Questo modulo trigger pianificato avvia uno scenario in cui viene aggiunto un nuovo ramo a un archivio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL GitLab] account a [!DNL Workfront] Fusion, vedi <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connetti [!DNL GitLab] a [!DNL Workfront] Fusion</a> in questo articolo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Risultati Max</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera che il modulo visualizzi durante ogni ciclo di esecuzione degli scenari.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda i tag dell’archivio]**

Questo modulo di attivazione immediata avvia uno scenario in cui un tag viene creato o eliminato in un archivio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che desideri che il webhook verifichi i tag</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osserva i commenti dei frammenti]**

Questo modulo di attivazione immediata avvia uno scenario in cui viene effettuato un nuovo commento su uno snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che si desidera venga controllato dal webhook per i commenti</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Strumenti di controllo]**

Questo modulo trigger pianificato avvia uno scenario in cui viene aggiunto un nuovo strumento. Quando non viene applicato alcun filtro, il trigger viene eseguito quando viene aggiunto un nuovo strumento in sospeso.

Per informazioni sui campi, consulta [Ottieni un elenco di attività](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Guarda la pagina wiki]**

Questo modulo di attivazione immediata avvia uno scenario quando viene creata o modificata una pagina wiki.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selezionare il webhook che si desidera utilizzare per questo trigger o aggiungere un nuovo webhook. </p><p>Per aggiungere un nuovo webhook, <ol><li>Fai clic su <b>[!UICONTROL Aggiungi]</b> accanto al campo del webhook [!UICONTROL].</li><li>Immetti quanto segue: <ul><li>Un nome per il gancio a ragnatela</li><li>Connessione che si desidera utilizzare per questo webhook</li><li>Il progetto che desideri che il webhook guardi per le pagine wiki</li></ul></li><li>Fai clic su <b>[!UICONTROL Save]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Azioni

+++**[!UICONTROL Accetta richiesta di unione]**

Questo modulo di azione unisce le modifiche inviate alla richiesta di unione specificata.

Per informazioni sui campi, consulta [Accetta richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Annullare una build]**

Questo modulo di azione annulla una singola build di un progetto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni su come collegare le [!DNL GitLab] account a [!DNL Workfront] Fusion, vedi <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connetti [!DNL GitLab] a [!DNL Workfront] Fusion</a> in questo articolo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Seleziona o mappa il progetto che contiene la build da annullare.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID build]</td> 
   <td>Seleziona o mappa la build da annullare.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Unisci messaggio commit]</td> 
   <td> Immettere o mappare un messaggio di commit per l'unione.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Rimuovi ramo di origine]</td> 
   <td>Selezionare se si desidera rimuovere il ramo di origine al termine dell'unione.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Unisci quando la build ha esito positivo]</td> 
   <td>Seleziona se unire la richiesta di unione non appena la build è stata completata.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>Se presente, questo SHA deve corrispondere al HEAD del ramo di origine. Se non corrisponde, l'unione non riesce.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Annullare le build di una pipeline]**

Questo modulo di azione annulla le build per una singola pipeline.

Per informazioni sui campi, consulta [Annullare i lavori di una pipeline](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Annulla unione quando la pipeline ha esito positivo]**

Se una richiesta di unione viene impostata per l’unione quando una pipeline ha esito positivo, questo modulo di azione annulla tale azione.

Per informazioni sui campi, consulta [Annulla unione quando la pipeline ha esito positivo](https://docs.gitlab.com/ee/api/merge_requests.html) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ciliegia scegliere un commit]**

Questa ciliegia del modulo di azione sceglie un commit per un determinato ramo.

Per informazioni sui campi, consulta [Ciliegia scegliere un commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una nuova etichetta]**

Questo modulo di azione crea una nuova etichetta per il repository specificato.

Per informazioni sui campi, consulta [Creare una nuova etichetta](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una nuova pipeline]**

Questo modulo di azione crea una nuova pipeline per il progetto specificato.

Per informazioni sui campi, consulta [Creare una nuova pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una nuova versione]**

Questo modulo di azione aggiunge note sulla versione al tag git esistente.

Per informazioni sui campi, consulta [Creare una versione](https://docs.gitlab.com/ee/api/releases/#create-a-release) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare un nuovo tag]**

Questo modulo di azione crea un nuovo tag nel repository che punta al riferimento fornito.

Per informazioni sui campi, consulta [Creare un nuovo tag](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare uno strumento]**

Questo modulo di azione crea uno strumento per l’utente corrente sul problema selezionato. L&#39;utente corrente è l&#39;utente identificato dalle credenziali sulla connessione utilizzata per questo modulo.

Per informazioni sui campi, consulta [Crea un](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare uno strumento su una richiesta di unione]**

Questo modulo di azione crea uno strumento per l&#39;utente corrente nella richiesta di unione selezionata. L&#39;utente corrente è l&#39;utente identificato dalle credenziali sulla connessione utilizzata per questo modulo.

Per informazioni sui campi, consulta [Creare un](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea richiesta di unione]**

Questo modulo di azione crea una nuova richiesta di unione su un progetto.

Per informazioni sui campi, consulta [Crea richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuovo file nell&#39;archivio]**

Questo modulo di azione crea un nuovo file nell’archivio selezionato.

Per informazioni sui campi, consulta [Crea nuovo file nell&#39;archivio](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuova nota del problema]**

Questo modulo di azione crea una nota di problema per un singolo problema di progetto.

Per informazioni sui campi, consulta [Crea nuova nota del problema](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuova nota di richiesta di unione]**

Questo modulo di azione crea una nota per una singola richiesta di unione.

Per informazioni sui campi, consulta [Crea nuova nota di richiesta di unione](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una nuova pietra miliare]**

Questo modulo di azione crea una nuova fase cardine per un progetto.

Per informazioni sui campi, consulta [Creare una nuova pietra miliare](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuova nota di frammento]**

Questo modulo di azione crea una nuova nota per un singolo frammento. Le note di snippet sono commenti che gli utenti possono inviare a uno snippet.

Per informazioni sui campi, consulta [Crea nuova nota di frammento](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea ramo archivio]**

Questo modulo di azione crea un singolo ramo archivio.

Per informazioni sui campi, consulta [Crea ramo archivio](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una variabile di compilazione]**

Questo modulo di azione crea una nuova variabile di compilazione.

Per informazioni sui campi, consulta [Crea variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Eliminare una richiesta di unione]**

Questo modulo di azione è riservato agli amministratori e ai proprietari del progetto. Elimina la richiesta di unione in questione

Per informazioni sui campi, consulta [Eliminare una richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elimina il file esistente nella directory archivio]**

Questo modulo di azione elimina un file esistente dall’archivio.

Per informazioni sui campi, consulta [Elimina il file esistente nella directory archivio](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elimina ramo archivio]**

Questo modulo di azione elimina un ramo dall’archivio.

Per informazioni sui campi, consulta [Elimina ramo archivio](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica problema]**

Questo modulo di azione aggiorna un problema di progetto esistente. Questa chiamata viene utilizzata anche per contrassegnare un problema come chiuso.

Per informazioni sui campi, consulta [Modifica problema](https://docs.gitlab.com/ee/api/issues.html#edit-issue) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica Milestone]**
Questo modulo di azione aggiorna una fase cardine del progetto esistente.

Per informazioni sui campi, consulta [Modifica cardine](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Cancellare una build]**

Questo modulo di azione cancella una build di un progetto (rimuove gli artefatti di lavoro e il registro di lavoro).

Per informazioni sui campi, consulta [Cancellare un lavoro](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un elenco di strumenti]**

Questo modulo di ricerca recupera un elenco di elementi da eseguire.

Per informazioni sui campi, consulta [Ottieni un elenco di attività](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una singola build]**

Questo modulo di azione recupera un singolo processo di un progetto.

Per informazioni sui campi, consulta [Ottieni un singolo lavoro](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un singolo tag archivio]**

Questo modulo di azione recupera un tag archivio specifico determinato dal suo nome.

Per informazioni sui campi, consulta [Ottieni un singolo tag archivio](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una distribuzione specifica]**

Questo modulo di azione recupera una distribuzione specifica.

Per informazioni sui campi, consulta [Ottieni una distribuzione specifica](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottenere tutti i problemi assegnati a un singolo cardine]**

Questo modulo di ricerca recupera tutti i problemi assegnati a un singolo progetto cardine.

Per informazioni sui campi, consulta [Ottenere tutti i problemi assegnati a un singolo cardine](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni file dal repository]**

Questo modulo di azione recupera informazioni su un file nell&#39;archivio come nome, dimensione o contenuto.

Per informazioni sui campi, consulta [Ottieni file dal repository](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni utenti del progetto]**

Questo modulo di ricerca recupera gli utenti del progetto.

Per informazioni sui campi, consulta [Ottieni utenti del progetto](https://docs.gitlab.com/ee/api/projects.html#get-project-users) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un singolo problema]**

Questo modulo di azione recupera i dettagli del problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per creare una nuova connessione, vedi <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>Seleziona il progetto che contiene il problema di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID problema]</td> 
   <td> <p>Immetti o mappa il nome del problema di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Ottieni una singola nota del problema]**

Questo modulo di azione recupera una singola nota per un problema specifico del progetto.

Per informazioni sui campi, consulta [Ottieni una singola nota del problema](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni richiesta di unione singola]**

Questo modulo di azione recupera informazioni su una singola richiesta di unione.

Per informazioni sui campi, consulta [Ottieni richiesta di unione singola](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni modifiche a richiesta di unione singola]**

Questo modulo di ricerca recupera le informazioni sulla richiesta di unione, compresi i relativi file e le modifiche.

Per informazioni sui campi, consulta [Ottieni modifiche a richiesta di unione singola](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni commit di richiesta di unione singola]**

Questo modulo di azione recupera un elenco di commit delle richieste di unione.

Per informazioni sui campi, consulta [Ottieni commit di richiesta di unione singola](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una nota di richiesta di unione singola]**

Questo modulo di azione restituisce una singola nota per una richiesta di unione specificata.

Per informazioni sui campi, consulta [Ottieni una nota di richiesta di unione singola](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottenere un Milestone]**

Questo modulo di azione recupera i dettagli della cardine.

Per informazioni sui campi, consulta [Ottieni una sola pietra miliare](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni progetto singolo]**

Questo modulo di azione recupera i dettagli del progetto.

Per informazioni sui campi, consulta [Ottieni progetto singolo](https://docs.gitlab.com/ee/api/projects.html#get-single-project) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un singolo ramo archivio]**

Questo modulo di azione recupera i dettagli del ramo dell&#39;archivio.

Per informazioni sui campi, consulta [Ottieni un singolo ramo archivio](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni nota frammento]**

Questo modulo recupera una singola nota per un frammento specificato.

Per informazioni sui campi, consulta [Ottieni una singola nota di frammento](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni i commenti di un commit]**

Questo modulo di ricerca recupera i commenti di un commit in un progetto.

Per informazioni sui campi, consulta [Ottieni i commenti di un commit](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni il diff di un commit]**

Questo modulo di azione ottiene la differenza di un commit in un progetto.

Per informazioni sui campi, consulta [Ottieni il diff di un commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Mantieni artefatti]**

Impedisce l’eliminazione degli artefatti quando è impostata la scadenza.

Per informazioni sui campi, consulta [Mantieni artefatti](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca tutte le note della richiesta di unione]**

Questo modulo di ricerca recupera un elenco di tutte le note per una singola richiesta di unione.

Per informazioni sui campi, consulta [Elenca tutte le note della richiesta di unione](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca tutte le note di frammento]**

Questo modulo ottiene un elenco di tutte le note per un singolo snippet. Le note di snippet sono commenti che gli utenti possono inviare a uno snippet.

Per informazioni sui campi, consulta [?](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare build di commit]**

Questo modulo di ricerca restituisce un elenco di build per un commit specifico in un progetto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per creare una nuova connessione, vedi <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Seleziona il progetto che contiene il commit per il quale vuoi elencare le build.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ambito [!UICONTROL]</td> 
   <td> Per limitare la ricerca alla creazione con uno stato specifico, seleziona lo stato . Se questo campo viene lasciato vuoto, vengono restituite tutte le build del commit.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Problemi elenco]**

Questo modulo di ricerca restituisce tutti i problemi relativi alle impostazioni di filtro specificate.

Per informazioni sui campi, consulta [Problemi elenco](https://docs.gitlab.com/ee/api/issues.html#list-issues) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenco dei problemi che si chiudono durante l&#39;unione]**

Questo modulo di ricerca recupera tutti i problemi che verrebbero chiusi unendo la richiesta di unione fornita.

Per informazioni sui campi, consulta [Elencare i problemi che si chiuderanno in caso di unione](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Etichette elenco]**

Questo modulo di ricerca recupera tutte le etichette nel progetto.

Per informazioni sui campi, consulta [Etichette elenco](https://docs.gitlab.com/ee/api/labels.html#list-labels) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare richieste di unione]**

Questo modulo di ricerca recupera tutte le richieste di unione dalle impostazioni del filtro.

Per informazioni sui campi, consulta [Elencare richieste di unione](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca progetti di proprietà]**

Questo modulo di ricerca recupera i progetti in cui l’utente autenticato è impostato come proprietario.

Per informazioni sui campi, consulta [Elencare progetti utente](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare build di progetto]**

Questo modulo di ricerca recupera un elenco di build in un progetto.

Per informazioni sui campi, consulta [Elencare processi di progetto](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare distribuzioni di progetti]**

Questo modulo di ricerca recupera un elenco di implementazioni in un progetto.

Per informazioni sui campi, consulta [Elencare distribuzioni di progetti](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le note sui problemi del progetto]**

Questo modulo di ricerca recupera un elenco di tutte le note per un singolo problema.

Per informazioni sui campi, consulta [Elencare le note sui problemi del progetto](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare i problemi del progetto]**

Questo modulo di ricerca restituisce tutti i problemi in un progetto specificato.

Per informazioni sui campi, consulta [Elencare i problemi del progetto](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le fasi cardine del progetto]**

Questo modulo di ricerca recupera tutte le tappe del progetto.

Per informazioni sui campi, consulta [Elencare le fasi cardine del progetto](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare pipeline di progetto]**

Questo modulo di ricerca recupera tutte le pipeline per il progetto.

Per informazioni sui campi, consulta [Elencare pipeline di progetto](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca tag archivio progetti]**

Questo modulo di ricerca recupera un elenco di tag archivio da un progetto, ordinati per nome in ordine alfabetico inverso.

Per informazioni sui campi, consulta [Elenca tag archivio progetti](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare variabili di progetto]**

Questo modulo di ricerca recupera un elenco delle variabili di un progetto.

Per informazioni sui campi, consulta [Elencare variabili di progetto](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare progetti]**

Questo modulo di ricerca recupera tutti i progetti di cui l&#39;utente autenticato è membro.

Per informazioni sui campi, consulta [Elenca tutti i progetti](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare rami del repository]**

Questo modulo cerca i rami del repository in base al termine di ricerca.

Per informazioni sui campi, consulta [Elencare rami del repository](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare i commit dell&#39;archivio]**

Questo modulo di ricerca recupera un elenco di conferme archivio in un progetto.

Per informazioni sui campi, consulta [Elencare i commit dell&#39;archivio](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare i collaboratori dell’archivio]**

Questo modulo di ricerca recupera un elenco dei collaboratori del repository.

Per informazioni sui campi, consulta [Collaboratori](https://docs.gitlab.com/ee/api/repositories.html#contributors) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenco struttura archivio]**

Questo modulo di ricerca recupera un elenco di file e directory archivio in un progetto.

Per informazioni sui campi, consulta [Elenco struttura archivio](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Contrassegna uno strumento come completato]**

Questo modulo di azione contrassegna un singolo elemento in sospeso specificato dal relativo ID per l’utente corrente come completato.

Per informazioni sui campi, consulta [Contrassegna un elemento come completato](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica nota del problema esistente]**

Modifica una nota esistente di un problema.

Per informazioni sui campi, consulta [Modifica nota del problema esistente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica nota richiesta unione esistente]**

Modifica la nota esistente di una richiesta di unione.

Per informazioni sui campi, consulta [Modifica nota richiesta unione esistente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica nota frammento esistente]**

Questo modulo di azione modifica una nota esistente di uno snippet.

Per informazioni sui campi, consulta [Modifica nota frammento esistente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Nuovo problema]**

Questo modulo di azione crea un nuovo problema di progetto.

Per informazioni sui campi, consulta [Nuovo problema](https://www.integromat.com/en/help/app/gitlab) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Riprodurre una build]**

Questo modulo di azione attiva un&#39;azione manuale per avviare un processo.

Per informazioni sui campi, consulta [Riprodurre un lavoro](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Pubblica il commento per effettuare il commit]**

Questo modulo di azione aggiunge un commento a un commit.

Per informazioni sui campi, consulta [Pubblica il commento per effettuare il commit](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Rimuovi variabile]**

Questo modulo di azione rimuove la variabile di un progetto.

Per informazioni sui campi, consulta [Rimuovi variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Riprovare a creare una build]**

Questo modulo di azione prova nuovamente una singola build in un commit.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per creare una nuova connessione, vedi <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Seleziona il progetto che contiene la build da riprovare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID build]</td> 
   <td> Seleziona la build da riprovare. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Tentativi di processi non riusciti in una pipeline]**

Questo modulo di azione prova nuovamente le build non riuscite in una pipeline.

Per informazioni sui campi, consulta [Riprova i lavori in una pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una variabile]**

Questo modulo recupera i dettagli della variabile specifica di un progetto.

Per informazioni sui campi, consulta [Mostra dettagli variabili](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Aggiornare una versione]**

Questo modulo di azione aggiorna una versione.

Per informazioni sui campi, consulta [Aggiornare una versione](https://docs.gitlab.com/ee/api/releases/#update-a-release) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Aggiorna richiesta di unione]**

Questo modulo di azione aggiorna una richiesta di unione esistente. È possibile modificare il ramo di destinazione, il titolo o anche chiudere il MR.

Per informazioni sui campi, consulta [Aggiorna richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) in [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Aggiornare una variabile]**

Questo modulo di azione aggiorna la variabile di un progetto.

Per informazioni sui campi, consulta [Aggiorna variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) in [!DNL GitLab] documentazione.

+++
