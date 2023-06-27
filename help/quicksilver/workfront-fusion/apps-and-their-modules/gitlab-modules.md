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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '4485'
ht-degree: 0%

---


# [!UICONTROL GitLab] moduli

Adobe Workfront Fusion richiede una licenza Adobe Workfront Fusion oltre a una licenza Adobe Workfront.

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL GitLab], oltre a collegarlo a più applicazioni e servizi di terze parti.

>[!NOTE]
>
>Questo articolo richiede una certa familiarità con la documentazione API e con [!DNL GitLab] funzionalità in generale.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o versione successiva</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
      <td>Immetti l’URL del [!DNL GitLab] dell'istanza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token di accesso]</td> 
      <td><p>Immetti il [!UICONTROL Private Token] o [!UICONTROL Personal Access Token].</p><p>Per informazioni su come individuare o creare un token di accesso personale in [!DNL GitLab], vedi "Creare un token di accesso personale" in <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Token di accesso personali</a> nel [!DNL GitLab] documentazione.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Clic **[!UICONTROL Continua]**.
1. Clic **[!UICONTROL Autorizza]** per creare la connessione e tornare al modulo.

## [!DNL GitLab] moduli e relativi campi

Quando si configura [!DNL GitLab] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL GitLab] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

+++**[!UICONTROL Guarda lo stato della build]**

Questo modulo di attivazione immediata avvia uno scenario quando lo stato di una build cambia.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Il progetto per il quale si desidera che il webhook controlli le modifiche di stato della build</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osserva commenti commit/MR/issue/snippet]**

Questo modulo di attivazione immediata avvia uno scenario quando viene aggiunto un commento su un commit, una richiesta di unione, un problema o uno snippet di codice.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto per il quale si desidera che il webhook controlli i commenti</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Conferme di controllo (push)]**

Questo modulo di attivazione immediata avvia uno scenario quando un commit viene inviato a un archivio. Questo modulo non avvia uno scenario quando viene inviato un tag.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto per il quale si desidera che il webhook controlli i commit</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osserva commento problema]**

Questo modulo di attivazione immediata avvia uno scenario quando viene aggiunto un commento su un problema.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto che desideri venga controllato dal webhook per i commenti sui problemi</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda i problemi]**

Questo [!UICONTROL trigger istantaneo] Il modulo avvia uno scenario quando viene creato un problema o quando un problema esistente viene aggiornato, chiuso o riaperto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Il progetto che desideri che il webhook controlli per i problemi</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osservare le richieste di unione]**

Questo modulo di attivazione immediata avvia uno scenario quando si verifica una delle seguenti situazioni:

* Viene creata una nuova richiesta di unione
* Una richiesta di unione esistente viene aggiornata, unita o chiusa
* Viene aggiunto un commit nel ramo di origine


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto che il webhook deve controllare per le richieste di unione</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osservare i commenti della richiesta di unione]**

Questo modulo di attivazione immediata avvia uno scenario quando viene aggiunto un commento a una richiesta di unione.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto per il quale si desidera che il webhook controlli i commenti della richiesta di unione</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Monitorare lo stato della pipeline]**

Questo modulo di attivazione immediata avvia uno scenario quando lo stato di una pipeline cambia.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Il progetto per il quale si desidera che il webhook controlli le modifiche di stato della pipeline</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda i progetti]**

Questo modulo di attivazione pianificato avvia uno scenario quando viene aggiunto un nuovo progetto di cui l’utente autenticato è membro.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL GitLab] account a [!DNL Workfront] Fusion, vedi <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connetti [!DNL GitLab] a [!DNL Workfront] Fusion</a> in questo articolo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Risultati Max</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve controllare durante ogni ciclo di esecuzione dello scenario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osservare i rami dell’archivio]**

Questo modulo di trigger pianificato avvia uno scenario quando viene aggiunto un nuovo ramo a un archivio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL GitLab] account a [!DNL Workfront] Fusion, vedi <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connetti [!DNL GitLab] a [!DNL Workfront] Fusion</a> in questo articolo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Risultati Max</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve controllare durante ogni ciclo di esecuzione dello scenario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osservare i tag dell’archivio]**

Questo modulo di attivazione immediata avvia uno scenario quando un tag viene creato o eliminato in un archivio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto per il quale si desidera che il webhook controlli i tag</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Osserva commenti frammento]**

Questo modulo di attivazione immediata avvia uno scenario quando viene aggiunto un nuovo commento su uno snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto per il quale si desidera che il webhook controlli i commenti</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Guarda le cose da fare]**

