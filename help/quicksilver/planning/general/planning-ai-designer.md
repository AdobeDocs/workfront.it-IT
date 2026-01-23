---
title: Guida introduttiva di Adobe Workfront Planning Designer
description: Utilizzando Adobe Planning Designer, è possibile generare una nuova area di lavoro, completa di tipi di record e campi in Workfront Planning, aggiungere oggetti a un'area di lavoro o visualizzare la cronologia delle modifiche sui record.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bd3dde54d986416af847b2f3b2a1e8570d5ce3f2
workflow-type: tm+mt
source-wordcount: '1278'
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


## Requisiti di accesso <!--edit theses??-->

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

Al momento, potete richiedere di partecipare al programma Beta chiuso per il Designer di pianificazione inviandoci un&#39;e-mail all&#39;indirizzo sargism@adobe.com.

Dopo aver ricevuto l&#39;e-mail, il nostro team tecnico attiverà il Designer di pianificazione nella tua istanza Workfront.

>[!IMPORTANT]
>
>Prima che Planning Designer sia disponibile nel sistema, è necessario che la società accetti il contratto di AI Assistant.

## Considerazioni sul Designer di Planning

* Per utilizzare il Designer di Planning, è innanzitutto necessario attivare l&#39;Assistente IA per l&#39;organizzazione. Affinché l’Assistente IA sia disponibile per tutti gli utenti dell’organizzazione, è necessario che siano presenti i seguenti elementi:

   * Workfront deve rendere l’Assistente AI disponibile per la tua organizzazione.

     Per informazioni dettagliate, vedere [Prerequisiti per l&#39;Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
   * Dopo che Workfront ha reso l’Assistente AI disponibile per la tua organizzazione, l’amministratore principale di Workfront può accedervi.

     Per informazioni, vedere [Configurare le informazioni di base per il sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).
   * L’amministratore di Workfront deve accettare il contratto di AI Assistant e quindi attivare l’AI Assistant per tutti gli altri utenti.

     Per ulteriori informazioni, vedere [Attivare o disattivare l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).
* Dopo che l&#39;amministratore di sistema ha attivato l&#39;Assistente IA per la propria organizzazione, l&#39;Assistente di Planning è disponibile per tutti gli utenti per impostazione predefinita, se è stato reso disponibile per la propria organizzazione.
* Le azioni eseguite dal Designer di Planning possono essere eseguite anche dall&#39;Assistente IA, quando lo si utilizza nell&#39;area Pianificazione.
* Le azioni eseguite dall&#39;Assistente IA nell&#39;area Pianificazione o quelle eseguite dal Designer di pianificazione si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront.

  Per informazioni, vedere i seguenti articoli:

   * [Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dall&#39;Assistente AI o dal Designer di Planning per conto dell&#39;utente vengono registrate nel pannello della cronologia del record.

* Le azioni eseguite dal Designer di pianificazione sono permanenti e potrebbero essere irreversibili. L’eliminazione di un campo, ad esempio, non può essere annullata. Rivedi tutte le azioni proposte da Designer prima di accettarle.

  >[!IMPORTANT]
  >
  >Durante la creazione, l&#39;aggiornamento o l&#39;eliminazione di un oggetto tramite il Designer di Planning, il prompt richiede una conferma solo per le azioni irreversibili. Ad esempio, l’eliminazione di un tipo di record o di un’area di lavoro è irreversibile. L&#39;eliminazione di un record non è. Il Designer di Planning richiederà conferma solo quando si tenta di eliminare un tipo di record o un&#39;area di lavoro.

* Quando si creano aree di lavoro e tipi di record mediante Planning Designer, vengono creati automaticamente anche le viste e i campi.

## Funzionalità attualmente disponibile per Planning Designer

È possibile utilizzare Planning Designer o l&#39;Assistente IA per eseguire una delle azioni seguenti:

* Creare e configurare le aree di lavoro

* Creare tipi di record, inclusa la definizione e l&#39;aggiunta di tipi di record globali alle aree di lavoro

* Progettare campi o campi formula

* Creare, eliminare, duplicare e ripristinare record

* Modificare, aggiornare e aggiungere un campo in un record

* Collega record ad altri record

* Cronologia modifiche record di accesso

* Creare viste personalizzate

* Creare record importando un documento

  È ad esempio possibile caricare un&#39;immagine di un organigramma della società e il Designer di Planning può creare un&#39;area di lavoro basata su tale immagine.

  La creazione di oggetti da un documento importato è disponibile solo in Planning Designer e non nell&#39;Assistente IA.

  >[!IMPORTANT]
  >
  >Sebbene supportino i tipi di file XLSX e CSV, non possono essere utilizzati per l&#39;importazione di record su larga scala tramite Planning Designer.
  >Se in questo momento è necessario importare un numero considerevole di record, è consigliabile utilizzare le funzionalità manuali disponibili in Planning.
  >
  >Per ulteriori informazioni, vedere [Creare record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Per informazioni sulle limitazioni relative al tipo di file, vedere la sezione &quot;Ottieni suggerimenti in base a un documento caricato&quot; in [Utilizzare il riempimento modulo basato su IA per compilare una richiesta utilizzando prompt o documenti](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Creazione o aggiornamento di oggetti mediante Planning Designer

È possibile creare o aggiornare oggetti in Workfront Planning utilizzando il Designer di Planning o l&#39;Assistente IA, salvo diversa indicazione.

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) in alto a sinistra, quindi fai clic su **Planning**.

   Verrà aperta l&#39;area **Planning**.

   ![Pulsante Progettazione con IA nella pagina Aree di lavoro](assets/design-with-ai-button-on-workspaces-page.png)

1. Fai clic su **Progettazione con IA**.

   Viene visualizzata la finestra **Planning Designer**.

   ![Finestra di Planning Designer](assets/planning-designer-window.png)

1. Nello spazio disponibile, inizia a digitare i prompt per l’Assistente AI, quindi al termine fai clic su Invio.

   <!--add screen shot-->

   È ad esempio possibile digitare prompt simili a quelli riportati di seguito:

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

   È possibile visualizzare aree di lavoro, tipi di record, campi, visualizzazioni e record nell&#39;area di anteprima a destra del prompt.

   >[!TIP]
   >
   >Alcuni oggetti vengono creati immediatamente, senza necessità di conferma.

1. (Facoltativo) Immettete ulteriori richieste per modificare ulteriormente gli oggetti.
1. (Facoltativo) Fai clic sull&#39;icona **Mostra o nascondi la schermata di anteprima** ![Nascondi o mostra l&#39;icona della schermata di anteprima](assets/hide-show-preview-screen-in-planning-designer.png) per aprire o chiudere la schermata di anteprima a destra.
1. Fai clic sull&#39;icona **Apri area di lavoro in una nuova scheda** ![Apri area di lavoro in una nuova scheda](assets/open-workspace-on-new-tab-icon.png) per aprire l&#39;area di lavoro che stai aggiornando in una nuova scheda.
1. Fare clic sull&#39;icona **Chiudi** **X** per chiudere Planning Designer e aprire l&#39;area Aree di lavoro.
1. Aprire l&#39;area di lavoro modificata mediante Planning Designer e apportare ulteriori modifiche ai relativi oggetti.

## Disattiva il Designer di pianificazione per la tua organizzazione

Dopo che l&#39;amministratore di Workfront accetta il contratto di Assistente AI, il Designer di Planning viene attivato per tutti gli utenti dell&#39;organizzazione, per impostazione predefinita.

Per spegnerlo:

1. Accedere a Workfront come amministratore di sistema.
1. Fai clic su **Menu principale** ![Icona menu principale](assets/main-menu-shell.png) nell&#39;angolo superiore sinistro dello schermo, quindi fai clic su **Configurazione**.
1. Fai clic su **Sistema** > nel pannello a sinistra, quindi vai all&#39;area **Preferenze AI**.
1. Disattivare l&#39;impostazione **Planning Designer**. <!--add new screen shot with info icon-->

   ![Impostazione di Planning Designer nelle preferenze di sistema](assets/planning-designer-toggle-in-system-preferences.png)
1. Fai clic su **Salva**.

   Questo rimuove Planning Designer per tutti gli utenti del sistema.






