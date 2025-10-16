---
product-area: projects
navigation-topic: financials
title: Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società
description: Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puoi configurare un progetto in modo che utilizzi le tariffe di fatturazione a livello di società anziché quelle a livello di progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a progetti e dati finanziari</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Gestire le autorizzazioni per il progetto con le autorizzazioni per Gestire le finanze</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilita l&#39;opzione di sostituzione delle tariffe di fatturazione a livello di società

Quando una società è associata a un progetto e questa opzione è abilitata, le modifiche fatte alle tariffe di fatturazione della società sovrascrivono la tariffa di fatturazione impostata sul progetto.

Quando un utente ricalcola manualmente i dati finanziari sul progetto, vengono applicate eventuali modifiche alle tariffe di fatturazione della società. Anche i calcoli dei ricavi storici vengono sostituiti a meno che non vengano contrassegnati come fatturati.

1. Vai a un progetto.
1. Fai clic sul menu **Altro** ![Altro menu](assets/qs-more-icon-on-an-object.png) accanto al nome del progetto nell&#39;intestazione, quindi fai clic su **Modifica**.
1. Nella sezione **Finanza**, abilita **Consenti tariffe di fatturazione a livello di società per sostituire le tariffe di fatturazione a livello di progetto**.

   >[!CAUTION]
   >
   >L’abilitazione di questa opzione sostituisce i calcoli dei ricavi storici a meno che non siano contrassegnati come fatturati. Puoi conservare i calcoli dei ricavi storici creando un record di fatturazione. Per ulteriori informazioni, vedere l&#39;articolo [Creare record fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Fai clic su **Salva modifiche**.

## Aggiornare le tariffe di fatturazione a livello aziendale e applicarle a un progetto

Dopo aver abilitato l&#39;opzione di sostituzione delle tariffe di fatturazione a livello di società in un progetto, le modifiche apportate alle tariffe di fatturazione della società vengono applicate al progetto in qualsiasi momento in cui vengono ricalcolati i dati finanziari.

>[!NOTE]
>
>Per aggiornare le tariffe di fatturazione a livello aziendale, gli utenti devono avere accesso alle Aziende nel proprio livello di accesso.

{{step-1-to-setup}}

1. Fai clic su **Aziende**.
1. Fare clic sul nome della società associata al progetto per la quale è stata abilitata la sostituzione delle tariffe di fatturazione a livello di società.
1. Fai clic su **Tariffe di fatturazione** nel pannello a sinistra.
1. Aggiornare la **tariffa di fatturazione aziendale** e le date di inizio/fine per una mansione esistente, quindi premere Invio.

   Per aggiungere una nuova tariffa di fatturazione della società con data effettiva, selezionare una tariffa di fatturazione per la mansione e fare clic su **Modifica**. Per ulteriori informazioni sulle tariffe di fatturazione della società valide per la data, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello di società](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Per aggiornare le tariffe aziendali per uno o più progetti, effettuare una delle seguenti operazioni:

   * Più progetti:

      1. Consente di passare a un elenco di progetti.
      1. Seleziona la casella di controllo in linea con i progetti da aggiornare.
      1. Fai clic su **Modifica**.
      1. Nella sezione Impostazioni abilitare l&#39;opzione **Ricalcola costi e ricavi**.
      1. Fai clic su **Salva modifiche**.

   * Progetto singolo:

      1. Vai al progetto per il quale hai abilitato la sostituzione delle tariffe di fatturazione a livello di società.
      1. Fai clic sul menu **Altro** ![Altro menu](assets/qs-more-icon-on-an-object.png) accanto al nome del progetto nell&#39;intestazione, quindi fai clic su **Ricalcola dati finanziari**.
