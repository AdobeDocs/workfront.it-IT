---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visualizzare e gestire gli elementi eliminati di recente da un gruppo
description: Quando si visualizza un gruppo gestito nell'area Gruppi, è possibile visualizzare, filtrare, ripristinare ed esportare gli elementi di lavoro, i documenti e i modelli eliminati di recente.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 1%

---

# Visualizzare e gestire gli elementi eliminati di recente da un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con i progetti, le attività, i problemi, i documenti e i modelli eliminati di recente nei seguenti modi:

* Visualizzare, filtrare e raggruppare un elenco degli elementi eliminati di recente
* Ripristina gli elementi eliminati di recente selezionati
* Esporta un elenco di elementi eliminati di recente

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per ulteriori informazioni sugli elementi eliminati, vedere [Gestire gli elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gli elementi eliminati devono essere associati al gruppo o a uno qualsiasi dei suoi sottogruppi. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare e gestire gli elementi eliminati di recente da un gruppo

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo.
1. Nel pannello a sinistra, fai clic su **Eliminato di recente**.
1. Aprire una delle seguenti schede in cui si desidera visualizzare e gestire gli elementi eliminati di recente dal gruppo:

   * Progetti
   * Attività
   * Problemi
   * Documenti
   * Modelli

   Ogni scheda elenca gli elementi del tipo di oggetto corrispondente che appartengono al gruppo corrente o ai relativi sottogruppi e che sono stati eliminati negli ultimi 30 giorni.

   >[!NOTE]
   >
   >Se qualcuno ha eliminato un progetto, tutte le sue singole attività, problemi e documenti sono stati eliminati insieme ad esso. Questi non vengono visualizzati singolarmente nelle schede Attività, Problemi, Documenti o Modelli. Tuttavia, il ripristino del progetto ripristina anche tutti questi oggetti secondari nel progetto.
   >
   >
   >Se qualcuno ha eliminato un&#39;attività, un problema, un documento o un modello singolarmente, puoi visualizzarlo e gestirlo nella scheda appropriata.

1. Effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Ripristina oggetti</p> </td> 
      <td> <p>Seleziona fino a 10 oggetti, quindi fai clic su <strong>Ripristina</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Esporta l'intero elenco di oggetti nella scheda</p> </td> 
      <td> <p>Fai clic su <strong>Esporta</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Modificare la visualizzazione delle informazioni nell'elenco</p> </td> 
      <td> <p>Nell'angolo superiore destro sopra l'elenco, utilizza <strong>Filtro</strong> per definire ciò che viene visualizzato in base ai criteri specificati. Utilizza <strong>Visualizza</strong> per definire quali campi vengono visualizzati come colonne. Usa <strong>Raggruppamento</strong> per raggruppare gli elementi in categorie.</p> </td> 
     </tr> 
    </tbody> 
   </table>
