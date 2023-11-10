---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare i team di un gruppo
description: Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo e a qualsiasi suo sottogruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# Creare e modificare i team di un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo e a qualsiasi suo sottogruppo.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per informazioni su come gli utenti con una licenza Pianificazione possono creare un team, consulta [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Per informazioni su come un amministratore di Workfront può creare un team, consulta [Creare un team dall’area Configurazione](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza disponibile, contattare l&#39;amministratore di Workfront.

## Visualizza, utilizza e crea team per il tuo gruppo dall’area Gruppi

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera creare o modificare i team.
1. Nel pannello a sinistra, fai clic su **Team** ![](assets/teams.png) per elencare i team associati al gruppo e a eventuali sottogruppi.

1. Effettua una delle seguenti operazioni:

   * **Aggiungi un team**: fai clic **Nuovo team**, quindi utilizza le seguenti opzioni per configurarlo:

   <!-- WRITER please check table below. I stripped out wonky conditions-->

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
       <td> <p> Nel campo Gruppo del nuovo team viene inserito automaticamente il gruppo visualizzato. Se si desidera associare il team a un gruppo diverso, iniziare a digitare il nome del gruppo, quindi selezionarlo quando viene visualizzato.</p> <p>Per assicurarsi di associare il gruppo corretto al team, posizionare il puntatore del mouse su di esso e fare clic sull'icona delle informazioni <img src="assets/info-icon.png"> che viene visualizzato accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p><b>NOTA</b>: quando un team viene assegnato a un gruppo o a un sottogruppo, qualsiasi amministratore di gruppo di tale gruppo o sottogruppo può gestire il team senza esserne membro. Gli amministratori dei gruppi possono passare all’area Team dal menu principale e fare clic sulla freccia Switch Teams (Cambia team). <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi che gestiscono.</p> </td> 
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

   * **Modifica team**: seleziona almeno un team, fai clic su **il** Icona Modifica ![](assets/edit-icon.png), quindi utilizza le seguenti opzioni per configurarlo:

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
       <td> <p>Associa il team a un gruppo. Iniziate a digitare il nome del gruppo, quindi selezionate il nome quando viene visualizzato.</p> <p>Per assicurarsi di associare il gruppo corretto al team, posizionare il puntatore del mouse su di esso e fare clic sull'icona delle informazioni <img src="assets/info-icon.png"> che viene visualizzato accanto ad esso. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p><b>NOTA</b>: quando un team viene assegnato a un gruppo o a un sottogruppo, qualsiasi amministratore di gruppo di tale gruppo o sottogruppo può gestire il team senza esserne membro. Gli amministratori dei gruppi possono passare all’area Team dal menu principale e fare clic sulla freccia Switch Teams (Cambia team). <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi che gestiscono.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Proprietario</td> 
       <td>Selezionare un proprietario per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membri team</td> 
       <td> <p>Aggiungi membri del gruppo e. Inizia a digitare il nome di un utente, quindi selezionalo quando viene visualizzato. Ripetere questo processo per aggiungere più utenti al team.</p> <p><b>SUGGERIMENTO</b>: non esiste alcun limite al numero di utenti che è possibile aggiungere a un team. Tuttavia, si consiglia di non avere un numero eccessivo di utenti in un unico team, perché la gestione del lavoro del team potrebbe diventare troppo complessa.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descrizione</td> 
       <td>Digitare una descrizione per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Modello di layout</td> 
       <td> <p>Iniziare a digitare il nome del modello di layout che si desidera venga utilizzato dal team, quindi fare clic su di esso quando viene visualizzato.</p> <p>Quando si designa il team con questo modello di layout come team predefinito di utenti, tutti gli utenti di questo team visualizzeranno le personalizzazioni nel modello di layout.<br>Le singole impostazioni del modello di layout sostituiranno quelle del modello di layout team principale. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Specifica se si tratta di un team Agile. Per informazioni sui team Agile e su come gestirne il lavoro, consulta <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team agile</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Lavoraci</td> 
       <td> <p>Cambiare il pulsante Lavoraci in un pulsante Start. Quando un utente fa clic su Start, lo stato dell’elemento viene aggiornato automaticamente.</p> <p>Per ulteriori informazioni su come configurare il pulsante Start, vedere <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Lavoraci con un pulsante Start</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Pulsante "Fine"</td> 
       <td> <p>Personalizzare il pulsante Fine. Per ulteriori informazioni, consulta:</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configura il pulsante Fine per le attività</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configura il pulsante Fine per i problemi</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Elimina team**: seleziona almeno un team, quindi fai clic sull’icona Elimina ![](assets/delete.png).
   * **Esporta l’elenco dei team**: fai clic **Esporta** ![](assets/export.png), quindi selezionare il formato di file desiderato per l&#39;elenco esportato.
