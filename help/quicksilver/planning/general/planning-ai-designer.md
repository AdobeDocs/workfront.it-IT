---
title: Guida introduttiva di Adobe Workfront Planning Designer
description: Utilizzando Adobe Planning Designer, è possibile generare una nuova area di lavoro, completa di tipi di record e campi in Workfront Planning, aggiungere oggetti a un'area di lavoro o visualizzare la cronologia delle modifiche sui record.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---


# Introduzione a Adobe Workfront Planning Designer

{{planning-important-intro}}

Utilizzando Adobe Planning Designer, è possibile generare una nuova area di lavoro, completa di tipi di record e campi in Workfront Planning, aggiungere oggetti a un&#39;area di lavoro o visualizzare la cronologia delle modifiche sui record.

>[!IMPORTANT]
>
>Il Designer di Planning è attualmente disponibile solo per gli utenti che partecipano alla fase beta chiusa.

## Requisiti di accesso <!--edit theses-->

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

<!--these are from the AI Assistant - edit these-->

* Per utilizzare il Designer di Planning, è innanzitutto necessario abilitare l&#39;Assistente IA per l&#39;organizzazione. Affinché l’Assistente IA sia disponibile per tutti gli utenti dell’organizzazione, è necessario abilitare quanto segue:

   * L’Assistente AI deve essere abilitato per la tua organizzazione prima che sia disponibile per gli utenti della tua azienda. Per informazioni, vedere [Panoramica dell&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * Dopo che Workfront ha abilitato l’Assistente AI per la tua organizzazione, questo sarà disponibile per l’amministratore Workfront principale. Per informazioni, vedere [Configurare le informazioni di base per il sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

   * L’amministratore di Workfront deve abilitare l’Assistente AI per tutti gli altri utenti. Per ulteriori informazioni, vedere [Attivare o disattivare l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

   * L’Assistente AI funziona nel contesto di ogni pagina. Le richieste inviate per l&#39;Assistente AI devono fare riferimento alla funzionalità disponibile nella pagina aperta.

* Per utilizzare Planning Designer, un amministratore di sistema deve abilitarlo nell&#39;area Preferenze di sistema della Configurazione.

* Le azioni eseguite dall&#39;Assistente IA nell&#39;area Planning si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront. Per informazioni, vedere i seguenti articoli:

   * [Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dall&#39;Assistente AI per conto dell&#39;utente vengono tracciate nel pannello della cronologia del record.

* Puoi utilizzare i comandi per annullare le azioni. Ad esempio, puoi digitare &quot;Annulla ultima modifica&quot; per ripristinare la modifica.

* Durante la creazione, l’aggiornamento o l’eliminazione di un oggetto tramite l’Assistente IA, l’Assistente AI visualizza le azioni previste e richiede una conferma. Puoi quindi confermare o annullare le azioni.

—>

## Funzionalità attualmente disponibile per Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

È possibile utilizzare Planning Designer o l&#39;Assistente IA per eseguire una delle azioni seguenti:

* Creare e configurare le aree di lavoro

* Crea tipi di record

* Progettare campi o campi formula

* Creare, eliminare, duplicare e ripristinare record

* Modificare, aggiornare e aggiungere un campo in un record

* Collega record ad altri record

* Cronologia modifiche record di accesso

* Creare viste personalizzate

* Creare record importando un documento. La creazione di record da un documento importato è disponibile solo in Planning Designer e non nell&#39;Assistente IA. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Individuare il Designer di Planning in Workfront Planning

È possibile accedere al Designer di Planning dalla pagina principale di Workfront Planning.

<!--add screen shot-->

È inoltre possibile utilizzare l&#39;Assistente AI per sfruttare le stesse funzionalità offerte dal Designer di Planning.

## Abilitare il Planing Designer per la tua organizzazione

In qualità di amministratore di Workfront, devi innanzitutto abilitare il Designer di Planning per la tua organizzazione.

<!--add steps here-->

## Creazione o aggiornamento di oggetti mediante Planning Designer

È possibile creare o aggiornare oggetti in Workfront Planning utilizzando il Designer di Planning o l&#39;Assistente IA, salvo diversa indicazione.

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Dots main menu](assets/dots-main-menu.png) nell&#39;angolo superiore destro dello schermo oppure sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile.

1. Fare clic su **Pianificazione**. Verrà visualizzata l&#39;area Pianificazione.

1. Fai clic su **Progettazione con IA**.

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

   Viene visualizzata un&#39;anteprima visiva con un esempio di ciò che l&#39;Assistente può creare.

1. Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti nella riga di comando per creare, aggiornare o rivedere l’oggetto della richiesta.




