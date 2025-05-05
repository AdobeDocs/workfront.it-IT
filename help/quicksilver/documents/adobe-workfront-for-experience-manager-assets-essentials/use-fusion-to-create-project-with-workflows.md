---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilizzare Workfront Fusion per creare un progetto Workfront con flussi di lavoro Adobe Experience Manager
description: Se stai creando un progetto tramite Workfront Fusion e desideri includere nel progetto i flussi di lavoro di Adobe Experience Manager, devi utilizzare una configurazione specifica del modulo Fusion, descritta in questo articolo.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Utilizzare Workfront Fusion per convertire un problema di Workfront in un progetto che include flussi di lavoro di Adobe Experience Manager

Se stai creando un progetto tramite Workfront Fusion e desideri includere nel progetto i flussi di lavoro di Adobe Experience Manager, devi utilizzare una configurazione specifica del modulo Fusion, descritta in questo articolo.

>[!NOTE]
>
>I flussi di lavoro sono disponibili solo in un’integrazione Adobe Experience Manager as a Cloud Service. Non sono disponibili nelle integrazioni con Adobe Experience Manager Assets Essentials.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Devi avere i seguenti:

<table>
  <tr>
    <td><strong>Piano Adobe Workfront*</strong></td>
    <td>Qualsiasi</td>
  </tr>
  <tr>
   <td><strong>Licenze Adobe Workfront*</strong></td>
   <td>Richiedi o superiore</td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>È necessario disporre di Assets Essentials di Experience Manager Assets as a Cloud Service e aggiungerli al prodotto come utente nell’Admin Console.</p>
       </li>
       <li>
        <p>Devi disporre dell’accesso in scrittura all’archivio in Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <p>Nuovo:</p>
     <ul>
       <li>
         <p>Selezionare o Prime Workfront Plan: l'organizzazione deve acquistare Adobe Workfront Fusion.</p>
       </li>
       <li> 
         <p>Piano Ultimate Workfront: Workfront Fusion è incluso.</p>
       </li>
     </ul>
     <p>Oppure</p>
     <p>Corrente: la tua organizzazione deve acquistare Adobe Workfront Fusion.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni del livello di accesso*</strong>
   </td>
   <td>Modifica accesso ai documenti
     <p>
       <strong>Nota: </strong>Se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <strong>Creare o modificare livelli di accesso personalizzati</strong>.
     </p>
   </td>
  </tr>
</table>

+++

## Prerequisiti

Prima di iniziare,

