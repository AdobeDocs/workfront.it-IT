---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Escludere i tassi di fatturazione dei ruoli di lavoro a livello aziendale
description: Quando viene creato un ruolo di lavoro, è possibile selezionare un tasso di fatturazione orario per quel ruolo. Puoi creare una tariffa di fatturazione oraria specifica di un'azienda.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Escludere i tassi di fatturazione dei ruoli di lavoro a livello aziendale

Quando viene creato un ruolo di lavoro, è possibile selezionare un tasso di fatturazione orario per quel ruolo. Puoi creare una tariffa di fatturazione oraria specifica di un&#39;azienda.

A livello di progetto, puoi abilitare un’opzione per consentire alle tariffe di fatturazione a livello di società di ignorare le tariffe a livello di progetto. Per ulteriori informazioni, consulta [Sostituisci i tassi di fatturazione a livello di progetto con i tassi di fatturazione a livello di società](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo alle società se non sei un amministratore di sistema</p> <p>Accesso ai dati finanziari tramite modifica</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Escludere o modificare il tasso di fatturazione stabilito utilizzato per un ruolo di lavoro specifico

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Aziende]**.
1. Individua la società a cui è assegnato il ruolo di lavoro.
1. Fai clic su **[!UICONTROL Modifica società]** nell&#39;angolo in alto a destra.
1. In **[!UICONTROL Tassi di fatturazione]** selezionare il ruolo di lavoro da modificare e immettere il nuovo tasso di fatturazione per il ruolo di lavoro nel **[!UICONTROL Tasso di fatturazione della società]** scatola.

   >[!NOTE]
   >
   >Le percentuali di ruolo modificate nel progetto avranno solo un impatto sul progetto. I tassi modificati a livello aziendale avranno un impatto su tutti i progetti. Per ulteriori informazioni, consulta [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
