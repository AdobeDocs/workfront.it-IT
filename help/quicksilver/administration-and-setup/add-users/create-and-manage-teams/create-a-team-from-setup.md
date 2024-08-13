---
title: Creare un team dall’area di configurazione
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: In qualità di amministratore di Adobe Workfront, puoi creare un team dall’area Configurazione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 4%

---

# Creare un team dall’area Configurazione

In qualità di amministratore di Adobe Workfront, puoi creare un team dall’area Configurazione. Per informazioni sui team, consulta [Panoramica sui team](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un amministratore gruppo può creare un team per un gruppo che amministra dall’area Configurazione. Per ulteriori informazioni, vedere [Creare e modificare i team di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utente con una licenza Pianificazione può anche creare un team dall’area Persone. Per ulteriori informazioni, vedere [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Creare un team

{{step-1-to-setup}}

1. Fai clic su **Team**, quindi su **Nuovo team**.

1. Nella casella **Nuovo team** visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome team</td> 
      <td>Digitare un nome per il team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppo</td> 
      <td> <p>Se si desidera associare il team a un gruppo, iniziare a digitare il nome del gruppo, quindi selezionarlo quando viene visualizzato.</p> <p>Per assicurarsi di associare il gruppo corretto al team, passare il puntatore del mouse su di esso e fare clic sull'icona delle informazioni <img src="assets/info-icon.png"> visualizzata accanto al gruppo. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p><b>NOTA</b>: quando un team viene assegnato a un gruppo o a un sottogruppo, qualsiasi amministratore di gruppo di tale gruppo o sottogruppo può gestire il team senza esserne membro. Gli amministratori dei gruppi possono accedere all'area Team dal menu principale e fare clic sulla freccia Switch Teams <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi che gestiscono.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri team</td> 
      <td> <p>Inizia a digitare il nome di un utente che farà parte del team, quindi seleziona il nome quando appare nell’elenco a discesa. Ripetere questo processo per aggiungere più utenti al team.</p> <p>Non esiste alcun limite al numero di utenti che è possibile aggiungere a un team. Tuttavia, si consiglia di non avere un numero eccessivo di utenti in un unico team, perché la gestione del lavoro del team potrebbe diventare troppo complessa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digitare una descrizione per il team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calendario</td> 
      <td>Scegliere la scheda del calendario visualizzata per questo team.</td> 
     </tr> 
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Questo è un team agile</td> 
      <td>Selezionare questo elemento se si desidera configurare il nuovo team come un team agile. Per ulteriori informazioni sui team Agile, vedi <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team Agile</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lavoraci</td> 
      <td>Cambiare il pulsante Lavoraci in un pulsante Start. Quando un utente fa clic su Start, lo stato dell’elemento viene aggiornato automaticamente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pulsante "Fine"</td> 
      <td>Selezionare lo stato che si desidera impostare per gli elementi quando si fa clic sul pulsante Fine.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fare clic su **Crea team**.

## Proprietari team

Per impostazione predefinita, quando si crea un team, si diventa il proprietario del team.

È possibile visualizzare i proprietari di tutti i team quando si crea un rapporto per i team e si include il campo Nome proprietario nel rapporto. Per ulteriori informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
