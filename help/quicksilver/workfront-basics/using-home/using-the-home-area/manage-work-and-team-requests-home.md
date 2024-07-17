---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Gestire le richieste di lavoro e team nell’area Home
description: Quando le attività e i problemi di lavoro vengono assegnati all'utente, sono elencati in [!UICONTROL Elenco lavori] nell'area [!UICONTROL Home]. Puoi visualizzare, riassegnare, rispondere, lavorare su una richiesta o rimuoverla. Le richieste di lavoro nell'area [!UICONTROL Home] non sono limitate ai problemi associati alle code di richieste.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Gestisci le richieste di lavoro e team nell&#39;area [!UICONTROL Home]

Quando le attività e i problemi di lavoro vengono assegnati all&#39;utente, sono elencati in [!UICONTROL Elenco lavori] nell&#39;area [!UICONTROL Home]. Puoi visualizzare, riassegnare, rispondere, lavorare su una richiesta o rimuoverla. Le richieste di lavoro nell&#39;area [!UICONTROL Home] non sono limitate ai problemi associati alle code di richieste.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Accesso a [!UICONTROL Edit] per attività e problemi</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni Contribute o superiori per le attività e i problemi su cui devi lavorare</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Visualizzare una richiesta di lavoro

Le richieste di lavoro assegnate all&#39;utente vengono visualizzate nel pannello a sinistra in [!UICONTROL Home]. Puoi configurare le richieste da visualizzare nella [!UICONTROL Home] utilizzando il filtro nella parte superiore del [!UICONTROL Elenco lavori].

Puoi selezionare filtri che visualizzano elementi pronti per l’uso oppure elementi su cui stai già lavorando.

