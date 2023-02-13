---
product-area: reporting
navigation-topic: report-usage
title: Visualizzazione dell'utilizzo dei rapporti
description: Visualizzazione dell'utilizzo dei rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Visualizzazione dell&#39;utilizzo dei rapporti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Per capire in che modo vengono utilizzati i rapporti nel sistema, puoi visualizzare le seguenti informazioni in un elenco di rapporti:

* Ultimi 10 utenti che hanno visualizzato il rapporto
* Visualizza il conteggio entro un intervallo di tempo specificato

   >[!NOTE]
   >
   >Adobe Workfront conta una visualizzazione al giorno per utente. Se accedi allo stesso rapporto più volte al giorno, Workfront lo considera come una visualizzazione per quel rapporto. Se un altro utente accede allo stesso report nello stesso giorno, Workfront lo considera come una nuova visualizzazione per il secondo utente.

* Data ultima visualizzazione
* Ultima visualizzazione per utente
* Elenco di dashboard contenenti il rapporto\
   Per ulteriori informazioni sulla visualizzazione del nome delle dashboard sulle quali è possibile aggiungere rapporti in un elenco di rapporti, consulta l’articolo [Informazioni su come organizzare i rapporti in un dashboard](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

È possibile creare una visualizzazione per un elenco di rapporti in cui visualizzare tali informazioni.\
È possibile filtrare un elenco di rapporti in base ad alcuni di questi campi.\
Per ulteriori informazioni sui campi in cui è possibile filtrare un rapporto, consulta l’articolo [Filtrare un elenco di rapporti in base alle informazioni di utilizzo](#filter-a-report-list-by-usage-information).

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
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizzazione delle informazioni di utilizzo del rapporto nella visualizzazione di un elenco di rapporti

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.

1. Nell’elenco dei rapporti, fai clic sul pulsante **Visualizza** menu a discesa.
1. (Facoltativo) Seleziona la **Utilizzo dei rapporti** per visualizzare le informazioni di utilizzo più comuni del rapporto.\
   Oppure

1. Fai clic su **Nuova vista** per creare una visualizzazione personalizzata.
1. Fai clic su **Aggiungi colonna**.
1. Inizia a digitare uno dei campi seguenti e selezionali quando compaiono nell’elenco sotto la **Rapporto** per aggiungerli a una nuova colonna:

   * **Ultimi 10 utenti**: Visualizza i nomi degli ultimi 10 utenti che hanno visualizzato il rapporto.
   * **Viste**: Visualizza il numero di visualizzazioni entro uno dei seguenti intervalli di tempo:

      * **Questo mese, trimestre, anno**
      * **Mese Scorso, Trimestre, Anno**
      * **Tutte le visualizzazioni**: Visualizza un conteggio complessivo per tutte le visualizzazioni del rapporto
   * **Ultima visualizzazione di**: Visualizza informazioni sull&#39;utente che ha visualizzato il rapporto per ultimo
   * **Data ultima visualizzazione**: Visualizza la data dell’ultima visualizzazione del rapporto


1. Fai clic su **Salva visualizzazione**.\
   Le informazioni sull’utilizzo del rapporto vengono visualizzate nelle colonne aggiunte alla visualizzazione.\
   È inoltre possibile creare un report per l&#39;oggetto report e utilizzarlo nel report.\
   Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Per creare un rapporto, devi disporre dell’accesso Modifica ai rapporti nel livello di accesso.\
   Per ulteriori informazioni sull’accesso ai rapporti, consulta l’articolo [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrare un elenco di rapporti in base alle informazioni di utilizzo {#filter-a-report-list-by-usage-information}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.
1. Nell’elenco dei rapporti, fai clic sul pulsante **Filtro** menu a discesa.
1. Fai clic su **Nuovo filtro**, quindi fai clic su **Aggiungere una regola filtro**.
1. Inizia a digitare uno dei campi seguenti e selezionali quando compaiono nell’elenco sotto la **Rapporto** oggetto per aggiungerli come nuova regola di filtro:

   * **Viste**: Visualizza il numero di visualizzazioni entro uno dei seguenti intervalli di tempo:

      * **Questo mese, trimestre, anno**
      * **Mese Scorso, Trimestre, Anno**
      * **Tutte le Viste**
   * **Ultima visualizzazione di**: Visualizza informazioni sull&#39;utente che ha visualizzato il rapporto per ultimo
   * **Data ultima visualizzazione**: Visualizza la data dell’ultima visualizzazione del rapporto


1. Selezionare un modificatore per il campo, quindi specificare un valore quando richiesto.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Fai clic su **Salva filtro**.\
   Viene visualizzato un elenco di rapporti che corrispondono alle informazioni di utilizzo definite.\
   È inoltre possibile creare un rapporto per l&#39;oggetto report e utilizzare questo filtro nel report.\
   Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Per creare un rapporto, devi disporre dell’accesso Modifica ai rapporti nel livello di accesso.\
   Per ulteriori informazioni sull’accesso ai rapporti, consulta l’articolo [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Eccezioni durante la visualizzazione delle informazioni di utilizzo del rapporto

>[!IMPORTANT]
>
>Le informazioni sull’utilizzo dei rapporti sono state raccolte a partire da marzo 2018. Tutte le informazioni precedenti a questa data non sono disponibili.

Di seguito sono riportate alcune eccezioni di cui tenere conto quando si lavora con le informazioni di utilizzo del rapporto:

* Ogni volta che un rapporto viene visualizzato su un dashboard o una scheda personalizzata, viene conteggiato come una visualizzazione. L’utente che visualizza il rapporto sul proprio dashboard viene visualizzato come Ultima visualizzazione per: L’utente del nome e la data in cui è stato visualizzato il dashboard vengono visualizzati come Data ultima visualizzazione.
* Workfront non raccoglie informazioni di utilizzo per i rapporti incorporati.\
   Per ulteriori informazioni sui rapporti incorporati di Workfront, consulta l’articolo [Utilizzare i report incorporati di Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront non raccoglie informazioni sull’utilizzo dei report consegnati. Un rapporto consegnato non viene conteggiato come una visualizzazione.\
   Per ulteriori informazioni sui rapporti consegnati, consulta l’articolo [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Quando un amministratore di sistema o di gruppo effettua l’accesso come un altro utente, le visualizzazioni vengono conteggiate e associate all’amministratore di sistema o di gruppo.
* Workfront non raccoglie informazioni sull’utilizzo dei rapporti per trimestri personalizzati. Nei campi di utilizzo del rapporto sono indicati solo i trimestri incorporati standard.
* Workfront non raccoglie informazioni di utilizzo per i rapporti condivisi e visualizzati pubblicamente. Quando un report pubblico viene visualizzato da un utente senza accedere a Workfront, le visualizzazioni del report non vengono conteggiate.\
   Per ulteriori informazioni sulla condivisione dei rapporti, consulta l’articolo [Condivisione di un rapporto in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
