---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporare una pagina web esterna in un dashboard
description: È possibile incorporare una pagina web esterna in un dashboard per fornire accesso alle informazioni correlate da altri sistemi all’interno di Adobe Workfront o ad altre pagine Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: a8a3aec50b5538de5867ce3ba7723d92c046b50d
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Incorporare una pagina web esterna in un dashboard

È possibile incorporare una pagina web esterna in un dashboard per fornire accesso alle informazioni correlate da altri sistemi all’interno di Adobe Workfront o ad altre pagine Workfront.

Ad esempio, se l’organizzazione dispone di un archivio documenti basato su Web, un sistema wiki o un altro sistema di gestione dei contenuti che contiene informazioni di progetto a cui viene regolarmente effettuato l’accesso tramite un URL, è possibile visualizzare tali informazioni in Workfront creando una pagina esterna su un dashboard.

>[!IMPORTANT]
>
>Per motivi di sicurezza, alcuni siti web non consentono di incorporare pagine web come iframe. Se la pagina web da incorporare in un dashboard non lo consente, la pagina non viene visualizzata nel dashboard. Tuttavia, è comunque possibile accedere alla pagina esterna facendo clic sul nome del dashboard.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Per consentire l’incorporazione di un sito Web di tua proprietà, rivolgiti all’amministratore web per regolare **Opzioni X-Frame** impostazione. Per ulteriori informazioni, consulta [Opzioni X-Frame](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).


>[!IMPORTANT]
>
>Le pagine dei dashboard non sono più supportate come pagine esterne incorporate nei dashboard. In particolare, i seguenti sottodomini Workfront.com non sono più supportati:
>
>* /dashboard &#x200B;
>* /dashboard/:ID &#x200B;
>* /portfolio/:ID/content-dashboard__:dashboardID &#x200B;
>* /program/:ID/content-dashboard__:dashboardID &#x200B;
>* /project/:ID/content-dashboard__:dashboardID &#x200B;
>* /task/:ID/content-dashboard__:dashboardID &#x200B;
>* /template/:ID/content-dashboard__:dashboardID &#x200B;
>* /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>* /resourcemanagement/:ID/content-dashboard__:dashboardID &#x200B;
>* /team/:ID/content-dashboard__:dashboardID &#x200B;
>* /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>* /requests/:ID/content-dashboard__:dashboardID &#x200B;
>* /group/:ID/content-dashboard__:dashboardID &#x200B;
>* /billingrecord/:ID/content-dashboard__:dashboardID


## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Accesso a Reports, Dashboard e Calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestione delle autorizzazioni al dashboard</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un dashboard prima di incorporarvi una pagina esterna.

Per informazioni sulla creazione di dashboard, consulta [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Incorporare una pagina esterna in un dashboard

>[!IMPORTANT]
>
>Se non è più necessario, è possibile rimuovere una pagina esterna da un dashboard. Tuttavia, non è possibile eliminare una pagina esterna dopo la sua creazione in Workfront. Puoi eliminare una pagina esterna solo utilizzando l’API . Per ulteriori informazioni, consulta [Rimuovere una pagina esterna da un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Individua l’URL della pagina da visualizzare in Workfront e copia l’URL che si trova nella barra degli indirizzi.

   >[!NOTE]
   >
   >Se condividi URL con oggetti Workfront, ricorda che alcuni URL scadono nel tempo. Ad esempio, gli URL dei documenti scadono dopo l’apertura. Questa configurazione è configurata come misura di sicurezza e per progettazione viene considerata come URL non statici e non deve essere condivisa.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Dashboard**.

1. Per modificare un dashboard esistente, seleziona il dashboard in cui desideri incorporare la pagina del sito Web, quindi fai clic su **Azioni dashboard**, quindi seleziona **Modifica** dal menu.\
   Oppure\
   Per creare un nuovo dashboard, fai clic su **Nuovo dashboard**.\
   Per ulteriori informazioni sulla creazione di un dashboard, consulta [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Fai clic su **Aggiungi pagina esterna**.

   ![](assets/qs-add-external-page-350x239.png)

1. Specifica una **Nome** per la pagina esterna.
1. Specifica una **Descrizione**.
1. Incolla l’URL copiato in precedenza in **URL** campo .\
   Puoi specificare i seguenti tipi di URL:

   * Un URL https (crittografato) per una pagina web.\
      Solo le pagine https (crittografate) vengono caricate con l’URL.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * URL modello contenente informazioni sulla sessione per un sito Web specifico.\
      Ad esempio: *https://localhost/?session=$$SESSION}*
Devi aver effettuato l’accesso al sito web specificato per visualizzare la pagina esterna.\
      Per informazioni su come ottenere un ID sessione da Workfront, vedi [Nozioni di base sulle API](../../../wf-api/general/api-basics.md).\
      Per motivi di sicurezza, l’amministratore di Workfront può configurare le preferenze di sistema in modo da non consentire l’utilizzo delle informazioni sulla sessione nelle pagine esterne. In questo caso, la pagina esterna non viene caricata sul dashboard.\
      Per ulteriori informazioni sulle preferenze di sicurezza del sistema, consulta [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Fai clic su **Salva**.\
   La pagina viene aggiunta automaticamente al dashboard. Se vengono create dashboard future, è possibile aggiungere la pagina esterna. La pagina esterna si trova tra i rapporti disponibili.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Aggiornare una pagina esterna in un dashboard

Per aggiornare le informazioni per una pagina esterna utilizzata in un dashboard:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Dashboard**.
1. Seleziona il dashboard da aggiornare, quindi fai clic su **Modifica** ![](assets/edit-icon.png).

   ![Seleziona l’icona Modifica .](assets/nwe-editdashboard2021-350x188.png)

1. Sul lato destro dello schermo, individua la pagina esterna da aggiornare e fai clic sul pulsante **Modifica** icona.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. In **Modifica pagina esterna** , aggiorna i campi da modificare, quindi fai clic su **Salva**.
1. (Facoltativo) Fai clic sul pulsante **Elimina** icona ![](assets/delete.png) per rimuovere la pagina esterna dal dashboard. Per ulteriori informazioni, consulta [Rimuovere una pagina esterna da un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Nell’angolo in basso a sinistra, fai clic su **Salva e chiudi**.

## Visualizzare pagine esterne in un rapporto

Puoi visualizzare tutte le pagine esterne in Workfront in un rapporto Pagina esterna.

1. Vai a **Menu principale** icona ![](assets/main-menu-icon.png) > **Rapporti**.
1. Fai clic su **Nuovo rapporto** > seleziona **Pagina esterna**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Facoltativo) Aggiorna le schede Visualizza, Filtri o Gruppi del rapporto.

   Per ulteriori informazioni, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Fai clic su **Salva e chiudi**.

   Nel nuovo rapporto puoi visualizzare il nome e l’URL associati alle pagine esterne del sistema.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
