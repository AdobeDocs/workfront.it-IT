---
content-type: overview
title: Panoramica dei breadcrumb
description: Le breadcrumb visualizzano la gerarchia di navigazione completa per tutti i tipi di oggetto.
feature: Get Started with Workfront
exl-id: c4103f8e-4c3f-4d4d-a0eb-628c60735ab7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VryLEVTqJFgAxlm-al5y0hqxVQ71zFPi8YG1oAlox8k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 8771d66f6b7ecae9ac439456822889d4fe438649
workflow-type: tm+mt
source-wordcount: 334
ht-degree: 1%

---

# Panoramica dei breadcrumb

Le breadcrumb visualizzano la gerarchia di navigazione completa per tutti i tipi di oggetto. Ogni oggetto nel percorso della breadcrumb ha un’etichetta che visualizza il tipo di oggetto. La pagina su cui ti trovi attualmente viene visualizzata sia nell’intestazione della pagina che alla fine del percorso della breadcrumb in corsivo. Nell&#39;esempio seguente, questa è l&#39;attività &quot;[!UICONTROL Condividi con Brand Team]&quot;.

![Breadcrumb compresso](assets/collapsed-breadcrumb-2026.png)

Se nel percorso delle breadcrumb sono presenti troppi oggetti o la larghezza dello schermo non consente la visualizzazione dell&#39;intera gerarchia di navigazione, il percorso comprime alcuni dei breadcrumb e raggruppa tali oggetti all&#39;inizio del percorso delle breadcrumb. Sia il progetto che la pagina oggetto corrente sono sempre visibili nel percorso della breadcrumb.

Ad esempio, &quot;3 more&quot; nell’immagine precedente indica che 3 oggetti non vengono visualizzati. Questi elementi possono trovarsi al di sopra del livello del progetto o tra il progetto e la pagina corrente.

Facendo clic su &quot;[!UICONTROL altro]&quot; è possibile espandere la gerarchia completa. Puoi fare clic su &quot;[!UICONTROL Meno]&quot; per comprimere nuovamente il percorso delle breadcrumb.

![Breadcrumb compresso](assets/expanded-breadcrumb-2026.png)

Per spostarsi tra le breadcrumb, è inoltre possibile utilizzare i tasti seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Scheda</strong> </td> 
   <td> <p>Passa a ogni elemento nelle breadcrumb</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Invio</strong> </td> 
   <td> <p>Espandere un percorso di breadcrumb compresso, comprimere un percorso di breadcrumb espanso e aprire una nuova pagina in un collegamento a un oggetto</p> </td> 
  </tr> 
 </tbody> 
</table>



<!--
drafted: this is no longer possible, since we removed Campaigns, but it might come back as part of Maestro: 

## Multi-object breadcrumbs

>[!NOTE]
>
>The information in this article is available only in the Preview environment when you participate in the [!UICONTROL Campaigns] beta program. The functionality described here might not be fully available yet. For more information about current available features and how to enroll, see [Campaigns beta].

Some objects can belong to multiple parent objects. For example, a project can belong to multiple campaigns. In this case, all the campaigns that the project belongs to display in the breadcrumb.

The multi-object listing in the breadcrumb (for example, the campaigns) displays the number of parent objects which expands into a list to display all the campaigns that the project is associated with. For more information, see [Add objects to a campaign](../../manage-work/campaigns/add-objects-to-a-campaign.md).


![Project with multiple campaigns in the breadcrumb](assets/project-with-multiple-campaigns-in-breadcrumb.png)

-->

## Accedere a un oggetto padre dalle breadcrumb

Per informazioni sugli oggetti padre in [!DNL Workfront], vedere [Informazioni sugli oggetti in [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Condizionale) Se l&#39;oggetto a cui si desidera passare non viene visualizzato in un percorso di breadcrumb compresso, fare clic su **[!UICONTROL altro]**, quindi individuare l&#39;oggetto.

   >[!NOTE]
   >
   >Se non disponi dell’autorizzazione per un oggetto, questo non sarà visibile nelle breadcrumb.

1. Fai clic su un oggetto nel percorso della breadcrumb per accedervi.

   Viene visualizzata la pagina oggetto.

   Se si sta esaminando un progetto connesso a un oggetto in Workfront Planning, ad esempio una campagna, è possibile passare dal tipo di oggetto Planning a quello di Workfront dalla breadcrumb. Per ulteriori informazioni, vedere [Panoramica della gerarchia e delle breadcrumb](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
