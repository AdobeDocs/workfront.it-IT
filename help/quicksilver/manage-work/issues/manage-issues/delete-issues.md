---
product-area: projects
navigation-topic: manage-issues
title: Elimina problemi
description: Puoi eliminare problemi o richieste in Adobe Workfront se disponi dell’accesso e delle autorizzazioni corrette per farlo.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# Elimina problemi

Puoi eliminare problemi o richieste in Adobe Workfront se disponi dell’accesso e delle autorizzazioni corrette per farlo.

>[!TIP]
>
>&quot;Issues&quot; e &quot;requests&quot; vengono utilizzati in modo intercambiabile in Workfront. È possibile registrare i problemi relativi a progetti e attività per indicare il lavoro imprevisto che deve essere affrontato. È inoltre possibile inviare richieste registrate come problemi in un progetto designato come coda di richiesta.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Rivedi o una licenza superiore per eliminare i problemi nella sezione Problemi di un progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione a livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p>Visualizza o consente un accesso più elevato a progetti e attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso ai problemi relativi al livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul problema</p> <p>Collaborare o autorizzazioni superiori per il progetto o l'attività</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sull’eliminazione dei problemi

* L’amministratore di Workfront o un amministratore di gruppo deve abilitare l’eliminazione dei problemi relativi a un progetto con stato Completa nell’area Preferenze progetto. Per informazioni sulla configurazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se il problema ha registrato delle ore, l’amministratore di Workfront o un amministratore di gruppo deve consentire l’eliminazione di questi problemi configurando le preferenze relative a attività e problemi nell’istanza Workfront. Questo vale anche quando tenti di eliminare progetti che hanno problemi con le ore di accesso.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   Per ulteriori informazioni sull&#39;abilitazione dell&#39;eliminazione dei problemi relativi alle ore di registrazione, consulta la sezione &quot;Eliminazione&quot; in [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## L&#39;impatto dell&#39;eliminazione dei problemi

Quando elimini un problema, influisci sugli altri oggetti collegati al problema.

Quando elimini un problema vengono eliminati anche i seguenti oggetti associati a un problema:

* Documenti

   Non è possibile eliminare un problema a cui è allegato un documento estratto. Per ulteriori informazioni sull&#39;estrazione dei documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

* Note
* Approvazioni

A seconda della modalità in cui l’amministratore di Workfront o di gruppo configura le preferenze per l’eliminazione di progetti, attività o problemi in **Scheda attività e preferenze ora** dell’istanza Workfront, le ore registrate per i problemi vengono gestite in uno dei modi seguenti quando si elimina un problema:

* Passa al progetto e non verrà ripristinato sul problema, se il problema viene successivamente ripristinato.
* Se il problema viene successivamente ripristinato, verrà eliminato e ripristinato.

   Questo vale anche quando tenti di eliminare progetti che hanno attività con ore registrate su di essi.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   Per ulteriori informazioni sulla configurazione delle preferenze di eliminazione per le ore di accesso ai problemi, vedi [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Gli utenti assegnati al problema o all’approvazione del problema rimangono nel team di progetto.\
   Per ulteriori informazioni sui team di progetto, consulta [Panoramica del team di progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Elimina problemi

* [Eliminare contemporaneamente più problemi in un progetto](#delete-multiple-issues-in-a-project-simultaneously)
* [Elimina un singolo problema](#delete-a-single-issue)

### Eliminare contemporaneamente più problemi in un progetto  {#delete-multiple-issues-in-a-project-simultaneously}

1. Vai a **Menu principale**.
1. Fai clic su **Progetti**.
1. Fai clic sul nome del progetto contenente i problemi da eliminare.
1. Fai clic su **Problemi** nel pannello a sinistra.
1. Seleziona un problema, quindi fai clic sul pulsante **Elimina** icona ![](assets/delete.png) in cima all&#39;elenco.

1. Se l&#39;eliminazione è consentita, fai clic su **Sì, eliminalo**.\
   L’amministratore di Workfront potrebbe non consentire l’eliminazione dei problemi relativi alle ore di registrazione.\
   Per ulteriori informazioni sull&#39;accesso e le autorizzazioni necessarie per eliminare un problema, vedi [Problemi di eliminazione](#access-and-permissions-needed).

### Elimina un singolo problema {#delete-a-single-issue}

1. Fai clic sul pulsante **Principale** menu.
1. Fai clic su **Progetti**.
1. Fai clic sul nome del progetto contenente il problema da eliminare.
1. Fai clic su **Problemi** nel pannello a sinistra.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Fai clic sul nome del problema da eliminare.
1. Fai clic sul pulsante **Altro** menu.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Fai clic su **Elimina**.
1. Se l&#39;eliminazione è consentita, fai clic su **Sì, eliminalo**.

   L’amministratore di Workfront potrebbe non consentire l’eliminazione dei problemi relativi alle ore di registrazione.\
   Per ulteriori informazioni sull&#39;accesso e le autorizzazioni necessarie per eliminare un problema, vedi [Problemi di eliminazione](#access-and-permissions-needed).

## Ripristinare i problemi eliminati

Un amministratore di Workfront o di gruppo può ripristinare i problemi entro 30 giorni dalla loro eliminazione. Per ulteriori informazioni sul ripristino di elementi in Workfront, vedi [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
