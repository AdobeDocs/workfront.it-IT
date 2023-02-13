---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Eliminare i ruoli di lavoro
description: È possibile eliminare i ruoli di lavoro non più utilizzati dalla propria organizzazione. Si consiglia di non eliminare i ruoli di lavoro se in passato sono stati associati a elementi di lavoro. Per conservare tutte le informazioni storiche sulle assegnazioni di lavoro, si consiglia di disattivare i ruoli, anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, vedere Disattivazione dei ruoli di lavoro.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Eliminare i ruoli di lavoro

È possibile eliminare i ruoli di lavoro non più utilizzati dalla propria organizzazione. Si consiglia di non eliminare i ruoli di lavoro se in passato sono stati associati a elementi di lavoro.

Per conservare tutte le informazioni storiche sulle assegnazioni di lavoro, si consiglia di disattivare i ruoli, anziché eliminarli quando diventano obsoleti. Per informazioni sulla disattivazione dei ruoli, consulta [Disattivazione dei ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

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
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai ruoli di lavoro</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Eliminare un ruolo di lavoro

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Ruoli processo].**
1. Selezionare il ruolo di processo da eliminare, quindi fare clic su **[!UICONTROL Elimina].**
1. Se sono presenti oggetti (utenti, attività, problemi) assegnati al ruolo di lavoro, eseguire una delle operazioni seguenti:

   * **Sostituisci il ruolo del processo con un altro ruolo:** Selezionare il nuovo ruolo del processo dall&#39;elenco a discesa.

      Tutte le allocazioni di risorse correnti e passate associate al ruolo di lavoro eliminato vengono trasferite al ruolo di processo selezionato.

      Gli utenti a cui è stato assegnato un solo ruolo di lavoro vengono riassegnati al ruolo selezionato; gli utenti a cui è stato assegnato un ruolo di lavoro secondario non vengono riassegnati al ruolo di lavoro selezionato.

   * **Elimina il ruolo del processo e la relativa allocazione delle risorse:** Seleziona **[!UICONTROL Nessuno]** dall’elenco a discesa.

      >[!IMPORTANT]
      >
      >L&#39;eliminazione di un ruolo di lavoro elimina tutte le assegnazioni di risorse correnti e passate relative a tale ruolo di lavoro per tutti i progetti.

      &#x200B; Ad esempio, se un&#39;attività o un problema viene assegnato solo a quel ruolo di lavoro, l&#39;attività o il problema viene rimosso dopo l&#39;eliminazione del ruolo di lavoro.

1. Fai clic su  **[!UICONTROL Sì, Elimina]**.
