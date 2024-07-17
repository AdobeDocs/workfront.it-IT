---
product-area: reporting
navigation-topic: report-usage
title: Visualizza utilizzo report
description: Visualizza utilizzo report
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 1%

---

# Visualizza utilizzo report

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Per comprendere l’utilizzo dei rapporti nel sistema, puoi visualizzare le seguenti informazioni in un elenco di rapporti:

* Ultimi 10 utenti che hanno visualizzato il rapporto
* Visualizza il conteggio entro un intervallo di tempo specificato

  >[!NOTE]
  >
  >Adobe Workfront conta una visualizzazione per utente al giorno. Se accedi allo stesso rapporto più volte al giorno, Workfront conta questa come una visualizzazione per quel rapporto. Se un altro utente accede allo stesso rapporto nello stesso giorno, Workfront lo considera come una nuova visualizzazione per il secondo utente.

* Data ultima visualizzazione
* Ultima visualizzazione per utente
* Elenco delle dashboard che contengono il rapporto\
  Per ulteriori informazioni sulla visualizzazione del nome delle dashboard in cui potrebbero essere aggiunti i report in un elenco di report, vedere l&#39;articolo [Informazioni su come organizzare i report in una dashboard](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

È possibile creare una visualizzazione per un elenco di rapporti in cui visualizzare queste informazioni.\
Puoi filtrare un elenco di rapporti in base ad alcuni di questi campi.\
Per ulteriori informazioni sui campi in base ai quali è possibile filtrare un report, vedere l&#39;articolo [Filtrare un elenco di report in base alle informazioni sull&#39;utilizzo](#filter-a-report-list-by-usage-information).

## Requisiti di accesso

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare le informazioni sull&#39;utilizzo del report nella visualizzazione di un elenco di report

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Rapporti**.

1. Nell&#39;elenco dei report fare clic sul menu a discesa **Visualizza**.
1. (Facoltativo) Seleziona la visualizzazione **Utilizzo report** per visualizzare le informazioni più comuni sull&#39;utilizzo del report.\
   Oppure

1. Fai clic su **Nuova visualizzazione** per creare una visualizzazione personalizzata.
1. Fai clic su **Aggiungi colonna**.
1. Inizia a digitare uno dei campi seguenti e selezionali quando vengono visualizzati nell&#39;elenco sotto l&#39;oggetto **Report** per aggiungerli a una nuova colonna:

   * **Ultimi 10 utenti**: visualizza i nomi degli ultimi 10 utenti che hanno visualizzato il report.
   * **Visualizzazioni**: visualizza il numero di visualizzazioni in uno dei seguenti intervalli di tempo:

      * **Questo Mese, Trimestre, Anno**
      * **Ultimo mese, trimestre, anno**
      * **Tutte le visualizzazioni**: visualizza un conteggio complessivo per tutte le visualizzazioni nel report

   * **Ultima visualizzazione di**: visualizza informazioni sull&#39;ultimo utente che ha visualizzato il report
   * **Data ultima visualizzazione**: visualizza la data dell&#39;ultima visualizzazione del report

1. Fai clic su **Salva vista**.\
   Le informazioni sull&#39;utilizzo del report vengono visualizzate nelle colonne aggiunte alla visualizzazione.\
   È inoltre possibile creare un report per l&#39;oggetto report e utilizzare questa visualizzazione nel report.\
   Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Per generare un rapporto è necessario disporre dell’accesso in modifica ai rapporti nel proprio livello di accesso.\
   Per ulteriori informazioni sull&#39;accesso ai report, vedere l&#39;articolo [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrare un elenco di rapporti in base alle informazioni sull’utilizzo {#filter-a-report-list-by-usage-information}

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Rapporti**.
1. Nell&#39;elenco dei report fare clic sul menu a discesa **Filtro**.
1. Fai clic su **Nuovo filtro**, quindi fai clic su **Aggiungi una regola filtro**.
1. Inizia a digitare uno dei campi seguenti e selezionali quando vengono visualizzati nell&#39;elenco sotto l&#39;oggetto **Report** per aggiungerli come nuova regola di filtro:

   * **Visualizzazioni**: visualizza il numero di visualizzazioni in uno dei seguenti intervalli di tempo:

      * **Questo Mese, Trimestre, Anno**
      * **Ultimo mese, trimestre, anno**
      * **Tutte le visualizzazioni**

   * **Ultima visualizzazione di**: visualizza informazioni sull&#39;ultimo utente che ha visualizzato il report
   * **Data ultima visualizzazione**: visualizza la data dell&#39;ultima visualizzazione del report

1. Seleziona un modificatore per il campo, quindi specifica un valore, quando richiesto.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Fai clic su **Salva filtro**.\
   Viene visualizzato un elenco di rapporti che soddisfano le informazioni di utilizzo definite.\
   È inoltre possibile creare un report per l&#39;oggetto report e utilizzare questo filtro nel report.\
   Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Per generare un rapporto è necessario disporre dell’accesso in modifica ai rapporti nel proprio livello di accesso.\
   Per ulteriori informazioni sull&#39;accesso ai report, vedere l&#39;articolo [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Eccezioni durante la visualizzazione delle informazioni sull’utilizzo del rapporto

>[!IMPORTANT]
>
>Le informazioni sull’utilizzo del rapporto sono state raccolte da marzo 2018. Tutte le informazioni precedenti a questa data non sono disponibili.

Di seguito sono riportate alcune eccezioni di cui tenere conto quando si utilizzano le informazioni sull’utilizzo dei rapporti:

* Ogni volta che un rapporto viene visualizzato su un dashboard o su una scheda personalizzata, viene conteggiato come una visualizzazione. L’utente che visualizza il report sul proprio dashboard viene visualizzato come utente Last View By: Name (Ultima visualizzazione di: Nome) e la data in cui è stato visualizzato il dashboard viene visualizzata come data Last Viewed On (Ultima visualizzazione il).
* Workfront non raccoglie informazioni sull’utilizzo per i rapporti incorporati.\
  Per ulteriori informazioni sui report integrati di Workfront, vedere l&#39;articolo [Utilizzare i report integrati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront non raccoglie informazioni sull’utilizzo dei rapporti consegnati. Un rapporto consegnato non conta come una visualizzazione.\
  Per ulteriori informazioni sui report consegnati, consulta l&#39;articolo [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Quando un amministratore di sistema o di gruppo effettua l’accesso come altro utente, le visualizzazioni vengono conteggiate e associate all’amministratore di sistema o di gruppo.
* Workfront non raccoglie informazioni sull’utilizzo per i rapporti per trimestri personalizzati. Solo i trimestri predefiniti standard sono indicati nei campi di utilizzo del rapporto.
* Workfront non raccoglie informazioni sull’utilizzo per i rapporti condivisi e visualizzati pubblicamente. Quando un report pubblico viene visualizzato da un utente che non ha effettuato l’accesso a Workfront, le visualizzazioni del report non vengono conteggiate.\
  Per ulteriori informazioni sulla condivisione di report, vedere l&#39;articolo [Condividere un report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
