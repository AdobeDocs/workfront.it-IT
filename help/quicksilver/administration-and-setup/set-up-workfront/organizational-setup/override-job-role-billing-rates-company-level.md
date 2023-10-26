---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Sostituisci le tariffe di fatturazione dei ruoli a livello aziendale
description: Quando viene creato un ruolo, è possibile selezionare una tariffa di fatturazione oraria per tale ruolo. Puoi creare una tariffa di fatturazione oraria specifica per una società.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Sostituisci le tariffe di fatturazione dei ruoli a livello aziendale

Quando viene creato un ruolo, è possibile selezionare una tariffa di fatturazione oraria per tale ruolo. Puoi creare più tariffe di fatturazione orarie specifiche per una società. Ogni tariffa di fatturazione è valida per un intervallo di date specifico.

A livello di progetto, è possibile abilitare un&#39;opzione per consentire alle tariffe di fatturazione a livello di società di sostituire le tariffe a livello di progetto. Per ulteriori informazioni, consulta [Sostituisci tariffe di fatturazione a livello di progetto con tariffe di fatturazione a livello di società](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo alle società se non si è amministratori di sistema</p> <p>Accesso a [!UICONTROL Edit] ai dati finanziari</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Sostituisci o modifica una tariffa di fatturazione stabilita utilizzata per una mansione specifica

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Aziende]**.
1. Individua l&#39;azienda a cui è assegnata la mansione.
1. Fare clic sul nome della società nell&#39;elenco.
1. Clic **[!UICONTROL Tariffe di fatturazione]** nel pannello a sinistra.
1. Clic **[!UICONTROL Aggiungi tariffa di fatturazione] > [!UICONTROL Nuova tariffa di fatturazione]** oppure scegli una tariffa esistente da modificare.
1. In [!UICONTROL Nuova tariffa di fatturazione] , seleziona una [!UICONTROL **Ruolo**] per definire la tariffa di fatturazione per.

   Il [!UICONTROL **Tariffa di fatturazione predefinita**] visualizza il tasso a livello di sistema per questa mansione.

   ![Finestra di dialogo Nuova tariffa di fatturazione](assets/date-effective-billing-rates-for-company.png)

1. In [!DNL **Tariffe di fatturazione 1**] , inserire la tariffa di fatturazione. Quindi, fai clic su [!UICONTROL **Salva**] per sostituire una sola volta la tariffa di fatturazione.

   Oppure

   Clic [!UICONTROL **Aggiungi tariffa**] per aggiungere altre tariffe di fatturazione con date di validità.

1. (Condizionale) Se si stanno aggiungendo più tariffe di fatturazione, inserire le seguenti informazioni:

   * **[!UICONTROL Tariffe di fatturazione 1], 2, ecc.**: il valore della tariffa di fatturazione per il periodo di tempo.
   * **[!UICONTROL Data di inizio]**: la data in cui il tasso diventa effettivo.
   * **[!UICONTROL Data di fine]**: la data in cui termina il tasso.

     La tariffa di fatturazione 1 non avrà una data di inizio e l&#39;ultima tariffa di fatturazione non avrà una data di fine. Alcune date vengono aggiunte automaticamente. Ad esempio, se la tariffa di fatturazione 1 non ha una data di fine e si aggiunge la tariffa di fatturazione 2 con una data di inizio del 1° maggio 2023, alla tariffa di fatturazione 1 viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.

1. Fai clic su [!UICONTROL **Salva**].

   >[!NOTE]
   >
   >I tassi di ruolo modificati nel progetto avranno effetto solo su tale progetto. I tassi modificati a livello aziendale avranno un impatto su tutti i progetti. Per ulteriori informazioni, consulta [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
