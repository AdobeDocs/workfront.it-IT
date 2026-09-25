---
title: Aggiungere un’approvazione a un modulo di richiesta in Adobe Workfront Planning
description: È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un'approvazione per ogni richiesta sottomessa, prima di creare un record.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 3b3d455ded251b06084249cf9df12c1f112f05e9
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 2%
---
# Aggiungere un’approvazione a un modulo di richiesta in Pianificazione di Adobe Workfront

<!--update the metadata with real information when making this available in TOC and in the left nav-->


<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un&#39;approvazione per ogni richiesta sottomessa, prima di creare un record.

<!--<span class="preview">Multiple stages are supported in the approval process. When all required decisions in a stage are made, the next stage begins and the new stage's approvers receive an email notification.</span>-->

Questo articolo descrive come un manager dell&#39;area di lavoro può aggiungere un&#39;approvazione a un modulo di richiesta associato a un tipo di record.

Per informazioni sulla creazione di un modulo di richiesta in Workfront Planning, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Per informazioni sull&#39;invio di una richiesta a un tipo di record per la creazione di un record, vedere [Inviare richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p></li>
Oppure
<li><p>Qualsiasi pacchetto Planning acquistato come prodotto standalone</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard flusso di lavoro</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Standard di pianificazione</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro e tipo di record</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull’aggiunta di approvazioni a un modulo di richiesta

