---
title: Elimina utenti
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Quando un utente lascia l’organizzazione, può rimuoverlo da Workfront; tuttavia, si consiglia di disattivarlo invece di eliminarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Elimina utenti

Quando un utente lascia l’organizzazione, puoi rimuoverlo da Adobe Workfront.

>[!IMPORTANT]
>
>* L&#39;eliminazione di un utente dal sistema comporta anche l&#39;eliminazione delle informazioni associate all&#39;utente che si desidera conservare. È consigliabile disattivare gli utenti invece di eliminarli. Per ulteriori informazioni, consulta [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding nell’Admin Console. Se la tua organizzazione è stata integrata in Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Eliminazione di un utente da [!DNL Adobe Admin Console] disattiva l&#39;utente in [!DNL Workfront], ma non li elimina da [!DNL Workfront].
>
>  Per istruzioni sull’eliminazione di un utente nel Adobe Admin Console, consulta la sezione &quot;Eliminare definitivamente gli utenti&quot; nell’articolo [Gestire gli utenti singolarmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) o contatta l&#39;amministratore di Adobe Admin Console.
>
>  Per un elenco delle procedure che differiscono in base al fatto che la tua organizzazione sia stata onboarding in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>

## Requisiti di accesso

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
     <li> <p>Livello di accesso Amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato su <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utenti</b> opzioni abilitate in <b>Metti a punto le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti gruppo)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> <p>Per ulteriori informazioni su <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminazione e disattivazione di un utente

La disattivazione di un utente causa i seguenti eventi:

* Rimuove le licenze dell’utente sia per Workfront che per Workfront Proof se il componente Workfront Proof è associato al tuo account Workfront. Per ulteriori informazioni su Workfront Proof, consulta [Workfront Proof: indice articolo](../../../workfront-proof/workfront-proof.md).
* L&#39;utente non può più essere assegnato al lavoro.
* L’utente non può più essere aggiunto agli aggiornamenti.
* L’utente non può più essere aggiunto a team o gruppi.
* Gli oggetti non possono più essere condivisi con l&#39;utente.
* L’associazione con i seguenti oggetti rimane intatta:

   * Attività, problemi, progetti, portfolio
   * Dashboard

     >[!NOTE]
     >
     >Se disattivi un utente e non riesci più a visualizzare i rapporti o le dashboard associati a un utente, potrebbe essere necessario aggiornare **Esegui questo report con i diritti di accesso di:** campo.\
     >Per ulteriori informazioni, consulta [Perché non posso accedere a un report di proprietà di un utente disattivato?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) sezione del [Domande frequenti sui rapporti](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) articolo.

   * Documenti
   * Aggiornamenti
   * Ore

* Se l&#39;utente ha estratto i documenti, questi rimarranno estratti anche dopo la loro disattivazione. Solo un amministratore di Workfront può archiviarli di nuovo. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrai documenti](../../../documents/managing-documents/check-out-documents.md).

L’eliminazione di un utente determina le seguenti situazioni:

* Rimuove le licenze dell’utente sia per Workfront che per Workfront Proof, se il componente Workfront Proof è associato al tuo account Workfront. Per ulteriori informazioni su Workfront Proof, consulta [Workfront Proof: indice articolo](../../../workfront-proof/workfront-proof.md).
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
     >Per ulteriori informazioni, consulta [Come posso accedere a una dashboard contenente un report di proprietà di un utente eliminato?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) sezione del [Domande frequenti sui rapporti](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) articolo.

   * Aggiornamenti
   * Ore

     >[!NOTE]
     >
     >Questi oggetti rimangono in Workfront ma il proprietario dell&#39;oggetto è ora vuoto.

* Se l’utente ha caricato dei documenti nell’area Documenti della barra di navigazione globale, anche i documenti vengono eliminati.
* Se l&#39;utente ha estratto i documenti di sua proprietà e i documenti vengono caricati nell&#39;area Documenti principale (accessibile dal menu principale), i documenti vengono eliminati insieme all&#39;utente. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrai documenti](../../../documents/managing-documents/check-out-documents.md).

Per ulteriori informazioni sulla disattivazione degli utenti, consulta [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

È possibile eliminare gli utenti in modo permanente uno alla volta oppure eliminare più utenti contemporaneamente in modo permanente. Quando elimini singoli utenti, devi attendere il completamento del processo di eliminazione prima di passare ad altre attività in Workfront. Il processo di eliminazione di più utenti viene eseguito contemporaneamente come processo in background, in modo da poter continuare a utilizzare Workfront man mano che gli utenti vengono eliminati.

## Elimina uno o più utenti

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront.

1. Clic **Utenti**.
1. Selezionare almeno un utente da eliminare, quindi scegliere il menu Altro ![](assets/more-icon.png), quindi fai clic su **Elimina**.
1. Nella casella visualizzata fare clic su **Elimina** per confermare l’eliminazione.

   Il processo di eliminazione degli utenti viene eseguito come processo in background, quindi puoi continuare a utilizzare Workfront quando uno o più utenti vengono eliminati.

   A seconda del numero di utenti che si sta eliminando, il processo può richiedere alcuni minuti o anche alcune ore.

   Dopo aver ricevuto in Workfront la conferma che gli utenti sono stati eliminati, puoi continuare a visualizzarli nel sistema fino a quando il processo di eliminazione non viene completato in background.

   In un secondo momento, se scopri che uno o più utenti non sono stati eliminati correttamente, prova a eliminarli uno alla volta.
