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
TQID: https://experienceleague.adobe.com/jJA7M34HwNyM-906Poo9-uTVmB4kQnXMv8iBWminjjg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 9%

---

# Eliminare le mansioni

Puoi eliminare le mansioni che la tua organizzazione non utilizza più. È consigliabile non eliminare le mansioni associate a elementi di lavoro in passato.

Per conservare tutte le informazioni cronologiche sulle assegnazioni di lavoro, è consigliabile disattivare i ruoli anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, vedere [Disattivare i ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisiti di accesso

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Piano]</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai Ruoli</td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
