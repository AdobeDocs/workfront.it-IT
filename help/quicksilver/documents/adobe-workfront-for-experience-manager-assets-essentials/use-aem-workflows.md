---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
description: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 7%

---

# Utilizzare i flussi di lavoro nell’integrazione di Experience Manager Assets

Un flusso di lavoro è un insieme di azioni che collegano Workfront ad Adobe Experience Manager as a Cloud Service. Un amministratore di Workfront può configurare i flussi di lavoro in Workfront, quindi assegnarli a Modelli di progetto.

Quando un progetto viene creato utilizzando un modello di progetto a cui è assegnato un flusso di lavoro, vengono attivate le azioni definite nel flusso di lavoro.

>[!NOTE]
>
>I flussi di lavoro sono disponibili solo in un’integrazione Adobe Experience Manager as a Cloud Service. Non sono disponibili nelle integrazioni con Adobe Experience Manager Assets Essentials.<br>
>Questa funzionalità non è disponibile nell&#39;area nuovi documenti.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>Devi disporre di Experience Manager as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente in Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorizzazioni Experience Manager</td> 
    <td>È necessario disporre dell'accesso in scrittura alla cartella.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare i flussi di lavoro in un’integrazione Adobe Experience Manager. Per ulteriori informazioni, vedere [Configurare l&#39;integrazione Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Aggiungere un flusso di lavoro a un modello

È possibile aggiungere un flusso di lavoro a un modello di progetto. Il flusso di lavoro verrà applicato a tutti i progetti creati dal modello.

1. Aprire un modello facendo clic su **Modelli** nel menu principale, quindi selezionare il modello dall&#39;elenco.
1. Fai clic su **Experience Manager Assets** nel pannello di navigazione a sinistra.

   >[!NOTE]
   >
   >Se la sezione Experience Manager Assets non è visibile nel menu di navigazione a sinistra, l’amministratore di Workfront non ha abilitato i flussi di lavoro per la tua organizzazione. <!--Is this right?-->

1. Nel campo **Selezionare un&#39;integrazione per flussi di lavoro automatizzati**, selezionare l&#39;integrazione con i flussi di lavoro che si desidera utilizzare per i progetti creati da questo modello.
1. (Facoltativo) Modifica i valori del flusso di lavoro che desideri applicare ai progetti creati da questo modello.

   Per istruzioni su flussi di lavoro specifici, vedere [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project) in questo articolo.

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.

1. Le modifiche vengono salvate automaticamente. <!-- do they though??-->

## Add a workflow to a project

You can add a workflow when creating a project, or add a workflow to an existing project. In both cases, you will use a project template to add the workflow.

### Add a workflow when creating a project

1. Begin creating a project.

   For instructions, see [Create a project using a template](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in [Edit workflow values in a project](#edit-workflow-values-in-a-project).

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.


### Add a workflow to an existing project

>[!NOTE]
>
>Workflows that run when a project is created (such as linked folder creation) do not run when the template is attached to an existing project. They only run when a project is created from a template.

1. Begin adding a template to the project.

   For instructions, see [Attach a template to a project](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in [Edit workflow values in a project](#edit-workflow-values-in-a-project).

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.



### Edit workflow values in a project

You can edit workflow values on the project level. Project-level workflow values override values set on the project template, which override the default values set in the Adobe Experience Manager Assets integration.

All workflow values can be found in:

* The Workflows or Linked folders section of the Create project or Edit project window.
* The Adobe Experience Manager section of the left navigation.


  >[!NOTE]
  >
  >If these areas are not visible, your Workfront administrator has not enabled Workflows for your organization.



#### Cartelle collegate

>[!NOTE]
>
>Because linked folders are created when the project is created, editing the linked folder workflow on an existing project is ineffective. La modifica di questi valori durante la creazione di un progetto funziona come previsto.

Per modificare il flusso di lavoro per le cartelle collegate:

1. Attiva o disattiva **[!UICONTROL Crea cartella collegata]** come desiderato. Se si attiva questa funzione, è possibile modificare la configurazione della cartella collegata.

   Per informazioni dettagliate sulla configurazione della cartella collegata, vedere [Creare cartelle collegate a Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) nell&#39;articolo [Configurare l&#39;integrazione di [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Facoltativo) Se si desidera che la struttura di cartelle venga creata solo se determinati valori sono presenti in un modulo personalizzato allegato al progetto, fare clic sul **Applica filtro** per la struttura di cartelle, quindi selezionare il modulo personalizzato contenente il campo, il campo e il valore del campo. Se il campo del modulo personalizzato allegato al nuovo progetto contiene il valore scelto, verrà creata la struttura ad albero delle cartelle.
1. (Facoltativo) Quando configuri i nomi delle cartelle, puoi scegliere tra le seguenti opzioni:

   * **Nome**: immettere un nome per la cartella.

   * **Dati oggetto**: selezionare l&#39;origine per il nome della cartella, ad esempio Nome progetto.

   * **Dati modulo personalizzato**: selezionare i dati del modulo personalizzato da utilizzare come nome della cartella.

     L’utilizzo dei dati del modulo personalizzato per i nomi delle cartelle è disponibile solo a livello di modello e non può essere configurato a livello di integrazione.

     Se il nome di una cartella è impostato su dati personalizzati che non esistono nella cartella personalizzata associata al progetto, come nome della cartella verrà assegnato un ID casuale.

1. Per visualizzare la struttura delle cartelle, fare clic sull&#39;icona **Anteprima** ![Anteprima](assets/preview-icon.png)
1. Fai clic su **[!UICONTROL Salva]**.

#### Pubblicazione delle risorse

Per modificare il flusso di lavoro per la pubblicazione delle risorse:

1. Attiva o disattiva **Pubblica automaticamente risorse** come desiderato.
1. (Condizionale) Se abiliti la pubblicazione, seleziona se desideri pubblicarla nel servizio di pubblicazione, nel portale del brand o in entrambi.
1. Fai clic su **[!UICONTROL Salva]**.
