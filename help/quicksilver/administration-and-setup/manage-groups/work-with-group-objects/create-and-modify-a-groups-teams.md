---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare i team di un gruppo
description: Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo e a qualsiasi suo sottogruppo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 4%

---

# Creare e modificare i team di un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo e a qualsiasi suo sottogruppo.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per informazioni su come gli utenti con una licenza Pianificazione possono creare un team, vedere [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Per informazioni su come un amministratore di Workfront può creare un team, vedere [Creare un team dall&#39;area Configurazione](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

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
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza, utilizza e crea team per il tuo gruppo dall’area Gruppi

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera creare o modificare i team.
1. Nel pannello a sinistra, fai clic su **Team** ![Team](assets/teams.png) per elencare i team associati al gruppo e ai suoi eventuali sottogruppi.

1. Effettua una delle seguenti operazioni:

   * **Aggiungi un team**: fai clic su **Nuovo team**, quindi utilizza le seguenti opzioni per configurarlo:

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
       <td> <p> Nel campo Gruppo del nuovo team viene inserito automaticamente il gruppo visualizzato. Se si desidera associare il team a un gruppo diverso, iniziare a digitare il nome del gruppo, quindi selezionarlo quando viene visualizzato.</p> <p>Per assicurarsi di associare il gruppo corretto al team, passare il puntatore del mouse su di esso e fare clic sull'icona delle informazioni <img src="assets/info-icon.png"> visualizzata accanto al gruppo. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p><b>NOTA</b>: quando un team viene assegnato a un gruppo o a un sottogruppo, qualsiasi amministratore di gruppo di tale gruppo o sottogruppo può gestire il team senza esserne membro. Gli amministratori dei gruppi possono accedere all'area Team dal menu principale e fare clic sulla freccia Switch Teams <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi che gestiscono.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membri del team</td> 
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

   * **Modifica team**: seleziona almeno un team, fai clic su **the** Modifica icona ![Modifica icona](assets/edit-icon.png), quindi utilizza le seguenti opzioni per configurarlo:

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
       <td> <p>Associa il team a un gruppo. Iniziate a digitare il nome del gruppo, quindi selezionate il nome quando viene visualizzato.</p> <p>Per assicurarsi di associare il gruppo corretto al team, passare il puntatore del mouse su di esso e fare clic sull'icona delle informazioni <img src="assets/info-icon.png"> visualizzata accanto al gruppo. In questo modo viene visualizzata una descrizione del gruppo contenente informazioni sul gruppo stesso, ad esempio la gerarchia dei gruppi al di sopra del gruppo e i relativi amministratori.</p> <p><b>NOTA</b>: quando un team viene assegnato a un gruppo o a un sottogruppo, qualsiasi amministratore di gruppo di tale gruppo o sottogruppo può gestire il team senza esserne membro. Gli amministratori dei gruppi possono accedere all'area Team dal menu principale e fare clic sulla freccia Switch Teams <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi che gestiscono.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Proprietario</td> 
       <td>Selezionare un proprietario per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membri del team</td> 
       <td> <p>Aggiungi membri del gruppo e. Inizia a digitare il nome di un utente, quindi selezionalo quando viene visualizzato. Ripetere questo processo per aggiungere più utenti al team.</p> <p><b>SUGGERIMENTO</b>: non esiste alcun limite al numero di utenti che è possibile aggiungere a un team. Tuttavia, si consiglia di non avere un numero eccessivo di utenti in un unico team, perché la gestione del lavoro del team potrebbe diventare troppo complessa.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descrizione</td> 
       <td>Digitare una descrizione per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Modello layout</td> 
       <td> <p>Iniziare a digitare il nome del modello di layout che si desidera venga utilizzato dal team, quindi fare clic su di esso quando viene visualizzato.</p> <p>Quando si designa il team con questo modello di layout come team predefinito di utenti, tutti gli utenti di questo team visualizzeranno le personalizzazioni nel modello di layout.<br>Le singole impostazioni del modello di layout sovrascriveranno quelle del modello di layout del team principale. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Specifica se si tratta di un team Agile. Per informazioni sui team Agile e su come gestirne il lavoro, consulta <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team Agile</a>.</td> 
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

   * **Elimina team**: seleziona almeno un team, quindi fai clic sull&#39;icona Elimina ![icona Elimina](assets/delete.png).
   * **Esporta l&#39;elenco dei team**: fare clic su **Esporta** ![Icona Esporta](assets/export.png), quindi selezionare il formato di file desiderato per l&#39;elenco esportato.
