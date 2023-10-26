---
product-area: projects
navigation-topic: financials
title: Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società
description: Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puoi configurare un progetto in modo che utilizzi le tariffe di fatturazione a livello di società anziché quelle a livello di progetto.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con le autorizzazioni per Gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Abilita l&#39;opzione di sostituzione delle tariffe di fatturazione a livello di società

Quando una società è associata a un progetto e questa opzione è abilitata, le modifiche fatte alle tariffe di fatturazione della società sovrascrivono la tariffa di fatturazione impostata sul progetto.

Quando un utente ricalcola manualmente i dati finanziari sul progetto, vengono applicate eventuali modifiche alle tariffe di fatturazione della società. Anche i calcoli dei ricavi storici vengono sostituiti a meno che non vengano contrassegnati come fatturati.

1. Vai a un progetto.
1. Fai clic su **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome del progetto nell’intestazione, quindi fai clic su **Modifica**.
1. In **Finanza** , abilita **Consenti tariffe di fatturazione a livello di società per sostituire le tariffe di fatturazione a livello di progetto**.

   >[!CAUTION]
   >
   >L’abilitazione di questa opzione sostituisce i calcoli dei ricavi storici a meno che non siano contrassegnati come fatturati. Puoi conservare i calcoli dei ricavi storici creando un record di fatturazione. Per ulteriori informazioni, consulta l’articolo [Crea record fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Clic **Salva modifiche**.

## Aggiornare le tariffe di fatturazione a livello aziendale e applicarle a un progetto

Dopo aver abilitato l&#39;opzione di sostituzione delle tariffe di fatturazione a livello di società in un progetto, le modifiche apportate alle tariffe di fatturazione della società vengono applicate al progetto in qualsiasi momento in cui vengono ricalcolati i dati finanziari.

>[!NOTE]
>
>Per aggiornare le tariffe di fatturazione a livello aziendale, gli utenti devono avere accesso alle Aziende nel proprio livello di accesso.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione**.
1. Clic **Aziende**.
1. Fare clic sul nome della società associata al progetto per la quale è stata abilitata la sostituzione delle tariffe di fatturazione a livello di società.
1. Clic **Tariffe di fatturazione** nel pannello a sinistra.
1. Aggiornare il **Tariffa di fatturazione della società** e le date di inizio/fine per una mansione esistente, quindi premere Invio.

   Per aggiungere una nuova tariffa di fatturazione della società con data effettiva, selezionare una tariffa di fatturazione per la mansione e fare clic su **Modifica**. Per ulteriori informazioni sulle tariffe di fatturazione aziendali effettive per data, consulta [Sostituisci le tariffe di fatturazione dei ruoli a livello aziendale](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Per aggiornare le tariffe aziendali per uno o più progetti, effettuare una delle seguenti operazioni:

   * Più progetti:

   1. Consente di passare a un elenco di progetti.
   1. Seleziona la casella di controllo in linea con i progetti da aggiornare.
   1. Clic **Modifica**.
   1. Nella sezione Settings, abilita **Ricalcolare Costi E Ricavi** opzione.
   1. Clic **Salva modifiche**.

   * Progetto singolo:

      1. Vai al progetto per il quale hai abilitato la sostituzione delle tariffe di fatturazione a livello di società.
      1. Fai clic su **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome del progetto nell’intestazione, quindi fai clic su **Ricalcola dati finanziari**.
