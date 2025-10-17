---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visualizzare e gestire gli elementi eliminati di recente di un gruppo
description: Quando si visualizza un gruppo gestito nell'area Gruppi, è possibile visualizzare, filtrare, ripristinare ed esportare gli elementi di lavoro, i documenti e i modelli eliminati di recente.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '414'
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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr>
   <td>Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
  <tr> 
   <td>Autorizzazioni oggetto</td>
   <td>Gli elementi eliminati devono essere associati al gruppo o a uno qualsiasi dei suoi sottogruppi.</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e gestire gli elementi eliminati di recente da un gruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

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

1. Completa una delle azioni seguenti:

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
