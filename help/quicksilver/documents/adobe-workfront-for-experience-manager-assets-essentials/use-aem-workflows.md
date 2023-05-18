---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
description: Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Utilizzare i flussi di lavoro nell’integrazione Experience Manager Assets

<span class="preview">Le informazioni in questa pagina si riferiscono a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Sandbox di anteprima.</span>

Un flusso di lavoro è un insieme di azioni che collegano Workfront ad Adobe Experience Manager as a Cloud Service. Un amministratore Workfront può configurare i flussi di lavoro in Workfront, quindi assegnarli ai modelli di progetto. Quando un progetto viene creato utilizzando un modello di progetto a cui è assegnato un flusso di lavoro, vengono attivate le azioni definite nel flusso di lavoro.

>[!NOTE]
>
>I flussi di lavoro sono disponibili solo in un’integrazione Adobe Experience Manager as a Cloud Service. Non sono disponibili nelle integrazioni con Adobe Experience Manager Assets Essentials.


## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table>
  <tr>
   <td><strong>piano Adobe Workfront*</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Adobe Workfront*</strong>
   </td>
   <td>Richiesta o superiore
   </td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong>
   </td>
   <td><p>Devi disporre di Experience Manager Assets as a Cloud Service o Assets Essentials e devi essere aggiunto al prodotto come utente nell’Admin Console.</p><p>Per creare cartelle collegate è necessario disporre dell’accesso in scrittura all’archivio in Adobe Experience Manager.</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni a livello di accesso*</strong>
   </td>
   <td>Modifica accesso ai documenti
<p>
<strong>Nota: </strong>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <strong>Creare o modificare livelli di accesso personalizzati</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Autorizzazioni oggetto</strong>
   </td>
   <td>Gestire l’accesso o una versione successiva al progetto 
<p>
Per informazioni sulla richiesta di accesso aggiuntivo, vedi <strong>Richiedere l’accesso agli oggetti </strong>.
   </td>
  </tr>
</table>

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare i flussi di lavoro in un’integrazione Adobe Experience Manager. Per ulteriori informazioni, consulta [Configurare l’integrazione as a Cloud Service di Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Aggiungere un flusso di lavoro a un modello

Puoi aggiungere un flusso di lavoro a un modello di progetto. Il flusso di lavoro verrà applicato a tutti i progetti creati dal modello.

1. <!-- main menu snippet??--> Apri un modello facendo clic su **Modelli** nel menu principale, quindi selezionare il modello dall’elenco.
1. Fai clic su **Experience Manager Assets** nel pannello di navigazione a sinistra.

   >[!NOTE]
   >
   >Se la sezione Experience Manager Assets non è visibile nel menu di navigazione a sinistra, l’amministratore Workfront non ha abilitato i flussi di lavoro per la tua organizzazione. <!--Is this right?-->

1. In **Selezionare un campo di integrazione per i flussi di lavoro automatizzati**, seleziona l’integrazione con i flussi di lavoro che desideri utilizzare per i progetti creati a partire da questo modello.
1. (Facoltativo) Modifica i valori del flusso di lavoro che desideri applicare ai progetti creati a partire da questo modello.

   Ad esempio, per creare una cartella collegata in un percorso diverso dal valore predefinito, immettere il percorso della cartella collegata.

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.

1. Le modifiche vengono salvate automaticamente. <!-- do they though??-->

## Aggiungere un flusso di lavoro a un progetto

Puoi aggiungere un flusso di lavoro durante la creazione di un progetto o un flusso di lavoro a un progetto esistente. In entrambi i casi, puoi utilizzare un modello di progetto per aggiungere il flusso di lavoro.

### Aggiungere un flusso di lavoro durante la creazione di un progetto

1. Inizia a creare un progetto.

   Per istruzioni, consulta [Creare un progetto utilizzando un modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Quando selezioni un modello per il progetto, seleziona il modello che contiene i flussi di lavoro che desideri utilizzare per questo progetto.
1. (Facoltativo) Modifica eventuali valori del flusso di lavoro per il progetto, come descritto in [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project).

   Solo i flussi di lavoro attivati nell’area Experience Manager di Configurazione sono disponibili nei modelli o nei progetti.


### Aggiungere un flusso di lavoro a un progetto esistente

1. Inizia ad aggiungere un modello al progetto.

   Per istruzioni, consulta [Allegare un modello a un progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Quando selezioni un modello per il progetto, seleziona il modello che contiene i flussi di lavoro che desideri utilizzare per questo progetto.
1. (Facoltativo) Modifica eventuali valori del flusso di lavoro per il progetto, come descritto in [Modificare i valori del flusso di lavoro in un progetto](#edit-workflow-values-in-a-project).

### Modificare i valori del flusso di lavoro in un progetto

Puoi modificare i valori del flusso di lavoro a livello di progetto. I valori del flusso di lavoro a livello di progetto sovrascrivono i valori impostati nel modello di progetto, che sovrascrivono i valori predefiniti impostati nell’integrazione di Adobe Experience Manager Assets.

Tutti i valori del flusso di lavoro si trovano in:

* La sezione Flussi di lavoro della finestra Crea progetto o Modifica progetto.
* La sezione Adobe Experience Manager della navigazione a sinistra.


   >[!NOTE]
   >
   >Se queste aree non sono visibili, l’amministratore Workfront non ha abilitato Flussi di lavoro per la tua organizzazione.

#### Cartelle collegate

Per modificare il flusso di lavoro per le cartelle collegate:

1. Attiva/disattiva la **[!UICONTROL Crea cartella collegata]** su.
1. Scegli un percorso di cartella per indicare la posizione in cui dovranno essere associate tutte le cartelle collegate a questa integrazione.
1. Fare clic su Salva se si utilizza la finestra Crea progetto o Modifica progetto.

   Oppure

   Se ti trovi nell’area Adobe Experience Manager, le modifiche vengono salvate automaticamente. <!--Do they though?-->