In questo articolo viene descritto come utilizzare i filtri nell&#39;area [!UICONTROL Home] per visualizzare gli elementi su cui si sta lavorando o che si potrebbe considerare di iniziare a lavorare. Per informazioni su tutti i filtri nell&#39;area [!UICONTROL Home], vedere [Visualizzare gli elementi nell&#39;elenco di lavoro nell&#39;area [!UICONTROL Home]](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Fai clic sul menu a discesa **[!UICONTROL Filtro]**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Fare clic su una o entrambe le opzioni seguenti per le attività:

   **[!UICONTROL Pronto per l&#39;avvio]:** Visualizza solo le attività e i problemi pronti per l&#39;avvio. Entrambe le istruzioni seguenti devono essere vere:

   * Le attività e i relativi genitori non hanno predecessori o vincoli di attività che impediscono di lavorarci.
   * La [!UICONTROL data di inizio pianificata] delle attività o dei problemi è nel passato o fino a due settimane nel futuro.

   **[!UICONTROL Non pronto]**: visualizza solo le attività e i problemi non ancora pronti per l&#39;avvio. Una delle seguenti affermazioni deve essere vera:

   * Le attività e i relativi genitori potrebbero avere predecessori o vincoli di attività che impediscono di lavorarci.
   * Le attività o i problemi hanno una [!UICONTROL Data inizio pianificata] che è superiore alle due settimane future.


1. Fai clic su **[!UICONTROL Lavori in corso]** in [!UICONTROL Attività] o [!UICONTROL Problemi] per visualizzare le attività e i problemi su cui stai lavorando.
1. Fai clic su **[!UICONTROL Richiesto]** in [!UICONTROL Problemi] per visualizzare i problemi che ti sono stati richiesti (a cui sei assegnato), ma per il momento non hai accettato di lavorare.

## Accedere a una richiesta team

Puoi accedere a una richiesta assegnata al tuo team direttamente dalla [!UICONTROL Home]. Per ulteriori informazioni sulle richieste del team, vedere [Panoramica delle richieste del team](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Nell&#39;area **[!UICONTROL Elenco lavori]**, fare clic per espandere il raggruppamento **[!UICONTROL Richieste team]**.

   Se al team non è stata assegnata alcuna richiesta, il raggruppamento non viene visualizzato.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Fare clic sul nome del team.\
   La sezione **[!UICONTROL Richieste team]** visualizza e mostra tutte le richieste assegnate al team. Per ulteriori informazioni sull&#39;utilizzo delle richieste del team, vedere [Gestire le richieste del team e del lavoro](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Riassegnare una richiesta

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Nell&#39;area **[!UICONTROL Elenco lavori]** selezionare la richiesta che si desidera riassegnare.

1. Fai clic sul widget **[!UICONTROL Assegnazioni]** e rimuoviti dalla richiesta, quindi digita il nome dell&#39;utente a cui desideri riassegnare la richiesta.

   >[!TIP]
   >
   >Se la richiesta di lavoro è ancora nello stato Pronto per l&#39;avvio o Non pronto, è possibile utilizzare il pulsante **[!UICONTROL Riassegna]** nel menu **[!UICONTROL Altro]** del [!UICONTROL Elenco lavori].\
   >![Pulsante Riassegna](assets/reassign-in-left-panel-350x204.png)

1. Se lo stato di un&#39;attività viene modificato in [!UICONTROL Nuovo] o [!UICONTROL In corso] dopo il completamento, è necessario annullare l&#39;assegnazione dell&#39;utente, salvare l&#39;attività e riassegnare l&#39;utente affinché l&#39;attività venga nuovamente visualizzata nella sezione Elenco lavori dell&#39;area Home.

## Rispondere a una richiesta

È possibile rispondere a una richiesta per chiarire ulteriormente la richiesta o proporre una nuova data.

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Nell&#39;area **[!UICONTROL Elenco lavori]** selezionare la richiesta a cui si desidera rispondere.
1. Individua la persona che ti ha assegnato la richiesta.

   Queste informazioni sono disponibili nella scheda [!UICONTROL Aggiornamenti] dell&#39;attività. Assicurarsi che l&#39;opzione **[!UICONTROL Mostra aggiornamenti di sistema]** sia abilitata.

1. Fai clic su **[!UICONTROL Avvia nuovo aggiornamento]** e inizia a digitare la risposta.
1. Immetti il nome del destinatario nella casella **[!UICONTROL Notify]**, quindi fai clic su **[!UICONTROL Update]**.

   >[!TIP]
   >
   >Se la richiesta di lavoro è ancora nello stato Pronto per l&#39;avvio o [!UICONTROL Non pronto], è possibile utilizzare il pulsante **[!UICONTROL Rispondi]** nel menu **[!UICONTROL Altro]** in [!UICONTROL Elenco lavori].\
   >![[!UICONTROL Pulsante Rispondi]](assets/reassign-in-left-panel-350x204.png)   >

## Lavorare su una richiesta

Quando si fa clic sul pulsante [!UICONTROL Lavoraci], si indica all&#39;utente che ha inviato la richiesta e a qualsiasi altro utente che potrebbe essere assegnato alla richiesta che si sta per iniziare a lavorare sulla richiesta. Per ulteriori informazioni sull&#39;utilizzo delle richieste, vedere [Gestire le richieste del team e del lavoro](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Nell&#39;area **[!UICONTROL Elenco lavori]**, seleziona la richiesta su cui vuoi lavorare, quindi fai clic su **[!UICONTROL Lavoraci]**.\
   Le informazioni sul problema vengono visualizzate nel pannello di destra.

## Rimuovere una richiesta

Se decidi di non lavorare sulla richiesta, puoi convertire l’attività o il problema in una richiesta o rimuoverla dall’elenco.

1. Fai clic sul **[!UICONTROL menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Nella **[!UICONTROL Elenco lavori]**, selezionare l&#39;elemento in attesa di elaborazione.
1. Fai clic sul widget **[!UICONTROL Assegnazioni]** e rimuovi te stesso. Questo rimuove l’elemento di lavoro dall’elenco di lavoro. Se la richiesta non viene assegnata ad altri utenti o a un altro team o mansione, la richiesta viene lasciata senza assegnazione.

   Oppure

   Fai clic sull&#39;icona del menu **[!UICONTROL Altro]** ![](assets/more-icon.png) a destra del nome dell&#39;attività o del problema nell&#39;elenco [!UICONTROL Lavoro principale].

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Selezionare una delle opzioni seguenti:

   * **[!UICONTROL Converti in richiesta di lavoro]:** Selezionare questa opzione per convertire nuovamente l&#39;elemento di lavoro in una richiesta di lavoro.\

     L’elemento di lavoro viene ritrasferito a una richiesta e l’utente rimane assegnato alla richiesta.\
      Puoi accettare la richiesta in un secondo momento facendo nuovamente clic su **[!UICONTROL Lavoraci]**.

   * **[!UICONTROL Rimuovi]:** Seleziona questa opzione per rimuovere una richiesta dal tuo [!UICONTROL Elenco lavori].\

     Sei stato rimosso dall&#39;assegnazione della richiesta e questa non è più associata al tuo nome in [!DNL Adobe Workfront].\
      Se la richiesta non viene assegnata ad altri utenti o a un altro team o mansione, la richiesta viene lasciata senza assegnazione.
