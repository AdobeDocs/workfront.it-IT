---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: Concedere l’accesso agli oggetti nell’area Home
description: Gli utenti possono richiedere l’accesso agli oggetti all’interno di Adobe Workfront. Per ulteriori informazioni sulla richiesta di accesso, vedere Richiedere l'accesso agli oggetti.
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Concedere l’accesso agli oggetti nell’area Home

<!--Audited: 10/2024-->

Gli utenti possono richiedere l’accesso agli oggetti all’interno di Adobe Workfront.

Per ulteriori informazioni sulla richiesta di accesso, vedere [Richiedere l&#39;accesso agli oggetti](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).

Se si è il proprietario di un oggetto, è possibile concedere o negare l&#39;accesso agli elementi dall&#39;area Home.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Nuovo: Standard</p> 
   <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi o documenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per progetti, attività, problemi o documenti</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Concedere l’accesso agli oggetti nell’area Home

1. Fai clic sul **menu principale** ![](assets/dots-main-menu.png) nell&#39;angolo superiore destro dello schermo o sul **menu principale** ![](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Home**
Oppure
Fai clic sull&#39;icona **Home** ![](assets/home-icon-30x29.png) nell&#39;angolo superiore sinistro di Adobe Workfront.

   >[!NOTE]
   >
   >L’amministratore di Workfront potrebbe apportare le seguenti modifiche all’icona Home nel tuo ambiente:
   >
   >* Sostituiscilo con un’immagine personalizzata per illustrare la tua organizzazione. In questo caso, l’icona avrà un aspetto diverso da quello mostrato in questo articolo.
   >* Sostituisci la pagina collegata con un’altra pagina. In questo caso, fai clic sul **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro della pagina, quindi fai clic su **Home**.

1. Effettua le seguenti operazioni:

   1. Vai al widget **Le mie approvazioni** e trova la richiesta di accesso aggiuntivo, quindi fai clic su **Concedi l&#39;accesso**.

      ![](assets/request-for-access-to-project-in-new-home-approvals-widget.png)

   1. (Facoltativo) Per concedere un livello di accesso diverso da quello richiesto, fai clic sul menu a discesa a sinistra del pulsante Concedi l&#39;accesso e seleziona il nuovo accesso, quindi fai clic su **Concedi l&#39;accesso**.

      La richiesta di accesso viene concessa e scompare dall’elenco delle richieste di approvazione.

1. (Facoltativo) Fai clic su **Ignora** per negare l&#39;accesso. La richiesta di accesso non viene concessa e scompare dall’elenco delle richieste di approvazione.

## Configurare le notifiche e-mail per le richieste di accesso

Puoi configurare la ricezione di notifiche e-mail per le richieste di accesso. L&#39;amministratore di Workfront può disabilitare questa funzionalità (come descritto in [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

1. Vai al tuo profilo utente effettuando una delle seguenti operazioni:

   * Fai clic sul **menu principale** ![](assets/dots-main-menu.png) nell&#39;angolo superiore destro dello schermo, quindi fai clic sul tuo nome.
   * Adobe Fai clic sul **menu principale** ![](assets/adobe-blue-main-menu.png) nell&#39;angolo superiore destro, se disponibile, quindi fai clic su **Profilo Workfront**.

1. Fai clic sul menu **Altro** ![](assets/more-icon.png) a destra del tuo nome nell&#39;intestazione, quindi fai clic su **Modifica**.
1. Fai clic su **Notifiche** e seleziona o deseleziona **Qualcuno richiede a me l&#39;accesso** nella sezione **Azione richiesta**, a seconda che tu desideri ricevere le notifiche e-mail quando un altro utente richiede l&#39;accesso da te o meno.

   Puoi abilitare una notifica giornaliera o immediata.

1. Fai clic su **Salva modifiche**.

<!--1. (Conditional) From the legacy Home area, do the following: 
   
   1. In the **Work List**, select the access request you want to manage in the **Approvals** section.  

   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

   The request displays on the right of the Work List. 

   1. In the upper-right corner, click the grant access button.  
   Depending on the type of access requested, the button name changes. For example, if the requestor asks for View access, the button says **Grant View Access**.  
   ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

   1. (Optional) To grant a different level of access than requested, click the arrow next to the grant access button and select the new access, then click **Grant < Permission level > Access >**.  
   A message appears confirming access was granted.  
   
   1. (Optional) Click **Ignore** to deny access.  
   A message appears confirming access was ignored.-->
