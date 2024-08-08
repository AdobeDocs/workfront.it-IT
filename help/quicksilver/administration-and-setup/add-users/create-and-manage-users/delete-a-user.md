---
title: Cancella Utenti
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Quando un utente lascia l’organizzazione, può rimuoverlo da Workfront; tuttavia, si consiglia di disattivarlo invece di eliminarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 1%

---

# Elimina utenti

Quando un utente lascia l’organizzazione, puoi rimuoverlo da Adobe Workfront.

>[!IMPORTANT]
>
>L&#39;eliminazione di un utente dal sistema comporta anche l&#39;eliminazione delle informazioni associate all&#39;utente che si desidera conservare. È consigliabile disattivare gli utenti invece di eliminarli. Per ulteriori informazioni, vedere [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. Per informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se l'utente <b>Amministratore (utenti gruppo)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> <p>Per ulteriori informazioni sull'impostazione <b>Utenti</b> in un livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

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

     >[!NOTE]
     >
     >Perdi inoltre l’accesso alle sezioni personalizzate contenenti dashboard associate all’utente eliminato.\
     >Per ulteriori informazioni, vedere [Come si accede a un dashboard contenente un report di proprietà di un utente eliminato?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) sezione dell&#39;articolo [Domande frequenti sui report](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Aggiornamenti
   * Ore

     >[!NOTE]
     >
     >Questi oggetti rimangono in Workfront ma il proprietario dell&#39;oggetto è ora vuoto.

* Se l’utente ha caricato dei documenti nell’area Documenti della barra di navigazione globale, anche i documenti vengono eliminati.
* Se l&#39;utente ha estratto i documenti di sua proprietà e i documenti vengono caricati nell&#39;area Documenti principale (accessibile dal menu principale), i documenti vengono eliminati insieme all&#39;utente. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

Per ulteriori informazioni sulla disattivazione degli utenti, vedere [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

È possibile eliminare gli utenti in modo permanente uno alla volta oppure eliminare più utenti contemporaneamente in modo permanente. Quando elimini singoli utenti, devi attendere il completamento del processo di eliminazione prima di passare ad altre attività in Workfront. Il processo di eliminazione di più utenti viene eseguito contemporaneamente come processo in background, in modo da poter continuare a utilizzare Workfront man mano che gli utenti vengono eliminati.

## Elimina uno o più utenti

{{step-1-to-users}}

1. Selezionare almeno un utente che si desidera eliminare, fare clic sul menu Altro ![](assets/more-icon.png) e quindi su **Elimina**.
1. Nella casella visualizzata, fare clic su **Elimina** per confermare l&#39;eliminazione.

   Il processo di eliminazione degli utenti viene eseguito come processo in background, quindi puoi continuare a utilizzare Workfront quando uno o più utenti vengono eliminati.

   A seconda del numero di utenti che si sta eliminando, il processo può richiedere alcuni minuti o anche alcune ore.

   Dopo aver ricevuto in Workfront la conferma che gli utenti sono stati eliminati, puoi continuare a visualizzarli nel sistema fino a quando il processo di eliminazione non viene completato in background.

   In un secondo momento, se scopri che uno o più utenti non sono stati eliminati correttamente, prova a eliminarli uno alla volta.
