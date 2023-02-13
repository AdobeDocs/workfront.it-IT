---
title: Crea un team dall'area Configurazione
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: In qualità di amministratore di Adobe Workfront, puoi creare un team dall’area Configurazione.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# Crea un team dall&#39;area Configurazione

In qualità di amministratore di Adobe Workfront, puoi creare un team dall’area Configurazione. Per informazioni sui team, consulta [Panoramica sui team](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un amministratore di gruppo può creare un team per un gruppo che amministra dall’area Configurazione. Per ulteriori informazioni, consulta [Creare e modificare i team di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utente con una licenza Plan può anche creare un team dall’area Persone. Per ulteriori informazioni, consulta [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
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

## Creare un team

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Team**, quindi fai clic su **Nuovo team**.

1. In **Nuovo team** casella visualizzata, specificare le informazioni seguenti:

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
      <td> <p>Se si desidera associare il team a un gruppo, iniziare a digitare il nome del gruppo, quindi selezionare il nome quando viene visualizzato.</p> <p>Per associare il gruppo destro al team, posiziona il puntatore del mouse su di esso e fai clic sull’icona delle informazioni <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> <p><b>NOTA</b>: Quando un team viene assegnato a un gruppo o a un sottogruppo, gli amministratori del gruppo o sottogruppo possono gestire il team senza esserne membri. Gli amministratori del gruppo possono accedere all'area Team dal menu principale e fare clic sulla freccia Cambia team <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi gestiti.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Questo è un team agile</td> 
      <td>Seleziona questo elemento se desideri configurare il nuovo team in modo che diventi un team agile. Per ulteriori informazioni sui team agili, vedi <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team agile</a>.</td> 
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

1. Fai clic su **Crea team**.

## Proprietari del team

Per impostazione predefinita, quando crei un team, diventi il proprietario del team.

Puoi visualizzare i proprietari del team per tutti i team quando crei un rapporto per i team e includere nel rapporto il campo Nome proprietario . (Per ulteriori informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
