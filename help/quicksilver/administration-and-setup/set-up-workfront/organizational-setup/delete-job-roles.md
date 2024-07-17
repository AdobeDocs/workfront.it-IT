---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Elimina mansioni
description: Puoi eliminare le mansioni che la tua organizzazione non utilizza più. È consigliabile non eliminare le mansioni associate a elementi di lavoro in passato. Per conservare tutte le informazioni cronologiche sulle assegnazioni di lavoro, è consigliabile disattivare i ruoli anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, vedere Disattivare i ruoli.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Elimina mansioni

Puoi eliminare le mansioni che la tua organizzazione non utilizza più. È consigliabile non eliminare le mansioni associate a elementi di lavoro in passato.

Per conservare tutte le informazioni cronologiche sulle assegnazioni di lavoro, è consigliabile disattivare i ruoli anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, vedere [Disattivare i ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo alle mansioni</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Eliminare una mansione

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

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