* L’amministratore di Workfront deve configurare i flussi di lavoro in un’integrazione Adobe Experience Manager. Per ulteriori informazioni, vedere [Configurare l&#39;integrazione as a Cloud Service di Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Devi avere un modello di progetto configurato con un flusso di lavoro cartelle collegate all’integrazione di Adobe Experience Manager.
* Devi aver creato un’applicazione OAuth in Workfront per configurare la connessione per questo modulo.

  Per istruzioni, consulta [Creare un&#39;applicazione OAuth](#create-an-oauth-application) in questo articolo.

## Configurazione del modulo

In Workfront Fusion, se desideri creare un progetto che includa flussi di lavoro Adobe Experience Manager, devi utilizzare il modulo Workfront > Azioni varie.

1. Aggiungi il modulo **Workfront** > **Misc Action** allo scenario.
1. Nel campo **Connessione**, selezionare la connessione Workfront che si connette all&#39;account che verrà utilizzato da questo modulo.

   Per istruzioni sulla creazione di una connessione, vedere [Connetti [!DNL Workfront] a [!DNL Workfront Fusion]](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) nell&#39;articolo Moduli di Workfront.

   Per istruzioni sulla creazione dell&#39;ID client e del segreto client, è necessario creare una connessione. Vedere [Creare un&#39;applicazione OAuth](#create-an-oauth-application) in questo articolo.

1. Nel campo **Tipo di record**, selezionare `Issue`.
1. Nel campo **Azione**, selezionare `convertToProject`.
1. Nel campo **ID**, immetti o mappa l&#39;ID del problema da convertire in un progetto.
1. Abilita **Mostra impostazioni avanzate**.
1. Scorri fino alla parte inferiore del modulo e individua il campo **Progetto (raccolta avanzata)**.
1. Incolla il testo seguente nel campo **Progetto (Raccolta avanzata)**.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Sostituisci `Folder tree ID here` con gli ID cartella.

   Per individuare gli ID dell&#39;albero delle cartelle, vedere [Individuare gli ID dell&#39;albero delle cartelle](#locate-folder-tree-ids) in questo articolo.

   Per utilizzare più di una struttura di cartelle, separa gli ID con una virgola:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Sostituire `New project name here` con il nome che verrà assegnato al nuovo progetto.
1. Sostituisci `Template ID here` con l&#39;ID del modello utilizzato per il nuovo progetto.

   Puoi mappare l’ID modello da un modulo precedente (ad esempio Workfront > Modulo di ricerca) o localizzarlo nell’URL della pagina del modello in Workfront.

1. Fare clic su **OK** per salvare la configurazione del modulo.

## Individua ID struttura cartelle

Per individuare gli ID della struttura di cartelle:

>[!NOTE]
>
>Queste istruzioni utilizzano il browser Chrome.

1. In Workfront, apri il modello da utilizzare per questo progetto. Questo modello deve includere la configurazione di Adobe Experience Manager che desideri utilizzare per il progetto.
1. Apri gli strumenti per sviluppatori per il browser.
1. Apri la scheda **Rete** negli strumenti per sviluppatori.
1. Nella casella **Filtro** immettere `object-workflow`.
1. Nella colonna Nome, fai clic sull’ID alfanumerico visualizzato.

   ![Individuazione dell&#39;ID cartella 1](assets/finding-folder-id-1.png)

1. Fai clic sulla scheda **Anteprima** a destra dell&#39;ID alfanumerico.
1. Aprite le seguenti sezioni compresse:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Ogni struttura di cartelle è rappresentata da un numero. 0 (zero) rappresenta la prima cartella dell&#39;elenco, 1 rappresenta la seconda e così via. Se il modello include una sola struttura di cartelle, il numero è 0.

1. Apri la struttura di cartelle da utilizzare per il nuovo progetto. Prendere nota del valore del campo `_id`. Se si desidera utilizzare più di una struttura di cartelle, prendere nota di tutti i valori di campo `_id` per le strutture di cartelle che si desidera utilizzare.

   ![Individuazione dell&#39;ID cartella 2](assets/finding-folder-id-2.png)

   Si tratta dei valori `aemNativeFolderTreeIDs` che verranno immessi nel campo **Project (Advanced Collection)** del modulo Fusion **Workfront** > **Misc Actions**.

## Creare un’applicazione OAuth

Devi impostare un’applicazione OAuth in Workfront per la connessione di questo modulo. È necessario eseguire questa operazione una sola volta per una determinata connessione Workfront in Fusion.

1. In Workfront, iniziare a creare un&#39;applicazione OAuth, come descritto in [Creare un&#39;applicazione OAuth2 utilizzando le credenziali utente (flusso del codice di autorizzazione)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) nell&#39;articolo Creare applicazioni OAuth2 per le integrazioni [!DNL Workfront].
1. Copia l’ID client e il segreto client in una posizione sicura.
1. Nel campo **URI di reindirizzamento** immettere quanto segue:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Fai clic su **Salva**.

Utilizzerai questo ID client e segreto client durante la configurazione della connessione del modulo in Fusion.

Per istruzioni sulla creazione di una connessione, vedere [Connetti [!DNL Workfront] a [!DNL Workfront Fusion]](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) nell&#39;articolo Moduli di Workfront.
