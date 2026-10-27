---
title: Cancella Utenti
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Quando un utente lascia l’organizzazione, può rimuoverlo da Workfront; tuttavia, si consiglia di disattivarlo invece di eliminarlo.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 9%
---
# Eliminare gli utenti

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applicava solo alle organizzazioni che non erano state caricate in Admin Console. Poiché la tua organizzazione è stata integrata in Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>  Per istruzioni sull&#39;eliminazione di un utente in Adobe Admin Console, vedere la sezione &quot;Eliminazione definitiva degli utenti&quot; nell&#39;articolo [Gestione individuale degli utenti](https://helpx.adobe.com/it/enterprise/using/manage-users-individually.html) o contattare l&#39;amministratore di Adobe Admin Console.

Quando un utente lascia l’organizzazione, puoi rimuoverlo da Adobe Workfront.

L’eliminazione di un utente deve essere eseguita tramite Adobe Admin Console. Per istruzioni, vedere la sezione &quot;Eliminare definitivamente gli utenti&quot; nell&#39;articolo [Gestire gli utenti singolarmente](https://helpx.adobe.com/it/enterprise/using/manage-users-individually.html) o contattare l&#39;amministratore di Adobe Admin Console.

>[!IMPORTANT]
>
>L&#39;eliminazione di un utente dal sistema comporta anche l&#39;eliminazione delle informazioni associate all&#39;utente che si desidera conservare. È consigliabile disattivare gli utenti invece di eliminarli. Per ulteriori informazioni, vedere [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Adobe Admin Console.</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminazione e disattivazione di un utente

La disattivazione di un utente causa i seguenti eventi:

* Rimuove le licenze dell’utente sia per Workfront che per Workfront Proof se il componente Workfront Proof è associato al tuo account Workfront. Per ulteriori informazioni su Workfront Proof, vedere [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* L&#39;utente non può più essere assegnato al lavoro.
* L’utente non può più essere aggiunto agli aggiornamenti.
* L’utente non può più essere aggiunto a team o gruppi.
* Gli oggetti non possono più essere condivisi con l&#39;utente.
* L’associazione con i seguenti oggetti rimane intatta:

  * Attività, problemi, progetti, portfolio
  * Dashboard

    >[!NOTE]
    >
    >Se si disattiva un utente e non è più possibile visualizzare i report o le dashboard associati a un utente, potrebbe essere necessario aggiornare **Esegui il report con i diritti di accesso di:**.\
    >Per ulteriori informazioni, vedere [Perché non è possibile accedere a un report di proprietà di un utente disattivato?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) sezione dell&#39;articolo [Domande frequenti sui report](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

  * Documenti
  * Aggiornamenti
  * Ore

* Se l&#39;utente ha estratto i documenti, questi rimarranno estratti anche dopo la loro disattivazione. Solo un amministratore di Workfront può archiviarli di nuovo. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

L’eliminazione di un utente determina le seguenti situazioni:

* Rimuove le licenze dell’utente sia per Workfront che per Workfront Proof, se il componente Workfront Proof è associato al tuo account Workfront. Per ulteriori informazioni su Workfront Proof, vedere [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* L&#39;utente non può più essere assegnato al lavoro.
* L’utente non può più essere aggiunto agli aggiornamenti.
* L’utente non può più essere aggiunto a team o gruppi.
* Gli oggetti non possono più essere condivisi con l&#39;utente.
* Elimina l&#39;associazione dell&#39;utente agli oggetti seguenti:

  * Attività, problemi, progetti, portfolio
  * Dashboard

<!--

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

-->
* Aggiornamenti
* Ore

  >[!NOTE]
  >
  >Questi oggetti rimangono in Workfront ma il proprietario dell&#39;oggetto è ora vuoto.

* Se l’utente ha caricato dei documenti nell’area Documenti della barra di navigazione globale, anche i documenti vengono eliminati.
* Se l&#39;utente ha estratto i documenti di sua proprietà e i documenti vengono caricati nell&#39;area Documenti principale (accessibile dal menu principale), i documenti vengono eliminati insieme all&#39;utente. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

Per ulteriori informazioni sulla disattivazione degli utenti, vedere [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
