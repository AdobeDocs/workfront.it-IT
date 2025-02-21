---
product-area: reporting;user-management
keywords: salva,nuovo,report,copia
navigation-topic: create-and-manage-reports
title: Creare una copia di un rapporto
description: Puoi creare una copia di qualsiasi rapporto a cui hai accesso. È possibile creare una copia esatta di un rapporto personalizzato oppure salvare una nuova versione di un rapporto predefinito. Dopo aver copiato un report, l'utente diventa il proprietario del report copiato e viene visualizzato nella sezione I miei report.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Creare una copia di un rapporto

<!-- Audited: 11/2024 -->

Puoi creare una copia di qualsiasi rapporto a cui hai accesso. È possibile creare una copia esatta di un rapporto personalizzato oppure salvare una nuova versione di un rapporto predefinito. Dopo aver copiato un report, l&#39;utente diventa il proprietario del report copiato e viene visualizzato nella sezione I miei report.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto*</td> 
   <td><p>Visualizzare le autorizzazioni per un rapporto</p></td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una copia esatta di un rapporto

Se si desidera creare una copia di un report personalizzato, eseguire le operazioni seguenti:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Reports]**.

1. Fai clic su **Tutti i report**, quindi apri un report.

1. Fai clic su **Azioni report**, quindi su **Copia**.

   >[!TIP]
   >
   >Se si tratta di un report predefinito, l&#39;opzione Copia non viene visualizzata nel menu Azioni report.\
   >Per informazioni su come creare una copia di un report predefinito, vedere [Creare una nuova versione di un report](#create-a-new-version-of-a-report).

   ![Copia report](assets/unshimmed-report-actions-copy.png)

   Viene creata una copia del report originale con il nome predefinito _[Nome del report originale] (copia)_. Ad esempio, una copia del rapporto &quot;Q4 Completed Tasks&quot; (Attività completate Q4) sarebbe denominata &quot;Q4 Completed Tasks (Copy)&quot;.

1. (Facoltativo) Per rinominare il report, fare clic su **Azioni report** e quindi su **Modifica**. Digita un nuovo nome nella casella di testo nell&#39;angolo in alto a sinistra, quindi fai clic su **Salva + Chiudi** al termine.

1. (Facoltativo) Per condividere la nuova versione del report con altri utenti, fai clic su **Azioni report**, quindi su **Condivisione**.

   >[!NOTE]
   >
   >Le informazioni di condivisione non vengono trasferite al report copiato dalla versione originale.\
   >Per informazioni su come vedere con chi è stato condiviso il report precedente, vedere [Creare un report sulle attività di reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Facoltativo) Se disponi delle autorizzazioni di gestione per il rapporto originale e il rapporto originale non è più necessario, puoi eliminarlo per rimuovere i rapporti duplicati non necessari in Workfront.

   Per eliminare il report originale, effettuare le seguenti operazioni:

   1. Passa al rapporto.

   1. Fai clic su **Azioni report**, quindi su **Elimina**.

   1. Fare clic su **Sì, Elimina** per confermare l&#39;eliminazione del report.

## Creare una nuova versione di un rapporto {#create-a-new-version-of-a-report}

Se si desidera creare una copia di un report predefinito, eseguire le operazioni seguenti:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront.

1. Fai clic su **Rapporti**, quindi su **Tutti i rapporti**.
1. Fare clic sul nome di un report predefinito per aprirlo.
1. Fai clic su **Azioni report**, quindi su **Modifica**.

   ![Modifica report](assets/unshimmed-report-actions-default-report.png)

1. Apporta le modifiche necessarie nelle seguenti schede del rapporto:

   * **Colonne (visualizzazione)**: per ulteriori informazioni sulla personalizzazione delle visualizzazioni, vedere l&#39;articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Raggruppamenti**: per ulteriori informazioni sulla personalizzazione dei raggruppamenti, consulta l&#39;articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtri**: per ulteriori informazioni sulla personalizzazione dei filtri, vedere l&#39;articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Grafico**: per ulteriori informazioni sulla personalizzazione di un grafico per report, vedere l&#39;articolo [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Nell&#39;angolo superiore destro fare clic su **Impostazioni report**.
1. Nel campo **Titolo report**, assegna un nuovo nome al report.
1. Fai clic su **Fine**.
1. Fare clic su **Salva come nuovo report**.

   ![Salva come nuovo report](assets/unshimmed-save-as-new-report.png)

1. (Facoltativo) Per condividere la nuova versione del report con altri utenti, fai clic su **Azioni report**, quindi su **Condivisione**.
