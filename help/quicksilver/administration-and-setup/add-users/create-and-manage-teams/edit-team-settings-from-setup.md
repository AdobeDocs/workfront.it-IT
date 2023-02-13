---
title: Modificare le impostazioni di un team dall'area Configurazione
description: In qualità di amministratore di Adobe Workfront, puoi modificare le impostazioni di un team dall’area Configurazione. È possibile aggiungere utenti a un team, impostare il modello di layout di un team e impostare il modo in cui viene registrato lo stato quando gli elementi di lavoro vengono completati da un team.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

# Modificare le impostazioni di un team dall&#39;area Configurazione

In qualità di amministratore di Adobe Workfront, puoi modificare le impostazioni di un team dall’area Configurazione. È possibile aggiungere utenti a un team, impostare il modello di layout di un team e impostare il modo in cui viene registrato lo stato quando gli elementi di lavoro vengono completati da un team.

Per informazioni sui team, consulta [Panoramica sui team](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un amministratore di gruppo può modificare le impostazioni di un team per un gruppo che amministra. Per ulteriori informazioni, consulta [Creare e modificare i team di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utente con una licenza di piano può modificare le impostazioni di un team dall&#39;area Persone. Per ulteriori informazioni, consulta [Modificare le impostazioni del team](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>


## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare le impostazioni di un team

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Team** nel pannello a sinistra.
1. Seleziona un team e fai clic su **Modifica** ![](assets/edit-icon.png).

1. Apporta una delle seguenti modifiche:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome team</td> 
      <td>Digita un nome per il team.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">È attivo </td> 
       <td>Per impostazione predefinita, questa opzione è abilitata per i team nuovi ed esistenti. Disattivala per disattivare il team. Per ulteriori informazioni, consulta <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Disattivare un team</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Gruppo</td> 
      <td> <p>Associa il team a un gruppo. Iniziate a digitare il nome del gruppo, quindi selezionate il nome quando viene visualizzato.</p> <p><b>NOTA</b>: Quando un team viene assegnato a un gruppo o a un sottogruppo, gli amministratori del gruppo o sottogruppo possono gestire il team senza esserne membri. Gli amministratori del gruppo possono accedere all'area Team dal menu principale e fare clic sulla freccia Cambia team <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi gestiti.</p> <p>Per associare il gruppo destro al team, posiziona il puntatore del mouse su di esso e fai clic sull’icona delle informazioni <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietario</td> 
      <td>Selezionare un proprietario per il team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri team</td> 
      <td> <p>Aggiungi e membri del team. Inizia a digitare il nome di un utente, quindi seleziona il nome quando viene visualizzato. Ripeti questo processo per aggiungere più utenti al team.</p> 
      <p><b>SUGGERIMENTO</b>: Puoi aggiungere un numero qualsiasi di utenti a un team. Tuttavia, consigliamo di non aggiungere un numero eccessivamente elevato in un unico team, perché la gestione del lavoro del team potrebbe diventare troppo complessa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digita una descrizione per il team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modello di layout</td> 
      <td> <p>Iniziare a digitare il nome del modello di layout che si desidera utilizzare per il team, quindi fare clic su di esso quando viene visualizzato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Specifica se si tratta di un team agile. Per informazioni sui team agili e su come gestire il loro lavoro, vedi <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team agile</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. Fai clic su **Salva modifiche**.
