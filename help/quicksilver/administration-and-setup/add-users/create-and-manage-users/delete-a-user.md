---
title: Eliminare gli utenti
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Quando un utente lascia l'organizzazione, può rimuovere l'utente da Workfront, anche se si consiglia di disattivare gli utenti invece di eliminarli.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Eliminare gli utenti

Quando un utente lascia l’organizzazione, puoi rimuovere quell’utente da Adobe Workfront.

>[!IMPORTANT]
>
>* Se si elimina un utente dal sistema, vengono anche eliminate le informazioni associate all&#39;utente che si desidera mantenere. È consigliabile disattivare gli utenti invece di eliminarli. Per ulteriori informazioni, consulta [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Eliminazione di un utente dal [!DNL Adobe Admin Console] disattiva l&#39;utente in [!DNL Workfront], ma non eliminarli [!DNL Workfront].
>
>  Per istruzioni sull’eliminazione di un utente in Adobe Admin Console, consulta la sezione &quot;Eliminare definitivamente gli utenti&quot; nell’articolo [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oppure contatta l’amministratore Adobe Admin Console.
>
>  Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminazione o disattivazione di un utente

La disattivazione di un utente causa il seguente verificarsi:

* Rimuove le licenze dell’utente sia da Workfront che da Workfront Proof se il componente Workfront Proof è associato al tuo account Workfront. Per ulteriori informazioni sulla bozza di Workfront, consulta [Prova Workfront](../../../workfront-proof/workfront-proof.md).
* Non è più possibile assegnare il lavoro all’utente.
* L’utente non può più essere aggiunto agli aggiornamenti.
* L’utente non può più essere aggiunto ai team o ai gruppi.
* Gli oggetti non possono più essere condivisi con l&#39;utente.
* La loro associazione con i seguenti oggetti rimane intatta:

   * Compiti, problemi, progetti, portfolio
   * Dashboard

      >[!NOTE]
      >
      >Se disattivi un utente e non riesci più a visualizzare i rapporti o le dashboard associate a un utente, potrebbe essere necessario aggiornare il **Esegui questo rapporto con i diritti di accesso di:** campo .\
      >Per ulteriori informazioni, consulta la sezione [Perché non posso accedere a un report di proprietà di un utente disattivato?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) della sezione [Domande frequenti sui rapporti](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) articolo.

   * Documenti
   * Aggiornamenti
   * Ore

* Se l’utente ha estratto dei documenti, questi rimangono estratti quando vengono disattivati. Solo un amministratore Workfront può effettuare nuovamente il check-in. Per ulteriori informazioni sull&#39;estrazione dei documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

Se si elimina un utente, si verifica quanto segue:

* Rimuove le licenze dell’utente sia da Workfront che da Workfront Proof, se il componente Workfront Proof è associato al tuo account Workfront. Per ulteriori informazioni sulla bozza di Workfront, consulta [Prova Workfront](../../../workfront-proof/workfront-proof.md).
* Non è più possibile assegnare il lavoro all’utente.
* L’utente non può più essere aggiunto agli aggiornamenti.
* L’utente non può più essere aggiunto ai team o ai gruppi.
* Gli oggetti non possono più essere condivisi con l&#39;utente.
* Elimina l’associazione di tale utente agli oggetti seguenti:

   * Compiti, problemi, progetti, portfolio
   * Dashboard

      >[!NOTE]
      >
      >Perdi anche l’accesso alle sezioni personalizzate contenenti dashboard associate all’utente eliminato.\
      >Per ulteriori informazioni, consulta la sezione [Come posso accedere a un dashboard contenente un report di proprietà di un utente eliminato?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) della sezione [Domande frequenti sui rapporti](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) articolo.

   * Aggiornamenti
   * Ore

      >[!NOTE]
      >
      >Questi oggetti rimangono in Workfront ma il proprietario dell’oggetto è ora vuoto.

* Se l&#39;utente ha caricato dei documenti nell&#39;area Documenti della barra di navigazione globale, anche i documenti vengono eliminati.
* Se l&#39;utente ha estratto i documenti di cui dispone e i documenti sono caricati nell&#39;area Documenti principale (a cui si accede dal menu principale), i documenti vengono eliminati insieme all&#39;utente. Per ulteriori informazioni sull&#39;estrazione dei documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

Per ulteriori informazioni sulla disattivazione degli utenti, consulta [Disattivare o riattivare un utente](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

È possibile eliminare definitivamente gli utenti uno alla volta oppure eliminare definitivamente più utenti contemporaneamente. Quando elimini singoli utenti, devi attendere il completamento del processo di eliminazione prima di passare ad altre attività in Workfront. Il processo di eliminazione di più utenti contemporaneamente viene eseguito come processo in background, per cui puoi continuare a utilizzare Workfront durante l’eliminazione degli utenti.

## Elimina uno o più utenti

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Utenti**.
1. Selezionare almeno un utente da eliminare, fare clic sul menu Altro ![](assets/more-icon.png), quindi fai clic su **Elimina**.
1. Nella casella visualizzata, fai clic su **Elimina** per confermare l’eliminazione.

   Il processo di eliminazione degli utenti viene eseguito come processo in background, per cui puoi continuare a utilizzare Workfront quando gli utenti o gli utenti vengono eliminati.

   A seconda del numero di utenti che si stanno eliminando, il processo può richiedere alcuni minuti o anche qualche ora.

   Dopo aver ricevuto in Workfront la conferma che gli utenti sono stati eliminati, potresti continuare a vederli nel sistema fino a quando il processo di eliminazione non è completo in background.

   In un secondo momento, se scopri che uno o più utenti non sono stati eliminati correttamente, prova a eliminarli uno alla volta.
