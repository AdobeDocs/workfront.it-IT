---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
description: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 0%

---

# Utilizzare i flussi di lavoro nell’integrazione di Experience Manager Assets

Un flusso di lavoro è un insieme di azioni che collegano Workfront ad Adobe Experience Manager as a Cloud Service. Un amministratore di Workfront può configurare i flussi di lavoro in Workfront, quindi assegnarli a Modelli di progetto.

Quando un progetto viene creato utilizzando un modello di progetto a cui è assegnato un flusso di lavoro, vengono attivate le azioni definite nel flusso di lavoro.

>[!NOTE]
>
>I flussi di lavoro sono disponibili solo in un’integrazione Adobe Experience Manager as a Cloud Service. Non sono disponibili nelle integrazioni con Adobe Experience Manager Assets Essentials.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p> </td> 
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
   <td> <p>Modifica accesso ai documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Aggiungere un flusso di lavoro a un progetto

Puoi aggiungere un flusso di lavoro durante la creazione di un progetto o un flusso di lavoro a un progetto esistente. In entrambi i casi, per aggiungere il flusso di lavoro verrà utilizzato un modello di progetto.

### Aggiungere un flusso di lavoro durante la creazione di un progetto

1. Inizia a creare un progetto.

   Per istruzioni, vedere [Creare un progetto utilizzando un modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Quando selezioni un modello per il progetto, seleziona il modello contenente i flussi di lavoro che desideri utilizzare per questo progetto.
1. (Facoltativo) Modificare i valori del flusso di lavoro per il progetto, come descritto in [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project).

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.


### Aggiungere un flusso di lavoro a un progetto esistente

>[!NOTE]
>
>I flussi di lavoro eseguiti al momento della creazione di un progetto (ad esempio la creazione di una cartella collegata) non vengono eseguiti quando il modello viene allegato a un progetto esistente. Vengono eseguiti solo quando un progetto viene creato da un modello.

1. Inizia ad aggiungere un modello al progetto.

   Per istruzioni, vedere [Allegare un modello a un progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Quando selezioni un modello per il progetto, seleziona il modello contenente i flussi di lavoro che desideri utilizzare per questo progetto.
1. (Facoltativo) Modificare i valori del flusso di lavoro per il progetto, come descritto in [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project).

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.



### Modificare i valori del flusso di lavoro in un progetto

Puoi modificare i valori del flusso di lavoro a livello di progetto. I valori del flusso di lavoro a livello di progetto sostituiscono i valori impostati nel modello di progetto, che sostituiscono i valori predefiniti impostati nell’integrazione Adobe Experience Manager Assets.

Tutti i valori del flusso di lavoro sono disponibili in:

* La sezione Flussi di lavoro o cartelle collegate della finestra Crea progetto o Modifica progetto.
* La sezione Adobe Experience Manager del menu di navigazione a sinistra.


  >[!NOTE]
  >
  >Se queste aree non sono visibili, l’amministratore di Workfront non ha abilitato i flussi di lavoro per la tua organizzazione.



#### Cartelle collegate

>[!NOTE]
>
>Poiché le cartelle collegate vengono create al momento della creazione del progetto, la modifica del flusso di lavoro delle cartelle collegate in un progetto esistente non è efficace. La modifica di questi valori durante la creazione di un progetto funziona come previsto.

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
