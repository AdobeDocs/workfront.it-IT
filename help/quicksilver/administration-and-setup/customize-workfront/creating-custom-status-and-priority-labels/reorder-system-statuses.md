---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Riordina gli stati a livello di sistema e di gruppo
description: In qualità di amministratore di Workfront, puoi modificare l’ordine degli stati di progetto, attività e problema per tutti gli utenti del sistema o per un singolo gruppo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# Riordina gli stati a livello di sistema e di gruppo

In qualità di amministratore di Workfront, puoi modificare l’ordine degli stati di progetto, attività e problema per tutti gli utenti del sistema o per un singolo gruppo.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Il riordinamento degli stati a livello di sistema non influisce sull&#39;ordine degli stati all&#39;interno dei gruppi.
>
>  Tuttavia, gli stati all’interno di un gruppo di primo livello appena creato ereditano l’ordine degli stati a livello di sistema. (Un nuovo sottogruppo eredita l’ordine degli stati nel gruppo di un livello superiore).
>
>* È possibile riordinare gli stati bloccati. Per informazioni sugli stati bloccati, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Gli amministratori di gruppi possono anche riordinare gli stati utilizzati nei loro gruppi. Per ulteriori informazioni, vedere [Riordinare gli stati dei gruppi](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront* </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di Workfront. Per informazioni sugli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

## Ordine predefinito degli stati

Per impostazione predefinita, gli stati vengono visualizzati nell&#39;ordine seguente:

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
     <li> Richiesto il </li> 
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

## Riordina gli stati per attività e progetti a livello di sistema o per un gruppo

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Preferenze progetto > Stati**.
1. (Condizionale) Se si stanno riordinando gli stati per un gruppo, iniziare a digitare il nome del gruppo nella casella nell&#39;angolo superiore destro, quindi fare clic sul nome quando viene visualizzato.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Sopra l&#39;elenco Stati visualizzato, fare clic sulla scheda **Progetti** o **Attività**.

1. Trascina e rilascia gli stati nell’ordine desiderato.

   Il nuovo ordine di stato viene salvato automaticamente.

1. Per verificare il nuovo ordine di stato, accedi a un&#39;attività o a un progetto, fai clic sullo stato nell&#39;angolo in alto a destra e accertati che gli stati visualizzati siano nell&#39;ordine configurato.

## Riordina gli stati per i problemi

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fare clic su **Preferenze progetto > Stati.**
1. (Condizionale) Se si stanno riordinando gli stati per un gruppo, iniziare a digitare il nome del gruppo nella casella nell&#39;angolo superiore destro, quindi fare clic sul nome quando viene visualizzato.

   ![](assets/issue-statuses-group-name.png)

1. Fai clic sulla scheda **Issues**.
1. (Facoltativo) Seleziona un tipo di problema (**Segnalazione bug**, **Ordine di modifica**, **Problema** o **Richiesta**).

   >[!NOTE]
   >
   >* Non è possibile personalizzare l&#39;ordine degli stati per l&#39;elenco principale.
   >* È consigliabile ordinare allo stesso modo gli stati per ogni tipo di problema. Per ulteriori informazioni sui tipi di problema, vedere [Configurare i tipi di richiesta](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Trascina e rilascia gli stati nell’ordine desiderato.

   Il nuovo ordine di stato viene salvato automaticamente.

1. Per verificare il nuovo ordine di stato, accedi a un problema, fai clic sullo stato nell’angolo in alto a destra e assicurati che gli stati di visualizzazione siano nell’ordine configurato.
