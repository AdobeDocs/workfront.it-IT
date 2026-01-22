---
title: Guida introduttiva di Adobe Workfront Planning Designer
description: Utilizzando Adobe Planning Designer, è possibile generare una nuova area di lavoro, completa di tipi di record e campi in Workfront Planning, aggiungere oggetti a un'area di lavoro o visualizzare la cronologia delle modifiche sui record.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Introduzione a Adobe Workfront Planning Designer

{{planning-important-intro}}

È possibile utilizzare Adobe Planning Designer basato su IA per generare una nuova area di lavoro, aggiungere oggetti a un&#39;area di lavoro (tipi di record, record, visualizzazioni o campi) o visualizzare la cronologia delle modifiche sui record.

>[!IMPORTANT]
>
>Planning Designer è attualmente disponibile solo per gli utenti che partecipano al programma Beta chiuso.

Per informazioni su Workfront Planning, vedere gli articoli seguenti:

* [Informazioni generali su Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Introduzione a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Panoramica sull’accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


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
<p>Qualsiasi pacchetto Workfront e Planning</p>
<p>Qualsiasi pacchetto di Workflow e Planning</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Iscrizione al programma Beta chiuso per il Designer di pianificazione

<!--edit this Or create a new article under Beta programs?? -->

Attualmente, è possibile richiedere di partecipare al programma Beta chiuso per Planning Designer.

## Considerazioni sul Designer di Planning

* Per utilizzare Planning Designer, l&#39;organizzazione deve soddisfare i requisiti per utilizzare Workfront AI Assistant.

  Per informazioni dettagliate, vedere [Prerequisiti per l&#39;Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* Per utilizzare Planning Designer, un amministratore di sistema deve abilitarlo nell&#39;area Preferenze di sistema della Configurazione.

* È possibile utilizzare i prompt per creare oggetti di Planning utilizzando l&#39;Assistente di Workfront AI dall&#39;area Planning oppure utilizzando il Designer di Planning.

* Le azioni eseguite dall&#39;Assistente IA nell&#39;area Pianificazione o quelle eseguite dal Designer di pianificazione si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront.

  Per informazioni, vedere i seguenti articoli:

   * [Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dal Designer di Planning per conto dell&#39;utente vengono registrate nel pannello della cronologia del record.

* Puoi utilizzare i comandi per annullare le azioni. Ad esempio, puoi digitare &quot;Annulla ultima modifica&quot; per ripristinare la modifica.

* Durante la creazione, l&#39;aggiornamento o l&#39;eliminazione di un oggetto tramite il Designer di Planning, vengono visualizzate le azioni desiderate e viene richiesta una conferma. Puoi quindi confermare o annullare le azioni.

* Quando si creano aree di lavoro e tipi di record mediante Planning Designer, vengono creati automaticamente anche le viste e i campi.

## Funzionalità attualmente disponibile per Planning Designer

È possibile utilizzare Planning Designer o l&#39;Assistente IA per eseguire una delle azioni seguenti:

* Creare e configurare le aree di lavoro

* Crea tipi di record

* Progettare campi o campi formula

* Creare, eliminare, duplicare e ripristinare record

* Modificare, aggiornare e aggiungere un campo in un record

* Collega record ad altri record

* Cronologia modifiche record di accesso

* Creare viste personalizzate

* Creare record importando un documento.

  La creazione di record da un documento importato è disponibile solo in Planning Designer e non nell&#39;Assistente IA.

  Per informazioni sui tipi e sulle dimensioni di file accettati, vedere la sezione &quot;Guardrail del documento&quot; nell&#39;articolo [Utilizzare il riempimento del modulo basato su IA per compilare una richiesta utilizzando prompt o documenti](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Abilitare il Planing Designer per la tua organizzazione

In qualità di amministratore di Workfront, devi innanzitutto abilitare il Designer di Planning per la tua organizzazione.

<!--add steps here-->

1. Accedi a Workfront come amministratore di sistema.
1. Fai clic su **Menu principale** ![Icona menu principale](assets/main-menu-shell.png) nell&#39;angolo superiore sinistro dello schermo, quindi fai clic su **Configurazione**.
1. Fai clic su **Sistema** > nel pannello a sinistra, quindi vai all&#39;area **Preferenze AI**.
1. Attiva le seguenti impostazioni:
   * **Abilita IA**
   * **Consenso a beta AI**
   * **Pianificazione di Designer**

   ![Impostazione di Planning Designer nelle preferenze di sistema](assets/planning-designer-toggle-in-system-preferences.png)
1. Fai clic su **Salva**.

   Tutti gli utenti del sistema che dispongono di una licenza Standard possono ora visualizzare il pulsante **Progettazione con IA** nella pagina principale delle aree di lavoro nell&#39;area Planning. <!--check screen shot-->

   ![Pulsante Progettazione con IA nella pagina Workspace](assets/design-with-ai-button-on-workspaces-page.png)

   Tutti gli utenti possono ora avviare e utilizzare il Designer di Planning per creare e aggiornare oggetti di Workfront Planning.

## Creazione o aggiornamento di oggetti mediante Planning Designer

È possibile creare o aggiornare oggetti in Workfront Planning utilizzando il Designer di Planning o l&#39;Assistente IA, salvo diversa indicazione.

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) nell&#39;angolo in alto a sinistra.

1. Fare clic su **Pianificazione**. Verrà visualizzata l&#39;area Pianificazione.

1. Fai clic su **Progettazione con IA**.

   Viene visualizzata la finestra **Planning Designer**.

   ![Finestra di Planning Designer](assets/planning-designer-window.png)

1. Nello spazio disponibile, inizia a digitare i comandi per l’Assistente AI, quindi al termine fai clic su Invio.

   <!--add screen shot-->

   Ad esempio, puoi digitare una richiesta simile a quelle seguenti:

   * Creare e configurare un’area di lavoro con cinque tipi di record per gestire le campagne

   * Crea campagne di marketing per ogni mese dell’anno corrente

   * Aggiungere un campo campagna per lo stato dell&#39;area di lavoro Progettazione marketing

   * Elimina tutti i record con lo stato Non aggiornato

   * Aggiorna tutte le campagne Planning con lo stato Attivo

   * Collegare le campagne a utenti tipo nell’area di lavoro Progettazione marketing

   * Visualizza la cronologia modifiche per la campagna &quot;San Valentino&quot;

   * Creare una visualizzazione timeline per le campagne nell’area di lavoro Progettazione marketing

   * Creare record importando un documento. La creazione di record da un documento importato è disponibile solo in Planning Designer e non nell&#39;Assistente IA.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti nell’area dei prompt per creare, aggiornare o rivedere l’oggetto della richiesta.

   Quando si accetta di creare gli oggetti, le modifiche vengono visualizzate a destra dell&#39;area del prompt.

   È possibile esaminare aree di lavoro, tipi di record, campi, visualizzazioni e record nell&#39;area di anteprima a destra del prompt.
1. (Facoltativo) Immettete ulteriori richieste per modificare ulteriormente gli oggetti.
1. (Facoltativo) Fai clic sull&#39;icona **Nascondi o mostra l&#39;icona della schermata di anteprima dell&#39;area di lavoro AI** per aprire o chiudere la schermata di anteprima a destra.![](assets/hide-show-preview-screen-in-planning-designer.png)
1. Fai clic sull&#39;icona **Apri area di lavoro in una nuova scheda** ![Apri area di lavoro in una nuova scheda](assets/open-workspace-on-new-tab-icon.png) per aprire l&#39;area di lavoro che stai aggiornando in una nuova scheda.
1. Fare clic sull&#39;icona **Chiudi** **X** per chiudere Planning Designer e aprire l&#39;area Aree di lavoro.
1. Aprire l&#39;area di lavoro modificata mediante Planning Designer e apportare ulteriori modifiche ai relativi oggetti.




