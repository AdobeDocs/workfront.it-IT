---
product-area: projects
navigation-topic: manage-issues
title: Elimina problemi
description: Puoi eliminare problemi o richieste in Adobe Workfront se disponi dell’accesso e delle autorizzazioni corretti.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# Elimina problemi

<!--Audited: 05/2025-->

Puoi eliminare problemi o richieste in Adobe Workfront se disponi dell’accesso e delle autorizzazioni corretti.

>[!TIP]
>
>&quot;Problemi&quot; e &quot;richieste&quot; vengono utilizzati in modo intercambiabile in Workfront. È possibile registrare problemi relativi a progetti e attività per indicare il lavoro imprevisto che deve essere risolto. Puoi anche inviare richieste registrate come problemi in un progetto designato come coda richieste.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>
   <p>Corrente: richiesta o successiva</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul problema</p> <p>Autorizzazioni Contribute o superiori per il progetto o l'attività</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per l’eliminazione di problemi

* L’amministratore di Workfront o un amministratore di gruppo deve abilitare l’eliminazione dei problemi in un progetto che si trova nello stato Completato nell’area Preferenze progetto.

  Per informazioni sulla configurazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se il problema ha registrato delle ore, l’amministratore di Workfront o un amministratore di gruppo deve consentire l’eliminazione di questi problemi configurando le Preferenze attività e problemi nell’istanza Workfront. Ciò si applica anche quando si tenta di eliminare progetti che presentano problemi con le ore collegate.

  Per ulteriori informazioni sull&#39;abilitazione dell&#39;eliminazione dei problemi in cui sono registrate le ore, vedere la sezione &quot;Eliminazione&quot; in [Configurare l&#39;attività a livello di sistema e le preferenze dei problemi](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).


## Impatto dell’eliminazione dei problemi

Quando elimini un problema, questo influisce su altri oggetti collegati al problema.

Quando si elimina un problema, vengono eliminati anche i seguenti oggetti associati a un problema:

* Documenti

  Non è possibile eliminare un problema a cui è associato un documento estratto. Per ulteriori informazioni sull&#39;estrazione di documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

* Note
* Approvazioni

A seconda del modo in cui l&#39;amministratore di Workfront o di gruppo configura le preferenze per l&#39;eliminazione di progetti, attività o problemi nelle **preferenze per schede orario e ore** dell&#39;istanza di Workfront, le ore registrate per i problemi vengono gestite in uno dei seguenti modi durante l&#39;eliminazione di un problema:

* Passa al progetto e non verrà ripristinato nel caso in cui il problema venga successivamente ripristinato.
* Sarà eliminato e ripristinato al momento del problema, se il problema viene successivamente ripristinato.

  Ciò si applica anche quando si tenta di eliminare progetti che dispongono di attività con ore collegate.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Per ulteriori informazioni sulla configurazione delle preferenze di eliminazione per le ore collegate a problemi, vedere [Configurare le preferenze relative alle ore e alla scheda orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Gli utenti assegnati al problema o all’approvazione del problema rimangono nel team di progetto.\
  Per ulteriori informazioni sui team di progetto, vedere [Panoramica team di progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Elimina problemi

### Eliminare più problemi contemporaneamente in un progetto  {#delete-multiple-issues-in-a-project-simultaneously}

1. Passa al **menu principale**.
1. Fai clic su **Progetti**.
1. Fai clic sul nome del progetto che contiene i problemi da eliminare.
1. Fai clic su **Problemi** nel pannello a sinistra.

   A destra viene visualizzato un elenco di problemi associati al progetto selezionato.
1. Seleziona uno o più problemi nell&#39;elenco, quindi fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png) nella parte superiore dell&#39;elenco.

1. Se l&#39;eliminazione è consentita, scegliere **Elimina**.

   L’amministratore di Workfront potrebbe non consentire l’eliminazione dei problemi in cui sono registrate le ore.\
   Per ulteriori informazioni sull&#39;accesso e sulle autorizzazioni necessarie per eliminare un problema, vedere la sezione [Considerazioni per l&#39;eliminazione dei problemi](#considerations-for-deleting-issues) in questo articolo.

### Eliminare un singolo problema {#delete-a-single-issue}

{{step1-to-projects}}

1. Fai clic sul nome del progetto che contiene il problema da eliminare.
1. Fai clic su **Problemi** nel pannello a sinistra.

   ![Sezione problemi nel pannello a sinistra](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Fai clic sul nome del problema che desideri eliminare.
1. Fai clic sul menu **Altro** a destra del nome del problema.

   ![Menu Altro problema](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Fai clic su **Elimina problema**.
1. Fai clic su **Elimina** per.

   >[!NOTE]
   >
   >  L’amministratore di Workfront potrebbe non consentire l’eliminazione dei problemi in cui sono registrate le ore.\
   >  Per ulteriori informazioni sull&#39;accesso e sulle autorizzazioni necessarie per eliminare un problema, vedere la sezione [Considerazioni per l&#39;eliminazione dei problemi](#considerations-for-deleting-issues) in questo articolo.

## Ripristina problemi eliminati

Un amministratore di Workfront o di gruppo può ripristinare i problemi entro 30 giorni dalla loro eliminazione.

Per ulteriori informazioni sul ripristino degli elementi in Workfront, vedere [Ripristinare gli elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
