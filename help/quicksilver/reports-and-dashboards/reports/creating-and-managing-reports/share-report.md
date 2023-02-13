---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Condivisione di un rapporto in Adobe Workfront
description: L’amministratore Adobe Workfront consente agli utenti di visualizzare o modificare i rapporti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell’accesso ai problemi, consulta Concedere l’accesso a rapporti, dashboard e calendari.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Condivisione di un rapporto in Adobe Workfront

L’amministratore Adobe Workfront consente agli utenti di visualizzare o modificare i rapporti quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell’accesso ai problemi, consulta [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Oltre al livello di accesso concesso agli utenti, puoi anche concedere loro le autorizzazioni per visualizzare o gestire rapporti specifici a cui hai accesso per la condivisione. Per ulteriori informazioni sui livelli di accesso e le autorizzazioni, consulta [Funzionamento congiunto dei livelli di accesso e delle autorizzazioni](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

>[!NOTE]
>
>Un amministratore Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

## Requisiti di accesso

Per condividere gli oggetti è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza l'accesso o una versione successiva a Report, Dashboard, Calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o superiore del rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulla condivisione dei rapporti

Oltre alle considerazioni seguenti, vedi [Condividere rapporti, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Puoi condividere i rapporti creati con altri utenti, team, gruppi, ruoli o aziende. Puoi anche condividere rapporti creati da altri utenti e condivisi con te.
* Puoi anche condividerli con l’intera organizzazione o renderli pubblici. Quando si rende pubblico un rapporto, viene generato un URL che può essere condiviso con altri utenti.
* È possibile condividere un singolo rapporto oppure più rapporti da un elenco.

## Modi per condividere i rapporti

Puoi condividere i rapporti in Workfront nel modo seguente:

* Manualmente, come descritto nel [Condividere un rapporto](#share-a-report) di seguito.
* In modo automatico, ereditando le autorizzazioni di visualizzazione da un dashboard contenente il report condiviso. Per informazioni sulla visualizzazione delle autorizzazioni ereditate sugli oggetti, vedere [Visualizzare le autorizzazioni ereditate sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Condividere un rapporto {#share-a-report}

La condivisione di uno o più rapporti da un elenco è identica.

1. Passa a un elenco di rapporti e seleziona uno o più rapporti, quindi fai clic su **Condividi**.

   Oppure

   Fai clic sul nome di un rapporto, quindi fai clic su **Azioni rapporto >****Condivisione**.

   ![](assets/qs-report-actions-sharing.png)

1. Nella casella visualizzata, nella **Aggiungi persone, team, ruoli, gruppi o aziende ...** inizia a digitare il nome dell&#39;utente, del team, del ruolo del lavoro, del gruppo o della società con cui desideri condividere il rapporto, quindi premi **Invio** quando viene visualizzato il nome.

1. Per regolare il livello di accesso per un nome aggiunto, fai clic sul menu a discesa a destra del nome, quindi scegli una delle opzioni seguenti.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzare</td> 
      <td> <p>Consente al destinatario di accedere per visualizzare il rapporto nel <strong>Rapporti</strong> <img src="assets/reports-in-main-menu.png"> e lo esegua.</p> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> per specificare se l'utente o gli utenti devono essere in grado di <strong>Condividi</strong> con chiunque nel sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestire</td> 
      <td> <p>Consente al destinatario di accedere in modalità di modifica completa al rapporto.</p> <p>Puoi fare clic su <strong>Impostazioni avanzate</strong> per specificare se l'utente o gli utenti devono essere in grado di <strong>Elimina</strong> la relazione del sistema e <strong>Condividi</strong> con chiunque nel sistema.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i 2 passaggi precedenti per aggiungere altri nomi all’elenco e configurare le relative opzioni.
1. (Facoltativo) Fai clic sul pulsante **Ingranaggio** icona ![](assets/gear-icon-settings-with-dn-arrow.jpg) nell&#39;angolo in alto a destra della casella di condivisione, quindi seleziona una delle seguenti opzioni:

   * **Rendi questo pubblico a utenti esterni:** Seleziona questa opzione per generare un URL che possa essere condiviso con altri utenti. Chiunque disponga dell’URL può accedere al rapporto senza disporre di una licenza Adobe Workfront.

      >[!CAUTION]
      >
      >È consigliabile prestare attenzione quando si condivide con utenti esterni un oggetto contenente informazioni confidenziali. Questo consente loro di visualizzare le informazioni senza essere un utente Workfront o parte dell’organizzazione.

      >[!NOTE]
      >
      >Se il report ha un prompt e lo condividi pubblicamente, gli utenti che eseguono il report devono essere connessi a Workfront per poter eseguire il report utilizzando il prompt. Se non possono accedere a Workfront, visualizzeranno il rapporto senza il prompt ad esso applicato. Per ulteriori informazioni sulle limitazioni della condivisione di rapporti con prompt, consulta la sezione . [Limitazioni della condivisione dei rapporti richiesti](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) nell&#39;articolo [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Rendere visibile il sistema a livello di sistema:** Seleziona questa opzione in modo che tutti gli utenti di Workfront con accesso ai rapporti possano visualizzare il rapporto.

1. Fai clic su **Salva**.
