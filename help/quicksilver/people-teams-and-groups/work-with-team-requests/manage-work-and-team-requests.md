---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Gestire le richieste di lavoro e team
description: Una richiesta rappresenta un'attività o un'assegnazione di problema in sospeso. Le richieste di lavoro vengono inviate ai singoli utenti e le richieste dei team ai team.
author: Jenny
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Gestire le richieste di lavoro e team

Una richiesta rappresenta un&#39;attività o un&#39;assegnazione di problema in sospeso. Le richieste di lavoro vengono inviate ai singoli utenti e le richieste dei team ai team.

>[!NOTE]
>
>I team Agile non dispongono di richieste team.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Per assegnare o lavorare su una richiesta:
   <p>Chiaro o superiore</p>
  <p>Revisione o successiva</p>
   <p>Per riassegnare una richiesta:
   <p>Standard</p>
   <p>Lavoro o superiore</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Assegnare una richiesta a un team {#assign-a-request-to-a-team}

I project manager e i richiedenti dei problemi possono assegnare il lavoro ai team quando non sanno quale risorsa è adatta per eseguire il lavoro o quando non importa chi completa il lavoro.

Le attività assegnate al team rimangono nella scheda [!UICONTROL Richieste team] fino a quando un utente del team non si offre volontario per lavorare alla richiesta.

Quando una richiesta viene assegnata sia a un team che a un utente che non è membro del team, la richiesta è visibile sia nella scheda [!UICONTROL Richieste team] che nell&#39;area delle richieste di lavoro dell&#39;utente. Se l&#39;utente che non fa parte del team si offre volontario per lavorare sull&#39;attività, l&#39;attività rimane comunque nella scheda [!UICONTROL Richieste team] fino a quando un utente del team non si offre volontario per lavorarci.

I team possono essere assegnati ad attività e problemi in uno dei seguenti modi:

* Tramite il [!UICONTROL Diagramma di Gantt]
* Da un elenco di attività o problemi (singolarmente o in blocco)
* Quando un’attività o un problema viene creato o modificato
* Tramite regole di instradamento su una richiesta (solo problemi)

Puoi assegnare manualmente una richiesta a un team dalla pagina del team, come descritto in questa sezione.

Per assegnare manualmente una richiesta a un team dalla pagina del team:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team icona](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Fai clic sull&#39;icona **[!UICONTROL Altro]** ![](assets/more-icon.png), quindi seleziona **[!UICONTROL Invia richiesta di lavoro]**.

   ![](assets/edit-team-settings-350x205.png)

1. Compila le informazioni nella casella visualizzata.
1. Fai clic su **[!UICONTROL Invia richiesta]**.\
   Al team viene ora assegnata una nuova attività che viene visualizzata nella scheda Richieste team. Questa attività non è attualmente associata a un progetto, ma può essere spostata, come descritto in [Sposta attività](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Riassegna richieste {#reassign-requests}

Puoi riassegnare le richieste assegnate al team:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team icona](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Nel pannello di navigazione a sinistra, seleziona **[!UICONTROL Richieste team]**.
1. Fai clic sull&#39;icona **[!UICONTROL Riassegna]**.

1. Iniziare a digitare il nome dell&#39;utente, del gruppo o del team a cui si desidera riassegnare la richiesta, quindi fare clic su **[!UICONTROL Assegna]**.\
   La richiesta viene riassegnata.