Questo modulo di attivazione pianificato avvia uno scenario quando viene aggiunto un nuovo oggetto. Se non viene applicato alcun filtro, il trigger viene eseguito quando viene aggiunto un nuovo oggetto in sospeso.

Per informazioni sui campi, consulta [Ottieni un elenco di cose da fare](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Guarda la pagina wiki]**

Questo modulo di attivazione immediata avvia uno scenario quando viene creata o modificata una pagina wiki.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleziona il webhook da utilizzare per questo trigger o aggiungi un nuovo webhook. </p><p>Per aggiungere un nuovo webhook: <ol><li>Clic <b>[!UICONTROL Add]</b> accanto al campo [!UICONTROL webhook].</li><li>Immetti quanto segue: <ul><li>Nome del webhook</li><li>Connessione da utilizzare per questo webhook</li><li>Progetto che si desidera che il webhook controlli per le pagine wiki</li></ul></li><li>Clic <b>[!UICONTROL Salva]</b> per salvare il webhook e tornare al modulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Azioni

+++**[!UICONTROL Accetta richiesta di unione]**

Questo modulo di azione unisce le modifiche inviate alla richiesta di unione specificata.

Per informazioni sui campi, consulta [Accetta richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Annullare una build]**

Questo modulo di azione annulla una singola build di un progetto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per istruzioni sulla connessione [!DNL GitLab] account a [!DNL Workfront] Fusion, vedi <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connetti [!DNL GitLab] a [!DNL Workfront] Fusion</a> in questo articolo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p>Seleziona o mappa il progetto che contiene la build da annullare.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td>Seleziona o mappa la build da annullare.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Merge commit message]</td> 
   <td> Immettere o mappare un messaggio di commit per l'unione.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Deve rimuovere il ramo di origine]</td> 
   <td>Selezionare se si desidera rimuovere il ramo di origine al termine dell'unione.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Unisci quando la compilazione riesce]</td> 
   <td>Seleziona se unire la richiesta di unione non appena la build viene completata.</td> 
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

Per informazioni sui campi, consulta [Annullare i processi di una pipeline](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Annulla unione al completamento della pipeline]**

Se una richiesta di unione è impostata per essere unita quando una pipeline viene eseguita correttamente, questo modulo di azione annulla l’azione.

