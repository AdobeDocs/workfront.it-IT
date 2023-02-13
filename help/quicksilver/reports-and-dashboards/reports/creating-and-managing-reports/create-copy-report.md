---
product-area: reporting;user-management
keywords: salva,nuovo,rapporto,copia
navigation-topic: create-and-manage-reports
title: Creare una copia di un rapporto
description: Puoi creare una copia di qualsiasi rapporto a cui hai accesso. Puoi creare una copia esatta di un rapporto personalizzato oppure salvare una nuova versione di un rapporto predefinito. Dopo aver copiato un rapporto, diventerai il proprietario del rapporto copiato e verrà visualizzato nella sezione Rapporti personali .
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Creare una copia di un rapporto

Puoi creare una copia di qualsiasi rapporto a cui hai accesso. Puoi creare una copia esatta di un rapporto personalizzato oppure salvare una nuova versione di un rapporto predefinito. Dopo aver copiato un rapporto, diventerai il proprietario del rapporto copiato e verrà visualizzato nella sezione Rapporti personali .

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un report</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare una copia esatta di un rapporto

Se desideri creare una copia di un rapporto di cui sei il proprietario, procedi come segue:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Rapporti**, quindi **Tutti i report**.
1. Apri un report.
1. Fai clic su **Azioni dei rapporti**, quindi **Copia**.

   >[!TIP]
   >
   >Se il rapporto è un rapporto predefinito, l&#39;opzione Copia non viene visualizzata nel menu Azioni rapporto.\
   >Per informazioni su come creare una copia di un rapporto predefinito, vedi [Creare una nuova versione di un rapporto](#create-a-new-version-of-a-report).

   ![Copia rapporto](assets/nwe-fulllistofreportactions-2022.png)

   Viene creata una copia del rapporto originale con il nome predefinito di *Copia di [Nome del rapporto originale]*. Ad esempio, il nome del rapporto &quot;Attività completate Q4&quot; avrebbe &quot;Copia delle attività completate Q4&quot;.

1. (Facoltativo) Per rinominare il rapporto, inizia a digitare un nuovo nome.

   >[!TIP]
   >
   >Se si deseleziona il titolo prima di digitare il nuovo nome, selezionare il titolo del rapporto, eliminare il nome, quindi immettere il nuovo nome.

1. (Facoltativo) Per condividere la nuova versione del rapporto con altri utenti, fai clic su **Azioni dei rapporti**, quindi **Condivisione**.

   >[!NOTE]
   >
   >Le informazioni di condivisione non vengono trasferite al report copiato dalla versione originale.\
   >Per informazioni su come vedere con chi è stato condiviso il rapporto precedente, vedi [Creare un rapporto sulle attività di reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Facoltativo) Se disponi delle autorizzazioni Gestisci per il rapporto originale e il rapporto originale non è più necessario, puoi eliminarlo per rimuovere i rapporti duplicati non necessari in Workfront.

   Per eliminare il rapporto originale, procedi come segue:

   1. Passa al rapporto .
   1. Fai clic su **Azioni dei rapporti**, quindi **Elimina**.

   1. Fai clic su **Sì, Elimina** per confermare l’eliminazione del rapporto.

## Creare una nuova versione di un rapporto {#create-a-new-version-of-a-report}

Se desideri creare una copia di un rapporto predefinito, procedi come segue:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Rapporti**, quindi **Tutti i report**.
1. Fai clic sul nome di un rapporto predefinito per aprirlo.
1. Fai clic su **Azioni dei rapporti**, quindi **Modifica**.

   ![Modifica rapporto](assets/nwe-reportactionsfordefaultreport-2022.png)

1. Apporta le modifiche necessarie nelle seguenti schede del rapporto:

   * **Colonne (visualizzazione)**: Per ulteriori informazioni sulla personalizzazione delle visualizzazioni, consulta l’articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Raggruppamenti**: Per ulteriori informazioni sulla personalizzazione dei raggruppamenti, consulta l’articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtri**: Per ulteriori informazioni sulla personalizzazione dei filtri, consulta l’articolo [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Grafico**: Per ulteriori informazioni sulla personalizzazione di un grafico a rapporti, consulta l’articolo [Aggiungere un grafico a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Nell’angolo in alto a destra, fai clic su **Impostazioni dei rapporti**.
1. In **Titolo rapporto** assegnare un nuovo nome al report.
1. Fai clic su **Fine**.
1. Fai clic su **Salva come nuovo rapporto**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Facoltativo) Per condividere la nuova versione del rapporto con altri utenti, fai clic su **Azioni dei rapporti**, quindi **Condivisione**.
