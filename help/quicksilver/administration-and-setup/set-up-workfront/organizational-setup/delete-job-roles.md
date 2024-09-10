---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Cancella Ruoli
description: Puoi eliminare le mansioni che la tua organizzazione non utilizza più. È consigliabile non eliminare le mansioni associate a elementi di lavoro in passato. Per conservare tutte le informazioni cronologiche sulle assegnazioni di lavoro, è consigliabile disattivare i ruoli anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, vedere Disattivare i ruoli.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Elimina mansioni

Puoi eliminare le mansioni che la tua organizzazione non utilizza più. È consigliabile non eliminare le mansioni associate a elementi di lavoro in passato.

Per conservare tutte le informazioni cronologiche sulle assegnazioni di lavoro, è consigliabile disattivare i ruoli anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, vedere [Disattivare i ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>
   <p>Nuovo: [!UICONTROL Standard]</p>
   <p>Oppure</p>
   <p>Corrente: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai Ruoli</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare una mansione

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Ruoli].**
1. Seleziona la mansione da eliminare, quindi fai clic su **[!UICONTROL Elimina].**
1. Se esistono oggetti (utenti, attività, problemi) assegnati al ruolo, effettuare una delle seguenti operazioni:

   * **Sostituisci la mansione con una mansione diversa:** Seleziona la nuova mansione dall&#39;elenco a discesa.

     Tutte le allocazioni di risorse correnti e passate associate alla mansione eliminata vengono trasferite alla mansione selezionata.

     Gli utenti a cui è stata assegnata una sola mansione vengono riassegnati alla mansione selezionata; gli utenti a cui è stata assegnata una mansione secondaria non vengono riassegnati alla mansione selezionata.

   * **Eliminare la mansione e la relativa allocazione di risorse:** Selezionare **[!UICONTROL Nessuno]** dall&#39;elenco a discesa.

     >[!IMPORTANT]
     >
     >L&#39;eliminazione di un ruolo comporta l&#39;eliminazione di tutte le allocazioni di risorse correnti e passate correlate a tale ruolo per tutti i progetti.

     &#x200B;Ad esempio, se un’attività o un problema è assegnato solo a tale mansione, l’attività o il problema non viene assegnato dopo l’eliminazione della mansione.

1. Fare clic su **[!UICONTROL Sì, Elimina]**.