Per informazioni sui campi, consulta [Annulla unione al completamento della pipeline](https://docs.gitlab.com/ee/api/merge_requests.html) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Cherry scegli un commit]**

Questo modulo di azione seleziona un commit per un determinato ramo.

Per informazioni sui campi, consulta [Cherry scegli un commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea una nuova etichetta]**

Questo modulo di azione crea una nuova etichetta per l’archivio specificato.

Per informazioni sui campi, consulta [Crea una nuova etichetta](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una nuova pipeline]**

Questo modulo di azione crea una nuova pipeline per il progetto specificato.

Per informazioni sui campi, consulta [Creare una nuova pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una nuova versione]**

Questo modulo di azione aggiunge note sulla versione al tag Git esistente.

Per informazioni sui campi, consulta [Creare una versione](https://docs.gitlab.com/ee/api/releases/#create-a-release) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea un nuovo tag]**

Questo modulo di azione crea un nuovo tag nell’archivio che punta al riferimento fornito.

Per informazioni sui campi, consulta [Crea un nuovo tag](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare una attività]**

Questo modulo di azione crea una attività per l’utente corrente sul problema selezionato. L’utente corrente è l’utente identificato dalle credenziali sulla connessione utilizzata per questo modulo.

Per informazioni sui campi, consulta [Creare un’attività](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Creare un’attività in una richiesta di unione]**

Questo modulo di azione crea un token per l’utente corrente nella richiesta di unione selezionata. L’utente corrente è l’utente identificato dalle credenziali sulla connessione utilizzata per questo modulo.

Per informazioni sui campi, consulta [Creare una cosa da fare](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea richiesta di unione]**

Questo modulo di azione crea una nuova richiesta di unione su un progetto.

Per informazioni sui campi, consulta [Crea richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuovo file nel repository]**

Questo modulo di azione crea un nuovo file nell’archivio selezionato.

Per informazioni sui campi, consulta [Crea nuovo file nel repository](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuova nota problema]**

Questo modulo di azione crea una nota di problema per un singolo problema di progetto.

Per informazioni sui campi, consulta [Crea nuova nota problema](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuova nota di richiesta di unione]**

Questo modulo di azione crea una nota per una singola richiesta di unione.

Per informazioni sui campi, consulta [Crea nuova nota di richiesta di unione](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea una nuova milestone]**

Questo modulo di azione crea una nuova milestone per un progetto.

Per informazioni sui campi, consulta [Crea nuova milestone](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea nuova nota frammento]**

Questo modulo di azione crea una nuova nota per un singolo frammento. Le note dello snippet sono commenti che gli utenti possono pubblicare su uno snippet.

Per informazioni sui campi, consulta [Crea nuova nota frammento](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea ramo dell’archivio]**

Questo modulo di azione crea un singolo ramo dell’archivio.

Per informazioni sui campi, consulta [Crea ramo dell’archivio](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Crea variabile di build]**

Questo modulo di azione crea una nuova variabile di build.

Per informazioni sui campi, consulta [Crea variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Eliminare una richiesta di unione]**

Questo modulo di azione è destinato solo agli amministratori e ai proprietari dei progetti. Elimina la richiesta di unione in questione

Per informazioni sui campi, consulta [Eliminare una richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elimina file esistente nel repository]**

Questo modulo di azione elimina un file esistente dal repository.

Per informazioni sui campi, consulta [Elimina file esistente nel repository](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elimina ramo archivio]**

Questo modulo di azione elimina un ramo dall’archivio.

Per informazioni sui campi, consulta [Elimina ramo archivio](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica problema]**

Questo modulo di azione aggiorna un problema di progetto esistente. Questa chiamata viene utilizzata anche per contrassegnare un problema come chiuso.

Per informazioni sui campi, consulta [Modifica problema](https://docs.gitlab.com/ee/api/issues.html#edit-issue) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica Milestone]**
Questo modulo di azione aggiorna una milestone di progetto esistente.

Per informazioni sui campi, consulta [Modifica milestone](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Cancellare una build]**

Questo modulo di azione cancella la build di un progetto (rimuove gli artefatti del processo e il registro di processo).

Per informazioni sui campi, consulta [Cancellare un processo](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un elenco di attività]**

Questo modulo di ricerca recupera un elenco di cose da fare.

Per informazioni sui campi, consulta [Ottieni un elenco di cose da fare](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una singola build]**

Questo modulo di azione recupera un singolo processo di un progetto.

Per informazioni sui campi, consulta [Ottieni un singolo lavoro](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un singolo tag archivio]**

Questo modulo di azione recupera un tag specifico dell’archivio determinato dal suo nome.

Per informazioni sui campi, consulta [Ottieni un singolo tag archivio](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottenere una distribuzione specifica]**

Questo modulo di azione recupera una distribuzione specifica.

Per informazioni sui campi, consulta [Ottenere una distribuzione specifica](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni tutti i problemi assegnati a un&#39;unica milestone]**

Questo modulo di ricerca recupera tutti i problemi assegnati a un singolo progetto milestone.

Per informazioni sui campi, consulta [Ottieni tutti i problemi assegnati a un&#39;unica milestone](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni file dal repository]**

Questo modulo di azione recupera informazioni su un file nell’archivio come nome, dimensione o contenuto.

Per informazioni sui campi, consulta [Ottieni file dal repository](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni utenti progetto]**

Questo modulo di ricerca recupera gli utenti del progetto.

Per informazioni sui campi, consulta [Ottieni utenti progetto](https://docs.gitlab.com/ee/api/projects.html#get-project-users) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un singolo problema]**

Questo modulo recupera i dettagli del problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per creare una nuova connessione, vedi <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Progetto [!UICONTROL]</td> 
   <td> <p>Seleziona il progetto contenente il problema di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID problema]</td> 
   <td> <p>Inserisci o mappa il nome del problema di cui desideri recuperare i dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Ottieni una singola nota sul problema]**

Questo modulo di azione recupera una singola nota per un problema di progetto specifico.

Per informazioni sui campi, consulta [Ottieni una singola nota sul problema](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una singola richiesta di unione]**

Questo modulo di azione recupera informazioni su una singola richiesta di unione.

Per informazioni sui campi, consulta [Ottieni una singola richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni singole modifiche richieste di unione]**

Questo modulo di ricerca recupera informazioni sulla richiesta di unione, inclusi i relativi file e le modifiche.

Per informazioni sui campi, consulta [Ottieni singole modifiche richieste di unione](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni commit di richiesta di unione singola]**

Questo modulo di azione recupera un elenco di commit di richieste di unione.

Per informazioni sui campi, consulta [Ottieni commit di richiesta di unione singola](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una singola nota di richiesta di unione]**

Questo modulo di azione restituisce una singola nota per una determinata richiesta di unione.

Per informazioni sui campi, consulta [Ottieni una singola nota di richiesta di unione](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un milestone]**

Questo modulo di azione recupera i dettagli delle milestone.

Per informazioni sui campi, consulta [Ottieni singola milestone](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni progetto singolo]**

Questo modulo recupera i dettagli del progetto.

Per informazioni sui campi, consulta [Ottieni progetto singolo](https://docs.gitlab.com/ee/api/projects.html#get-single-project) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni un singolo ramo dell’archivio]**

Questo modulo di azione recupera i dettagli del ramo dell’archivio.

Per informazioni sui campi, consulta [Ottieni un singolo ramo dell’archivio](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni nota frammento]**

Questo modulo recupera una singola nota per uno snippet specifico.

Per informazioni sui campi, consulta [Ottieni una singola nota frammento](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottenere i commenti di un commit]**

Questo modulo di ricerca recupera i commenti di un commit in un progetto.

Per informazioni sui campi, consulta [Ottenere i commenti di un commit](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottenere la differenza di un commit]**

Questo modulo di azione ottiene la differenza di un commit in un progetto.

Per informazioni sui campi, consulta [Ottenere la differenza di un commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Mantieni artefatti]**

Impedisce l&#39;eliminazione degli artefatti quando è impostata la scadenza.

Per informazioni sui campi, consulta [Mantieni artefatti](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca tutte le note della richiesta di unione]**

Questo modulo di ricerca recupera un elenco di tutte le note per una singola richiesta di unione.

Per informazioni sui campi, consulta [Elenca tutte le note della richiesta di unione](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca tutte le note frammento]**

Questo modulo ottiene un elenco di tutte le note per un singolo snippet. Le note dello snippet sono commenti che gli utenti possono pubblicare su uno snippet.

Per informazioni sui campi, consulta [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le build di commit]**

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
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p>Selezionare il progetto contenente il commit per il quale si desidera elencare le build.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ambito]</td> 
   <td> Per limitare la ricerca alla generazione con uno stato specifico, seleziona lo stato. Se si lascia vuoto questo campo, vengono restituite tutte le build del commit.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Elencare i problemi]**

Questo modulo di ricerca restituisce tutti i problemi in base alle impostazioni del filtro specificate.

Per informazioni sui campi, consulta [Elencare i problemi](https://docs.gitlab.com/ee/api/issues.html#list-issues) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca i problemi che si chiudono al momento dell’unione]**

Questo modulo di ricerca recupera tutti i problemi che verrebbero chiusi unendo la richiesta di unione fornita.

Per informazioni sui campi, consulta [Elenca i problemi che verranno chiusi al momento dell’unione](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Etichette elenco]**

Questo modulo di ricerca recupera tutte le etichette nel progetto.

Per informazioni sui campi, consulta [Etichette elenco](https://docs.gitlab.com/ee/api/labels.html#list-labels) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare richieste di unione]**

Questo modulo di ricerca recupera tutte le richieste di unione in base alle impostazioni del filtro.

Per informazioni sui campi, consulta [Elencare richieste di unione](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca progetti di proprietà]**

Questo modulo di ricerca recupera i progetti in cui l’utente autenticato è impostato come proprietario.

Per informazioni sui campi, consulta [Elencare progetti utente](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le build dei progetti]**

Questo modulo di ricerca recupera un elenco di build in un progetto.

Per informazioni sui campi, consulta [Elencare processi di progetto](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare distribuzioni di progetti]**

Questo modulo di ricerca recupera un elenco di distribuzioni in un progetto.

Per informazioni sui campi, consulta [Elencare distribuzioni di progetti](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le note sui problemi del progetto]**

Questo modulo di ricerca recupera un elenco di tutte le note per un singolo problema.

Per informazioni sui campi, consulta [Elencare le note sui problemi del progetto](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare i problemi del progetto]**

Questo modulo di ricerca restituisce tutti i problemi di un progetto specificato.

Per informazioni sui campi, consulta [Elencare i problemi del progetto](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le fasi cardine del progetto]**

Questo modulo di ricerca recupera tutte le milestone nel progetto.

Per informazioni sui campi, consulta [Elencare le fasi cardine del progetto](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le pipeline dei progetti]**

Questo modulo di ricerca recupera tutte le pipeline per il progetto.

Per informazioni sui campi, consulta [Elencare le pipeline dei progetti](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare i tag dell’archivio del progetto]**

Questo modulo di ricerca recupera un elenco di tag del repository da un progetto, ordinati per nome in ordine alfabetico inverso.

Per informazioni sui campi, consulta [Elencare i tag dell’archivio del progetto](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare le variabili di progetto]**

Questo modulo di ricerca recupera un elenco delle variabili di un progetto.

Per informazioni sui campi, consulta [Elencare le variabili di progetto](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare progetti]**

Questo modulo di ricerca recupera tutti i progetti di cui l’utente autenticato è membro.

Per informazioni sui campi, consulta [Elenca tutti i progetti](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca rami archivio]**

Questo modulo cerca i rami dell’archivio in base al termine di ricerca.

Per informazioni sui campi, consulta [Elenca rami archivio](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elenca commit archivio]**

Questo modulo di ricerca recupera un elenco di commit dell’archivio in un progetto.

Per informazioni sui campi, consulta [Elenca commit archivio](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Elencare i collaboratori dell’archivio]**

Questo modulo di ricerca recupera un elenco di collaboratori dell’archivio.

Per informazioni sui campi, consulta [Collaboratori](https://docs.gitlab.com/ee/api/repositories.html#contributors) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Struttura dell’archivio elenchi]**

Questo modulo di ricerca recupera un elenco di file e directory del repository in un progetto.

Per informazioni sui campi, consulta [Struttura dell’archivio elenchi](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Contrassegna un attività come completata]**

Questo modulo di azione contrassegna come completato un singolo elemento da fare in sospeso fornito dal relativo ID per l’utente corrente.

Per informazioni sui campi, consulta [Contrassegna un elemento da fare come completato](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica nota problema esistente]**

Modifica una nota esistente di un problema.

Per informazioni sui campi, consulta [Modifica nota problema esistente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica nota richiesta di unione esistente]**

Modifica la nota esistente di una richiesta di unione.

Per informazioni sui campi, consulta [Modifica nota richiesta di unione esistente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Modifica nota frammento esistente]**

Questo modulo modifica una nota esistente di uno snippet.

Per informazioni sui campi, consulta [Modifica nota frammento esistente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Nuovo problema]**

Questo modulo di azione crea un nuovo problema di progetto.

Per informazioni sui campi, consulta [Nuovo problema](https://www.integromat.com/en/help/app/gitlab) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Riproduci una build]**

Questo modulo di azione attiva un’azione manuale per avviare un processo.

Per informazioni sui campi, consulta [Riproduci un processo](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Pubblica commento da confermare]**

Questo modulo di azione aggiunge un commento a un commit.

Per informazioni sui campi, consulta [Pubblica commento da confermare](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Rimuovi variabile]**

Questo modulo di azione rimuove la variabile di un progetto.

Per informazioni sui campi, consulta [Rimuovi variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Riprovare una build]**

Questo modulo di azione tenta nuovamente una singola build in un commit.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Per creare una nuova connessione, vedi <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> in questo articolo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID progetto]</td> 
   <td> <p>Seleziona il progetto contenente la build da riprovare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td> Seleziona la build da riprovare. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Ritentare i processi non riusciti in una pipeline]**

Questo modulo di azione tenta nuovamente le build non riuscite in una pipeline.

Per informazioni sui campi, consulta [Ritentare i processi in una pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Ottieni una variabile]**

Questo modulo recupera i dettagli della variabile specifica di un progetto.

Per informazioni sui campi, consulta [Mostra dettagli variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Aggiornare una versione]**

Questo modulo di azione aggiorna una versione.

Per informazioni sui campi, consulta [Aggiornare una versione](https://docs.gitlab.com/ee/api/releases/#update-a-release) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Aggiorna richiesta di unione]**

Questo modulo di azione aggiorna una richiesta di unione esistente. È possibile modificare il ramo di destinazione, il titolo o anche chiudere MR.

Per informazioni sui campi, consulta [Aggiorna richiesta di unione](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) nel [!DNL GitLab] documentazione.

+++

+++**[!UICONTROL Aggiornare una variabile]**

Questo modulo di azione aggiorna la variabile di un progetto.

Per informazioni sui campi, consulta [Aggiorna variabile](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) nel [!DNL GitLab] documentazione.

+++
