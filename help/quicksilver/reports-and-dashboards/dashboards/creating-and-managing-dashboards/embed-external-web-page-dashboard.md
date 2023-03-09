---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporare una pagina web esterna in una dashboard
description: Puoi incorporare una pagina web esterna in una dashboard per fornire accesso alle informazioni correlate provenienti da altri sistemi all’interno di Adobe Workfront o da altre pagine Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: a8a3aec50b5538de5867ce3ba7723d92c046b50d
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Incorporare una pagina web esterna in una dashboard

Puoi incorporare una pagina web esterna in una dashboard per fornire accesso alle informazioni correlate provenienti da altri sistemi all’interno di Adobe Workfront o da altre pagine Workfront.

Ad esempio, se la tua organizzazione dispone di un archivio documenti basato su Web, di un wiki o di un altro sistema di gestione dei contenuti che contiene informazioni sul progetto a cui si accede regolarmente tramite un URL, puoi visualizzare tali informazioni in Workfront creando una pagina esterna su un dashboard.

>[!IMPORTANT]
>
>Per motivi di sicurezza, alcuni siti web non consentono di incorporare le pagine web come iframe. Se la pagina web che desideri incorporare in un dashboard non lo consente, la pagina non viene visualizzata nel dashboard. Tuttavia, è comunque possibile accedere alla pagina esterna facendo clic sul nome della dashboard.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Per consentire l’incorporamento per un sito web di tua proprietà, rivolgiti al tuo amministratore web per modificare **X-Frame-Options** impostazione. Per ulteriori informazioni, consulta [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).


>[!IMPORTANT]
>
>Le pagine del dashboard non sono più supportate come pagine esterne incorporate nei dashboard. In particolare, i seguenti sottodomini Workfront.com non sono più supportati:
>
>* /dashboard&#x200B;
>* /dashboard/:ID&#x200B;
>* /portfolio/:ID/content-dashboard__:dashboardID&#x200B;
>* /program/:ID/content-dashboard__:dashboardID&#x200B;
>* /project/:ID/content-dashboard__:dashboardID&#x200B;
>* /task/:ID/content-dashboard__:dashboardID&#x200B;
>* /template/:ID/content-dashboard__:dashboardID&#x200B;
>* /templatetask/:ID/content-dashboard__:dashboardID&#x200B;
>* /resourcemanagement/:ID/content-dashboard__:dashboardID&#x200B;
>* /team/:ID/content-dashboard__:dashboardID&#x200B;
>* /iteration/:ID/content-dashboard__:dashboardID&#x200B;
>* /requests/:ID/content-dashboard__:dashboardID&#x200B;
>* /group/:ID/content-dashboard__:dashboardID&#x200B;
>* /billingrecord/:ID/content-dashboard__:dashboardID


## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a rapporti, dashboard e calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per il dashboard</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un dashboard prima di incorporarvi una pagina esterna.

Per informazioni sulla creazione di dashboard, consulta [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Incorporare una pagina esterna in una dashboard

>[!IMPORTANT]
>
>Se non è più necessario, è possibile rimuovere una pagina esterna da un dashboard. Tuttavia, non è possibile eliminare una pagina esterna dopo che è stata creata in Workfront. Puoi eliminare una pagina esterna solo utilizzando l’API. Per ulteriori informazioni, consulta [Rimuovere una pagina esterna da un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Individua l’URL della pagina da visualizzare in Workfront e copia l’URL che si trova nella barra degli indirizzi.

   >[!NOTE]
   >
   >Se condividi gli URL di oggetti Workfront, ricorda che alcuni URL scadono nel tempo. Ad esempio, gli URL del documento scadono dopo l’apertura. Questo è configurato come misura di sicurezza e, per progettazione, è considerato un URL non statico e non deve essere condiviso.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Dashboard**.

1. Per modificare un dashboard esistente, seleziona il dashboard in cui desideri incorporare la pagina del sito web, quindi fai clic su **Azioni dashboard**, e seleziona **Modifica** dal menu.\
   Oppure\
   Per creare un nuovo dashboard, fai clic su **Nuovo dashboard**.\
   Per ulteriori informazioni sulla creazione di un dashboard, consulta [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Clic **Aggiungi pagina esterna**.

   ![](assets/qs-add-external-page-350x239.png)

1. Specifica un **Nome** per la pagina esterna.
1. Specifica un **Descrizione**.
1. Incolla l’URL copiato in precedenza in **URL** campo.\
   Puoi specificare i seguenti tipi di URL:

   * Un URL https (crittografato) di una pagina web.\
      Solo le pagine https (crittografate) vengono caricate con l’URL.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * URL del modello che contiene informazioni sulla sessione per un sito Web specifico.\
      Ad esempio: *https://localhost/?session={$$SESSION}*
Per visualizzare la pagina esterna, è necessario aver effettuato l&#39;accesso al sito Web specificato.\
      Per informazioni su come ottenere un ID sessione da Workfront, vedi [Nozioni di base sulle API](../../../wf-api/general/api-basics.md).\
      L’amministratore di Workfront può configurare le preferenze di sistema in modo da non consentire l’utilizzo delle informazioni sulla sessione nelle pagine esterne per motivi di sicurezza. In questo caso, la pagina esterna non viene caricata sul dashboard.\
      Per ulteriori informazioni sulle preferenze di protezione del sistema, vedere [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Fai clic su **Salva**.\
   La pagina viene aggiunta automaticamente al dashboard. Se vengono create dashboard future, è possibile aggiungere la pagina esterna. La pagina esterna si trova tra i Report disponibili.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Aggiornare una pagina esterna in un dashboard

Per aggiornare le informazioni per una pagina esterna utilizzata in un dashboard:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png), quindi fai clic su **Dashboard**.
1. Seleziona la dashboard da aggiornare, quindi fai clic su **Modifica** ![](assets/edit-icon.png).

   ![Seleziona l’icona Modifica.](assets/nwe-editdashboard2021-350x188.png)

1. Nella parte destra dello schermo, individua la pagina esterna che desideri aggiornare e fai clic sul pulsante **Modifica** icona.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. In **Modifica pagina esterna** , aggiorna i campi da modificare, quindi fai clic su **Salva**.
1. (Facoltativo) Fai clic su **Elimina** icona ![](assets/delete.png) per rimuovere la pagina esterna dal dashboard. Per ulteriori informazioni, consulta [Rimuovere una pagina esterna da un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Nell’angolo in basso a sinistra, fai clic su **Salva e chiudi**.

## Visualizzare pagine esterne in un rapporto

Puoi visualizzare tutte le pagine esterne in Workfront in un rapporto di pagina esterna.

1. Vai a **Menu principale** icona ![](assets/main-menu-icon.png) > **Rapporti**.
1. Clic **Nuovo rapporto** > seleziona **Pagina esterna**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Facoltativo) Aggiorna le schede Visualizza, Filtri o Raggruppamenti del rapporto.

   Per ulteriori informazioni, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Clic **Salva+Chiudi**.

   Puoi visualizzare il nome e l’URL associati alle pagine esterne nel tuo sistema nel nuovo rapporto.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
