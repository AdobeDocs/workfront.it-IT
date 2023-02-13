---
product-area: projects
navigation-topic: financials
title: Sostituisci i tassi di fatturazione a livello di progetto con i tassi di fatturazione a livello di società
description: Sostituisci i tassi di fatturazione a livello di progetto con i tassi di fatturazione a livello di società
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Sostituisci i tassi di fatturazione a livello di progetto con i tassi di fatturazione a livello di società

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puoi configurare un progetto in modo che utilizzi le tariffe di fatturazione a livello di azienda invece delle tariffe di fatturazione a livello di progetto.

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a progetti e dati finanziari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con autorizzazioni per Manage Finance</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Attiva l&#39;opzione di sostituzione Tassi di fatturazione a livello aziendale

Quando un&#39;azienda è associata a un progetto e questa opzione è abilitata, le modifiche apportate ai tassi di fatturazione a livello di azienda sovrascrivono il tasso di fatturazione impostato sul progetto.

Quando un utente ricalcola manualmente le finanze del progetto, vengono applicate tutte le modifiche ai tassi di fatturazione a livello aziendale. Vengono ignorati anche i calcoli storici dei ricavi, a meno che non siano contrassegnati come fatturati.

1. Vai a un progetto.
1. Fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome del progetto nell’intestazione, quindi fai clic su **Modifica**.
1. In **Finanza** abilitare **Consenti ai tassi di fatturazione a livello aziendale di ignorare i tassi di fatturazione a livello di progetto**.

   >[!CAUTION]
   >
   >L’abilitazione di questa opzione sostituisce i calcoli storici dei ricavi a meno che non siano contrassegnati come fatturati. È possibile mantenere i calcoli storici dei ricavi creando un record di fatturazione. Per ulteriori informazioni, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Fai clic su **Salva modifiche**.

## Aggiornare i tassi di fatturazione a livello aziendale e applicarli a un progetto

Dopo aver abilitato l&#39;opzione di sostituzione dei tassi di fatturazione a livello aziendale su un progetto, le modifiche apportate ai tassi di fatturazione dell&#39;azienda vengono applicate al progetto ogni volta che le finanze vengono ricalcolate.

>[!NOTE]
>
>Gli utenti devono avere accesso alle Aziende nel loro livello di accesso per aggiornare le tariffe di fatturazione a livello aziendale.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione**.
1. Fai clic su **Aziende**.
1. Fai clic sul nome della società associata al progetto per cui hai abilitato la sostituzione delle tariffe di fatturazione a livello di società.
1. Fai clic su **Tassi di fatturazione** nel pannello a sinistra.
1. Immettere il nuovo tasso di fatturazione per un ruolo di lavoro esistente nel **Tasso di fatturazione della società** quindi premere Invio.
1. Per aggiornare le tariffe aziendali per uno o più progetti, eseguire una delle operazioni seguenti:

   * Più progetti:
   1. Vai a un elenco di progetti.
   1. Seleziona la casella di controllo in linea con i progetti da aggiornare.
   1. Fai clic su **Modifica**.
   1. Nella sezione Impostazioni , abilita **Ricalcolare Costi E Entrate** opzione .
   1. Fai clic su **Salva modifiche**.
   * Progetto unico:

      1. Passa al progetto per il quale hai abilitato la sostituzione delle tariffe di fatturazione a livello di società.
      1. Fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome del progetto nell’intestazione, quindi fai clic su **Ricalcola finanza**.
