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
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 930
ht-degree: 3%

---

# Aggiungere un’approvazione a un modulo di richiesta in Pianificazione di Adobe Workfront

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

È possibile aggiungere un processo di approvazione a un modulo di richiesta di Adobe Workfront Planning, per avviare un&#39;approvazione per ogni richiesta sottomessa, prima di creare un record.

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
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e qualsiasi pacchetto Planning</p>
Oppure
<p>Qualsiasi pacchetto del flusso di lavoro e qualsiasi pacchetto Planning</p>

<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p> 
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

* È possibile aggiungere uno o più approvatori a un modulo di richiesta. Puoi aggiungere utenti e team come approvatori.
* È possibile visualizzare le informazioni sull&#39;approvazione in un record creato inviando un modulo di richiesta nei campi Approvato da e Data approvata. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).
* Quando si aggiungono più approvatori a un modulo di richiesta, tutti gli approvatori devono accettare la richiesta prima di creare un record in Workfront Planning.
* Se tutti gli approvatori approvano la richiesta, viene creato un record per il tipo di record associato al modulo di richiesta.
* Se almeno un approvatore rifiuta la richiesta e tutti gli altri la approvano, viene creata una richiesta per l&#39;area Richieste di Workfront, ma non viene creato alcun record per il tipo di record associato al modulo di richiesta.
* L’aggiunta di approvazioni a un modulo di richiesta è facoltativa. Workfront Planning crea immediatamente un record quando viene sottomessa una richiesta, se il modulo di richiesta non è associato a un&#39;approvazione.

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

## Aggiungere regole di approvazione a un modulo di richiesta

Le regole di approvazione definiscono il processo di approvazione in base ai valori dei campi nelle richieste inviate.

Ad esempio, se un modulo di richiesta ha il campo &quot;Tipo di campagna&quot;, è possibile creare una regola che invia la richiesta a una persona quando il campo ha il valore &quot;Digitale&quot; e a una persona diversa quando ha il valore &quot;Stampa&quot;.

Quando aggiungi regole di approvazione, tieni presente quanto segue:

* È possibile aggiungere uno o più approvatori a una regola di approvazione.
* Se almeno un approvatore rifiuta la richiesta, la richiesta viene rifiutata e il record non viene creato. La richiesta rimane nell’area Richieste di Workfront.
* Se si aggiungono più approvatori e l&#39;opzione È necessaria una sola decisione non è abilitata, tutti gli approvatori devono prendere una decisione prima che una richiesta venga approvata o rifiutata.
* Se un team è impostato come approvatore, è necessaria una sola decisione da parte di un membro del team.

Per impostare le regole di approvazione per un modulo di richiesta:

1. Iniziare a creare un modulo di richiesta per un tipo di record, come descritto nell&#39;articolo [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. All&#39;apertura del modulo di richiesta, fare clic su **Impostazioni**.

   Viene visualizzata la scheda **Impostazioni**.

1. Per iniziare a configurare le regole di approvazione, fai clic su **Approvazioni** ![Icona Approvazioni](assets/approvals-icon-on-form.png) nel pannello a sinistra.

1. (Facoltativo) Se desideri impostare un processo di approvazione predefinito, aggiungi almeno un utente o un team al campo **Approvatori** dell&#39;area **Regola di approvazione predefinita**, quindi fai clic sulla casella di controllo **È necessaria una sola decisione** se desideri che il record venga creato dopo che uno qualsiasi degli approvatori predefiniti lo ha approvato.

   ![Area regola di approvazione predefinita](assets/default-approvers.png)

1. (Facoltativo) Inizia ad aggiungere le regole di approvazione. Per ogni regola di approvazione personalizzata, effettua le seguenti operazioni:

   1. Fai clic su **Aggiungi regola di approvazione**
   1. Fare clic sul titolo del segnaposto **Regola di approvazione senza titolo** e immettere un nome per la regola di approvazione.
   1. Fai clic su **Seleziona un campo** e seleziona il campo che attiva la regola.
   1. Seleziona l’operatore per la regola. Gli operatori variano in base al tipo di campo.
   1. Se l’operatore selezionato richiede un valore, fai clic sull’icona più e aggiungi uno o più valori.
   1. (Facoltativo) Fai clic su **Aggiungi condizione** per aggiungere altre condizioni e connetterle tramite **And** o **Or** istruzioni configurando le condizioni aggiuntive come nei passaggi C-E.
   1. Nell&#39;area **Azioni** della regola di approvazione, nel campo **Approvatori**, aggiungere almeno un utente o un team da impostare presso l&#39;approvatore quando la condizione viene soddisfatta.
   1. (Condizionale e facoltativo) Se desideri che il record venga creato dopo che uno qualsiasi degli approvatori lo ha approvato, seleziona la casella di controllo **È necessaria una sola decisione**. In caso contrario, tutti gli approvatori devono decidere in merito all’approvazione prima che la richiesta venga accettata o rifiutata.

   >[!NOTE]
   >
   >   Quando aggiungi regole di approvazione, tieni presente quanto segue:
   >
   >   * Se è impostata solo una regola predefinita, questa si applica a ogni richiesta inviata.
   >   * Se viene soddisfatta una regola personalizzata, l’impostazione predefinita non viene applicata al flusso di lavoro di approvazione delle richieste. Per le approvazioni vengono applicate solo le regole personalizzate corrispondenti e la regola predefinita viene ignorata.
   >   * Se vengono soddisfatte più regole personalizzate, viene applicata la prima nell’ordine. In questo caso, l’approvazione predefinita non si applica, se presente.

1. Fai clic su **Salva** per salvare le regole di approvazione.
1. (Facoltativo) Fai clic su **Pubblica** se non hai mai condiviso il modulo di richiesta in precedenza.