* Puoi aggiungere uno o più approvatori (utenti o team) a un modulo di richiesta o a una regola di approvazione.
* Le regole di approvazione indirizzano le richieste in base ai valori dei campi nella richiesta inviata (ad esempio, approvatori diversi per valori diversi di un campo &quot;Tipo di campagna&quot;).
* Puoi visualizzare le informazioni di approvazione sul record creato tramite i campi Data di approvazione e Data di approvazione. Consulta Creare campi.
* Se tutti gli approvatori approvano, viene creato un record per il tipo di record associato al modulo di richiesta.
* Se almeno un approvatore rifiuta, non viene creato alcun record per il tipo di record; la richiesta rimane/arriva all’area Richieste di Workfront. (Questo punto è presente in entrambe le sezioni con una formulazione leggermente diversa, qui riunita in un&#39;unica dichiarazione).
* Quando sono necessari più approvatori, tutti devono prendere una decisione prima che la richiesta venga approvata o rifiutata, a meno che non sia abilitata l’opzione È necessaria una sola decisione.
* Se un team è impostato come approvatore, è necessaria una sola decisione da parte di un membro di quel team.
* Le approvazioni sono facoltative: se a un modulo di richiesta non è associata alcuna approvazione, Workfront Planning crea il record immediatamente dopo l&#39;invio.
* <span class="preview">È possibile aggiungere una o più fasi alle approvazioni.</span>

## Aggiungere regole di approvazione a un modulo di richiesta

Le regole di approvazione definiscono il processo di approvazione in base ai valori dei campi nelle richieste inviate.

Ad esempio, se un modulo di richiesta ha il campo &quot;Tipo di campagna&quot;, è possibile creare una regola che invia la richiesta a una persona quando il campo ha il valore &quot;Digitale&quot; e a una persona diversa quando ha il valore &quot;Stampa&quot;.

Per impostare le regole di approvazione per un modulo di richiesta:

1. Iniziare a creare un modulo di richiesta per un tipo di record, come descritto nell&#39;articolo [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. All&#39;apertura del modulo di richiesta, fare clic su **Impostazioni**.

   Viene visualizzata la scheda **Impostazioni**.

1. Per iniziare a configurare le regole di approvazione, fai clic su **Approvazioni** ![Icona Approvazioni](assets/approvals-icon-on-form.png) nel pannello a sinistra.

1. (Facoltativo) Se desideri impostare un processo di approvazione predefinito, aggiungi almeno un utente o un team al campo **Approvatori** dell&#39;area **Regola di approvazione predefinita**, quindi fai clic sulla casella di controllo **È necessaria una sola decisione** se desideri che il record venga creato dopo che uno qualsiasi degli approvatori predefiniti lo ha approvato.

   ![Area regola di approvazione predefinita](assets/default-approvers.png)

1. (Facoltativo) Inizia ad aggiungere le regole di approvazione. Per ogni regola di approvazione personalizzata, effettua le seguenti operazioni:

   1. Fai clic su **Aggiungi regola di approvazione**.
   1. Fare clic sul titolo del segnaposto **Regola di approvazione senza titolo** e immettere un nome per la regola di approvazione.
   1. Fai clic su **Seleziona un campo** e seleziona il campo che attiva la regola.
   1. Seleziona l’operatore per la regola. Gli operatori variano in base al tipo di campo.
   1. Se l’operatore selezionato richiede un valore, fai clic sull’icona più e aggiungi uno o più valori.
   1. (Facoltativo) Fai clic su **Aggiungi condizione** per aggiungere altre condizioni e connetterle tramite **And** o **Or** istruzioni configurando le condizioni aggiuntive come nei passaggi C-E.
   1. Nell&#39;area **Azioni** della regola di approvazione, nel campo **Approvatori**, aggiungere almeno un utente o un team da impostare come approvatore quando viene soddisfatta la condizione.
   1. (Condizionale e facoltativo) Se desideri che il record venga creato dopo che uno qualsiasi degli approvatori lo ha approvato, seleziona la casella di controllo **È necessaria una sola decisione**. In caso contrario, tutti gli approvatori devono decidere in merito all’approvazione prima che la richiesta venga accettata o rifiutata.

   >[!NOTE]
   >
   >   Quando aggiungi regole di approvazione, tieni presente quanto segue:
   >
   >   * Se è impostata solo una regola predefinita, questa si applica a ogni richiesta inviata.
   >   * Se viene soddisfatta una regola personalizzata, l’impostazione predefinita non viene applicata al flusso di lavoro di approvazione delle richieste. Per le approvazioni vengono applicate solo le regole personalizzate corrispondenti e la regola predefinita viene ignorata.
   >   * Se vengono soddisfatte più regole personalizzate, viene applicata la prima nell’ordine. In questo caso, l’approvazione predefinita non si applica, se presente.

1. <span class="preview">(Facoltativo) Fare clic su **Aggiungi fase** per aggiungere un&#39;altra fase all&#39;approvazione.</span>

1. Fai clic su **Salva** per salvare le regole di approvazione.

1. <span class="preview">(Facoltativo) Per aggiungere altre fasi all&#39;approvazione, eseguire le operazioni seguenti:</span>

   1. <span class="preview">Fare clic su **Aggiungi fase**.</span>

      <span class="preview">Viene visualizzata la casella **Approvazione in più fasi**. Se è già stata creata un&#39;azione di approvazione predefinita, tali approvatori vengono aggiunti automaticamente alla fase 1.</span>

   1. <span class="preview">Nel campo **Aggiungi persone o team**, aggiungi almeno un utente o team da impostare come approvatore per la fase.</span>
   1. <span class="preview">(Condizionale e facoltativo) Se si desidera che il record passi alla fase successiva dopo l&#39;approvazione di uno qualsiasi degli approvatori, selezionare la casella di controllo **È necessaria una sola decisione**. In caso contrario, tutti gli approvatori devono decidere in merito all&#39;approvazione prima che la richiesta passi alla fase successiva.</span>
   1. <span class="preview">Fare clic su **Aggiungi fase** e ripetere il passaggio B per aggiungere altre fasi all&#39;approvazione.</span>

      <span class="preview">Quando sono presenti due o più fasi, è possibile fare clic sull&#39;icona **Trascina** ![Trascina icona](assets/drag-icon.png) per trascinarle e rilasciarle in ordine.</span>

      <span class="preview">Fai clic su **Elimina questa fase** per eliminare una fase dall&#39;approvazione, oppure fai clic sull&#39;icona **Elimina** ![Elimina icona](assets/delete.png) accanto a un approvatore per eliminare l&#39;utente o il team dall&#39;elenco degli approvatori in una fase.</span>

      ![Casella di approvazione in più fasi](assets/planning-request-multi-stage-approval-box.png)

   1. <span class="preview">Al termine della creazione del flusso di lavoro di approvazione, fare clic su **Salva**.</span>

      <span class="preview">È possibile modificare o eliminare l&#39;approvazione in più fasi dalla pagina Approvazioni.</span>

1. (Facoltativo) Fai clic su **Pubblica** se non hai mai condiviso il modulo di richiesta in precedenza.



<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->