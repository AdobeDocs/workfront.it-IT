---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Riordinare gli stati a livello di sistema e di gruppo
description: In qualità di amministratore di Workfront, puoi modificare l’ordine del progetto, delle attività e degli stati di emissione per tutti gli utenti del sistema o per un singolo gruppo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# Riordinare gli stati a livello di sistema e di gruppo

In qualità di amministratore di Workfront, puoi modificare l’ordine del progetto, delle attività e degli stati di emissione per tutti gli utenti del sistema o per un singolo gruppo.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Il riordinamento degli stati a livello di sistema non influisce sull’ordine degli stati all’interno dei gruppi.
>
>  Tuttavia, gli stati all’interno di un gruppo di livello superiore appena creato ereditano l’ordine degli stati a livello di sistema. Un nuovo sottogruppo eredita l’ordine degli stati del gruppo di un livello superiore.
>
>* È possibile riordinare gli stati bloccati. Per informazioni sugli stati bloccati, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Gli amministratori dei gruppi possono inoltre riordinare gli stati utilizzati nei loro gruppi. Per ulteriori informazioni, consulta [Riordinare gli stati del gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront* </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore Workfront. Per informazioni sugli amministratori di Workfront, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Ordine predefinito degli stati

Per impostazione predefinita, gli stati vengono visualizzati nell’ordine seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Progetto</th> 
   <th width="33.33%">Attività</th> 
   <th width="33.33%">Problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Attuali</li> 
     <li>Morto</li> 
     <li> In sospeso </li> 
     <li> In Pianificazione </li> 
     <li> Completato </li> 
     <li> Richiesto </li> 
     <li> Approvato </li> 
     <li> Rifiutato </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nuovo</li> 
     <li>In corso</li> 
     <li>Completato</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nuovo</li> 
     <li>In corso</li> 
     <li>Ri-Aperto</li> 
     <li>In attesa di Riscontro</li> 
     <li>In sospeso</li> 
     <li>Non Duplicabile</li> 
     <li>Chiuso</li> 
     <li>Risolto</li> 
     <li>Verifica Completata</li> 
     <li>Non Risolvibile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Riordinare gli stati per attività e progetti a livello di sistema o per un gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze progetto > Stati**.
1. (Condizionale) Se stai riordinando gli stati per un gruppo, inizia a digitare il nome del gruppo nella casella nell&#39;angolo in alto a destra, quindi fai clic sul nome quando viene visualizzato.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Sopra l’elenco Stati visualizzato, fai clic sul pulsante **Progetti** o **Attività** scheda .

1. Trascina e rilascia gli stati nell’ordine desiderato.

   Il nuovo ordine di stato viene salvato automaticamente.

1. Per verificare il nuovo ordine di stato, passare a un&#39;attività o a un progetto, fare clic sullo stato nell&#39;angolo in alto a destra e assicurarsi che gli stati visualizzati siano nell&#39;ordine configurato.

## Riordinare gli stati per i problemi

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze progetto > Stati.**
1. (Condizionale) Se stai riordinando gli stati per un gruppo, inizia a digitare il nome del gruppo nella casella nell&#39;angolo in alto a destra, quindi fai clic sul nome quando viene visualizzato.

   ![](assets/issue-statuses-group-name.png)

1. Fai clic sul pulsante **Problemi** scheda .
1. (Facoltativo) Seleziona un tipo di problema (**Report bug**, **Cambia ordine**, **Problema** oppure **Richiesta**).

   >[!NOTE]
   >
   >* Non è possibile personalizzare l’ordine degli stati per l’elenco principale.
   >* È consigliabile ordinare gli stati per ogni tipo di problema allo stesso modo. Per ulteriori informazioni sui tipi di problemi, vedi [Configurare i tipi di richiesta](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Trascina e rilascia gli stati nell’ordine desiderato.

   Il nuovo ordine di stato viene salvato automaticamente.

1. Per verificare il nuovo ordine di stato, apri un problema, fai clic sullo stato nell’angolo in alto a destra e assicurati che gli stati visualizzati siano nell’ordine configurato.
