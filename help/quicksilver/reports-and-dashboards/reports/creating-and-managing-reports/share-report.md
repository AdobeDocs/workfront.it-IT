---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Condividere un rapporto in Adobe Workfront
description: L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i rapporti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell’accesso ai problemi, consulta Concedere l’accesso a rapporti, dashboard e calendari.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Condividere un rapporto in Adobe Workfront

<!-- Audited: 11/2024 -->

L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i rapporti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell&#39;accesso ai problemi, vedere [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare o gestire rapporti specifici a cui si ha accesso per la condivisione. Per ulteriori informazioni sui livelli di accesso e sulle autorizzazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per condividere gli oggetti, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
      <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Chiaro o superiore</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Revisione o successiva</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o superiore a report, dashboard, calendari</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni o superiore al report</p></td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla condivisione dei rapporti

Oltre alle considerazioni seguenti, vedere anche [Condividere report, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Puoi condividere i rapporti che hai creato con altri individui, team, gruppi, mansioni o aziende. Puoi anche condividere i rapporti creati da altri utenti e che sono stati condivisi con te.
* Puoi anche condividerli con l’intera organizzazione o renderli pubblici. Rendendo pubblico un report viene generato un URL che può essere condiviso con altri utenti.
* Puoi condividere un singolo rapporto oppure più rapporti da un elenco di rapporti.

## Modi per condividere i rapporti

Puoi condividere i rapporti in Workfront nel modo seguente:

* Manualmente, come descritto nella sezione [Condividi un report](#share-a-report) di seguito.
* Automaticamente, ereditando le autorizzazioni di visualizzazione da un dashboard contenente il report condiviso. Per informazioni sulla visualizzazione delle autorizzazioni ereditate sugli oggetti, vedere [Visualizzare le autorizzazioni ereditate sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Condividere un rapporto {#share-a-report}

La condivisione di uno o più report da un elenco è identica.

1. Vai a un elenco di report e seleziona uno o più report, quindi fai clic su **Condividi**.

   Oppure

   Fai clic sul nome di un report, quindi fai clic su **Azioni report >****Condivisione**.

   ![](assets/unshimmed-report-actions-sharing.png)

1. Nella casella visualizzata, nel campo **Aggiungi persone, team, ruoli, gruppi o aziende ...** inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui vuoi condividere il report, quindi premi **Invio** quando viene visualizzato il nome.

1. Per regolare il livello di accesso per un nome aggiunto, fai clic sul menu a discesa a destra del nome, quindi scegli una delle opzioni di seguito.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzare</td> 
      <td> <p>Consente al destinatario di accedere per visualizzare il report nell'area <strong>Report</strong> ed eseguirlo.</p> <p>È possibile fare clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera che l'utente o gli utenti possano <strong>condividerlo</strong> con chiunque nel sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestire</td> 
      <td> <p>Consente al destinatario l’accesso in modifica completa al rapporto.</p> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> per specificare se desideri che l'utente o gli utenti possano <strong>eliminare</strong> il report dal sistema e <strong>condividerlo</strong> con chiunque nel sistema.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i 2 passaggi precedenti per aggiungere altri nomi all’elenco e configurarne le opzioni.
1. (Facoltativo) Fai clic sul menu a discesa **Solo le persone invitate possono accedere** nella casella di condivisione, quindi scegli tra le seguenti opzioni:

   * **Solo gli utenti invitati possono accedere** Selezionare questa opzione in modo che solo gli utenti a cui è stato concesso l&#39;accesso al report possano visualizzarlo.

   * **Tutti gli utenti del sistema possono visualizzare** Selezionare questa opzione per consentire a tutti gli utenti di Workfront con accesso ai report di visualizzare il report.

1. (Facoltativo) Fai clic sull&#39;icona **Ingranaggio** ![Impostazioni icona ingranaggio](assets/gear-icon-settings-with-dn-arrow.jpg) nell&#39;angolo superiore destro della casella di condivisione, quindi, facoltativamente, seleziona la seguente opzione:

   * **Rendi pubblico agli utenti esterni** Seleziona questa opzione per generare un URL che possa essere condiviso con altri utenti. Chiunque abbia l’URL può accedere al rapporto senza disporre di una licenza Adobe Workfront.

     >[!CAUTION]
     >
     >Si consiglia di usare cautela quando si condivide con utenti esterni un oggetto contenente informazioni riservate. Questo consente loro di visualizzare le informazioni senza essere utenti di Workfront o parte dell’organizzazione.

     >[!NOTE]
     >
     >Se il report include una richiesta e viene condiviso pubblicamente, gli utenti che eseguono il report tramite il collegamento di condivisione pubblico non potranno eseguire il report utilizzando la richiesta. Il report verrà visualizzato senza che sia stato applicato il prompt, a meno che non accedano a Workfront e non accedano al report senza utilizzare il collegamento di condivisione pubblica. Per ulteriori informazioni sulle limitazioni della condivisione di report con i prompt, vedere la sezione [Limitazioni della condivisione dei report richiesti](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) nell&#39;articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Fai clic su **Salva**.
