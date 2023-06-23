---
product-area: projects
navigation-topic: use-the-home-area
title: Creare elementi di lavoro dall'area Home
description: Creare elementi di lavoro dall'area Home
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Creare elementi di lavoro dall&#39;area Home

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

È possibile creare elementi di lavoro da [!UICONTROL Home] area. È possibile creare attività personali per se stessi, richiedere lavoro ad altri utenti o aggiungere attività a progetti specifici.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker]</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso a [!UICONTROL Edit] o versione successiva per le attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Crea un&#39;attività personale

È possibile creare un&#39;attività personale disponibile solo per l&#39;utente nel [!UICONTROL Home] area:

1. Fai clic su **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell’angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Clic **[!UICONTROL Crea Attività]** > **[!UICONTROL Personale]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. In **[!UICONTROL Nome]** , specificare un nome per l&#39;attività.
1. (Facoltativo) Fai clic su **[!UICONTROL Seleziona data]**, quindi selezionare la data di scadenza dell&#39;attività. Questo imposta il [!UICONTROL Data di completamento Pianificata] per l&#39;attività.\
   È possibile modificare il **[!UICONTROL Data di completamento Pianificata]** facendo clic sulla data nel pannello di destra o modificando il **[!UICONTROL Questa operazione verrà eseguita da]** data direttamente nell’attività.

1. Clic **[!UICONTROL Crea]** per salvare l&#39;attività.\
   L’attività ti viene assegnata ed è disponibile nella [!UICONTROL Home] area.

>[!NOTE]
>
>* Quando crei un’attività personale, questa viene memorizzata in un progetto &quot;nascosto&quot; che non è ricercabile in [!UICONTROL Workfront]. Il progetto si chiama &quot;&lt; Nome utente >&#39;s Tasks&quot; (Attività di). &quot;Nome utente&quot; è il nome completo dell&#39;utente che ha creato l&#39;attività. Puoi accedere a questo progetto solo quando fai clic sull’attività personale nella [!UICONTROL Home] , ad esempio dalla breadcrumb dell’attività.
>
>* A differenza delle normali attività di progetto, le attività personali hanno un set limitato di campi visibili nell’interfaccia di Workfront e non influenzano la timeline o l’avanzamento di alcun progetto. Quando si riassegna un&#39;attività personale a un altro utente, tutti i campi delle attività vengono aggiunti a un&#39;attività personale, ma l&#39;attività rimane nel progetto personale dell&#39;utente che ha creato l&#39;attività.
>
>* Se desideri che le attività personali facciano parte del flusso di lavoro normale, è consigliabile creare un progetto e spostarvi tutte le attività personali.
>
> ![[!UICONTROL Progetto per attività personali]](assets/createworkitems-personal--project-350x105.png)

## Richiedi lavoro da un altro utente

È possibile richiedere il lavoro a un altro utente direttamente dall&#39;area Home. Quando si richiede il lavoro a un altro utente come descritto in questa sezione, l&#39;attività viene visualizzata come richiesta nell&#39;area Home dell&#39;utente fino a quando l&#39;utente non fa clic su **[!UICONTROL Lavoraci]**.

Per richiedere il lavoro a un altro utente da [!UICONTROL Home] area:

1. Fai clic su **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell’angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. Clic **[!UICONTROL Crea Attività]**, quindi seleziona **[!UICONTROL Richiesta]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. In **[!UICONTROL Nome]** , specificare un nome per l&#39;attività.
1. In **[!UICONTROL Assegna a]** , digitare il nome dell&#39;utente, del team o del ruolo che si desidera assegnare, quindi fare clic sul nome quando viene visualizzato nel menu a discesa.
1. In [!UICONTROL Aggiungi come] , selezionare se aggiungere un&#39;attività o un problema.
1. Clic **[!UICONTROL Seleziona data]**, quindi selezionare la data e l&#39;ora di scadenza dell&#39;attività.
1. Clic **[!UICONTROL Crea]** per salvare l&#39;attività.\
   L’attività viene visualizzata come richiesta di lavoro nel [!UICONTROL Home] dell’utente che hai designato.

## Aggiungere un’attività o un problema a un progetto

Puoi aggiungere un’attività o un problema a un progetto esistente direttamente dall’area Home:

1. Fai clic su **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell’angolo superiore destro, quindi fai clic su **Home**.
1. Clic **[!UICONTROL Crea Attività]**, quindi seleziona **[!UICONTROL Attività progetto]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. In **[!UICONTROL Nome]** , specifica un nome per l’attività o il problema.
1. In **[!UICONTROL Assegna a]** , digitare il nome dell&#39;utente, del team o del ruolo che si desidera assegnare, quindi fare clic sul nome quando viene visualizzato nel menu a discesa.
1. Inizia a digitare il nome del progetto in cui desideri creare l’attività o il problema, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.

   >[!IMPORTANT]
   >
   >L’attività o il problema viene visualizzato sul [!UICONTROL Elenco lavori] solo quando il progetto [!UICONTROL Stato] è impostato su [!UICONTROL Corrente].

1. (Condizionale) Per creare un problema, seleziona **[!UICONTROL Problema]** dal **[!UICONTROL Aggiungi come]** menu a discesa. Per impostazione predefinita, **[!UICONTROL Attività]** è selezionato.

1. Clic **[!UICONTROL Seleziona data]**, quindi selezionare la data e l&#39;ora di scadenza dell&#39;attività.
1. Clic **[!UICONTROL Crea]** per salvare l&#39;attività.
