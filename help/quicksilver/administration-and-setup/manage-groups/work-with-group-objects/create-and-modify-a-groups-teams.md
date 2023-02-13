---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare i team di un gruppo
description: Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo e con uno qualsiasi dei relativi sottogruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# Creare e modificare i team di un gruppo

Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo e con uno qualsiasi dei relativi sottogruppi.

Se ci sono gruppi al di sopra del gruppo, i loro amministratori possono fare queste cose anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

Per informazioni su come gli utenti con una licenza Plan possono creare un team, consulta [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Per informazioni su come un amministratore Workfront può creare un team, consulta [Crea un team dall&#39;area Configurazione](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Visualizzare, lavorare con e creare team per il gruppo dall’area Gruppi

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fai clic sul nome del gruppo per il quale desideri creare o modificare i team.
1. Nel pannello a sinistra, fai clic su **Team** ![](assets/teams.png) per elencare i team associati al gruppo e a eventuali sottogruppi.

1. Effettua una delle seguenti operazioni:

   * **Aggiungi un team**: Fai clic su **Nuovo team**, quindi utilizza le seguenti opzioni per configurarlo:
   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Nome team</td> 
       <td>Digita un nome per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Gruppo</td> 
       <td> <p> Il sistema compila il campo Gruppo del nuovo portfolio con il gruppo che stai visualizzando. Se si desidera associare il team a un gruppo diverso, iniziare a digitare il nome del gruppo, quindi selezionare il nome quando viene visualizzato.</p> <p>Per associare il gruppo destro al team, posiziona il puntatore del mouse su di esso e fai clic sull’icona delle informazioni <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> <p><b>NOTA</b>: Quando un team viene assegnato a un gruppo o a un sottogruppo, gli amministratori del gruppo o sottogruppo possono gestire il team senza esserne membri. Gli amministratori del gruppo possono accedere all'area Team dal menu principale e fare clic sulla freccia Cambia team <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi gestiti.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membri team</td> 
       <td> <p>Inizia a digitare il nome di un utente che deve far parte del team, quindi seleziona il nome quando viene visualizzato in nell’elenco a discesa. Ripeti questo processo per aggiungere più utenti al team.</p> <p>Non esiste alcun limite al numero di utenti che puoi aggiungere a un team. Tuttavia, consigliamo di non avere un numero eccessivo di utenti in un unico team, perché la gestione del lavoro del team potrebbe diventare troppo complessa.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descrizione</td> 
       <td>Digita una descrizione per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Calendario</td> 
       <td>Scegliere la scheda del calendario visualizzata per questo team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Lavoraci</td> 
       <td>Impostare il pulsante Lavora su un pulsante Start. Quando un utente fa clic su Start, lo stato dell’elemento viene aggiornato automaticamente.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Pulsante "Fine"</td> 
       <td>Selezionare lo stato da impostare per gli elementi quando si fa clic sul pulsante Fine.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Modifica team**: Seleziona almeno un team e fai clic su **la** Icona Modifica ![](assets/edit-icon.png), quindi utilizza le seguenti opzioni per configurarlo:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Nome team</td> 
       <td>Digita un nome per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Gruppo</td> 
       <td> <p>Associa il team a un gruppo. Iniziate a digitare il nome del gruppo, quindi selezionate il nome quando viene visualizzato.</p> <p>Per associare il gruppo destro al team, posiziona il puntatore del mouse su di esso e fai clic sull’icona delle informazioni <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> <p><b>NOTA</b>: Quando un team viene assegnato a un gruppo o a un sottogruppo, gli amministratori del gruppo o sottogruppo possono gestire il team senza esserne membri. Gli amministratori del gruppo possono accedere all'area Team dal menu principale e fare clic sulla freccia Cambia team <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi gestiti.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Proprietario</td> 
       <td>Selezionare un proprietario per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membri team</td> 
       <td> <p>Aggiungi e membri del team. Inizia a digitare il nome di un utente, quindi seleziona il nome quando viene visualizzato. Ripeti questo processo per aggiungere più utenti al team.</p> <p><b>SUGGERIMENTO</b>: Non esiste alcun limite al numero di utenti che puoi aggiungere a un team. Tuttavia, consigliamo di non avere un numero eccessivo di utenti in un unico team, perché la gestione del lavoro del team potrebbe diventare troppo complessa.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descrizione</td> 
       <td>Digita una descrizione per il team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Modello di layout</td> 
       <td> <p>Iniziare a digitare il nome del modello di layout che si desidera utilizzare per il team, quindi fare clic su di esso quando viene visualizzato.</p> <p>Quando si designa il team con questo modello di layout come Home Team di utenti, tutti gli utenti del team visualizzeranno le personalizzazioni in questo modello di layout.<br>Le impostazioni dei singoli modelli di layout sovrascriveranno le impostazioni del modello di layout del team principale. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Specifica se si tratta di un team agile. Per informazioni sui team agili e su come gestire il loro lavoro, vedi <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team agile</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Lavoraci</td> 
       <td> <p>Impostare il pulsante Lavora su un pulsante Start. Quando un utente fa clic su Start, lo stato dell’elemento viene aggiornato automaticamente.</p> <p>Per ulteriori informazioni su come configurare il pulsante Start, vedi <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Work On It con un pulsante Start</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Pulsante "Fine"</td> 
       <td> <p>Personalizza il pulsante Fine. Per ulteriori informazioni, consulta:</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configura il pulsante Fine per le attività</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configura il pulsante Fine per i problemi</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Eliminare i team**: Seleziona almeno un team, quindi fai clic sull’icona Elimina ![](assets/delete.png).
   * **Esportare l’elenco dei team**: Fai clic su **Esporta** ![](assets/export.png), quindi selezionare il formato di file desiderato per l’elenco esportato.
