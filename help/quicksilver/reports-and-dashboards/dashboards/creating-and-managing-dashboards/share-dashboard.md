---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Condividere un dashboard
description: L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare le dashboard quando assegnano i livelli di accesso. Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare o gestire dashboard specifiche a cui si ha accesso per la condivisione.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Condividere un dashboard

<!-- Audited: 1/2025 -->

L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare le dashboard quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell&#39;accesso ai problemi, vedere [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare o gestire dashboard specifiche a cui si ha accesso per la condivisione. Per ulteriori informazioni sui livelli di accesso e sulle autorizzazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
    <td> 
   <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a report, dashboard, calendari</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per il dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare il dashboard prima di poterlo condividere.

Per informazioni sulla creazione di dashboard, vedere [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Considerazioni sulla condivisione delle dashboard

Oltre alle considerazioni seguenti, vedere anche [Condividere report, dashboard e calendari](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Per impostazione predefinita, l’autore di un dashboard dispone delle autorizzazioni di gestione per tale dashboard.

* Puoi condividere dashboard che hai creato con altri singoli utenti, team, gruppi, mansioni o aziende. Puoi anche condividere dashboard creati da altri utenti e che sono stati condivisi con te.
* Puoi anche condividerli con l’intera organizzazione rendendoli visibili a livello di sistema.
* È possibile condividere un singolo dashboard oppure più dashboard da un elenco.
* Quando si condivide un dashboard, per impostazione predefinita gli utenti ereditano le autorizzazioni di visualizzazione da tutti gli oggetti report nel dashboard.

  Per ulteriori informazioni sulla gerarchia degli oggetti in Workfront, vedere [Informazioni sugli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Per informazioni sulla visualizzazione delle autorizzazioni ereditate, vedere [Visualizzare le autorizzazioni ereditate sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Condividere un dashboard

La condivisione di uno o più dashboard da un elenco è identica.

1. Vai a un elenco di dashboard e seleziona uno o più dashboard, quindi fai clic su **Condividi** ![](assets/share-icon.png).

   Oppure

   Fai clic sul nome di un dashboard, quindi fai clic su **Azioni dashboard** > **Condivisione**.

   ![](assets/unshimmed-share-dashboard.png)

1. Nel campo **Aggiungi persone, team, ruoli, gruppi o società**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui vuoi condividere il dashboard, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.
1. (Facoltativo) Per rendere il dashboard accessibile a tutti gli utenti del sistema, fai clic sul menu a discesa **Solo gli invitati possono accedere** nella finestra di dialogo di condivisione, quindi seleziona **Tutti nel sistema possono visualizzare**.

1. Fai clic su **Salva**.
