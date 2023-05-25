---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
description: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 3849bd8ce80f40ae7d05b81e0dd8e846851dffc0
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Utilizzare i flussi di lavoro nell’integrazione di Experience Manager Assets

Un flusso di lavoro è un insieme di azioni che collegano Workfront ad Adobe Experience Manager as a Cloud Service. Un amministratore di Workfront può configurare i flussi di lavoro in Workfront, quindi assegnarli a Modelli di progetto. Quando un progetto viene creato utilizzando un modello di progetto a cui è assegnato un flusso di lavoro, vengono attivate le azioni definite nel flusso di lavoro.

>[!NOTE]
>
>I flussi di lavoro sono disponibili solo in un’integrazione Adobe Experience Manager as a Cloud Service. Non sono disponibili nelle integrazioni con Adobe Experience Manager Assets Essentials.


## Requisiti di accesso

Devi avere i seguenti:

<table>
  <tr>
   <td><strong>Piano Adobe Workfront*</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Adobe Workfront*</strong>
   </td>
   <td>Richiedi o superiore
   </td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong>
   </td>
   <td><p>Devi disporre di Experience Manager Assets as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente nell’Admin Console.</p><p>Per creare cartelle collegate, è necessario disporre dell’accesso in scrittura all’archivio in Adobe Experience Manager.</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni del livello di accesso*</strong>
   </td>
   <td>Modifica accesso ai documenti
<p>
<strong>Nota: </strong>Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <strong>Creare o modificare livelli di accesso personalizzati</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Autorizzazioni oggetto</strong>
   </td>
   <td>Gestire l’accesso o versione successiva al progetto 
<p>
Per informazioni sulla richiesta di accesso aggiuntivo, consulta <strong>Richiedi accesso agli oggetti </strong>.
   </td>
  </tr>
</table>

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare i flussi di lavoro in un’integrazione Adobe Experience Manager. Per ulteriori informazioni, consulta [Configurare l’integrazione di Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Aggiungere un flusso di lavoro a un modello

È possibile aggiungere un flusso di lavoro a un modello di progetto. Il flusso di lavoro verrà applicato a tutti i progetti creati dal modello.

1. <!-- main menu snippet??--> Aprire un modello facendo clic su **Modelli** nel menu principale, quindi selezionare il modello dall&#39;elenco.
1. Clic **Experience Manager Assets** nel pannello di navigazione a sinistra.

   >[!NOTE]
   >
   >Se la sezione Experience Manager Assets non è visibile nel menu di navigazione a sinistra, l’amministratore di Workfront non ha abilitato i flussi di lavoro per la tua organizzazione. <!--Is this right?-->

1. In **Seleziona un campo di integrazione per flussi di lavoro automatizzati**, seleziona l’integrazione con i flussi di lavoro che desideri utilizzare per i progetti creati da questo modello.
1. (Facoltativo) Modifica i valori del flusso di lavoro che desideri applicare ai progetti creati da questo modello.

   Ad esempio, per creare una cartella collegata in un percorso diverso da quello predefinito, immettere il percorso della cartella collegata.

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.

1. Le modifiche vengono salvate automaticamente. <!-- do they though??-->

## Aggiungere un flusso di lavoro a un progetto

Puoi aggiungere un flusso di lavoro durante la creazione di un progetto o un flusso di lavoro a un progetto esistente. In entrambi i casi, per aggiungere il flusso di lavoro verrà utilizzato un modello di progetto.

### Aggiungere un flusso di lavoro durante la creazione di un progetto

1. Inizia a creare un progetto.

   Per istruzioni, consulta [Creare un progetto utilizzando un modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Quando selezioni un modello per il progetto, seleziona il modello contenente i flussi di lavoro che desideri utilizzare per questo progetto.
1. (Facoltativo) Modifica i valori del flusso di lavoro per il progetto, come descritto in [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project).

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.


### Aggiungere un flusso di lavoro a un progetto esistente

1. Inizia ad aggiungere un modello al progetto.

   Per istruzioni, consulta [Allegare un modello a un progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Quando selezioni un modello per il progetto, seleziona il modello contenente i flussi di lavoro che desideri utilizzare per questo progetto.
1. (Facoltativo) Modifica i valori del flusso di lavoro per il progetto, come descritto in [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project).

### Modificare i valori del flusso di lavoro in un progetto

Puoi modificare i valori del flusso di lavoro a livello di progetto. I valori del flusso di lavoro a livello di progetto sostituiscono i valori impostati nel modello di progetto, che sostituiscono i valori predefiniti impostati nell’integrazione di Adobe Experience Manager Assets.

Tutti i valori del flusso di lavoro sono disponibili in:

* La sezione Workflow della finestra Crea progetto o Modifica progetto.
* La sezione Adobe Experience Manager del menu di navigazione a sinistra.


   >[!NOTE]
   >
   >Se queste aree non sono visibili, l’amministratore di Workfront non ha abilitato i flussi di lavoro per la tua organizzazione.

#### Cartelle collegate

Per modificare il flusso di lavoro per le cartelle collegate:

1. Attiva/disattiva **[!UICONTROL Crea cartella collegata]** su.
1. Scegli un percorso di cartella per indicare dove desideri che tutte le cartelle collegate siano associate a questa integrazione.
1. Se utilizzi la finestra Crea progetto o Modifica progetto, fai clic su Salva.

   Oppure

   Se ti trovi nell’area Adobe Experience Manager, le modifiche vengono salvate automaticamente. <!--Do they though?-->

