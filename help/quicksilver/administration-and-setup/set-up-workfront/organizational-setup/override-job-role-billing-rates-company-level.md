---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Sostituisci tariffe di fatturazione mansione a livello aziendale
description: Quando viene creato un ruolo, è possibile selezionare una tariffa di fatturazione oraria per tale ruolo. Puoi creare una tariffa di fatturazione oraria specifica per una società.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# Sostituisci le tariffe di fatturazione dei ruoli a livello aziendale

Quando viene creato un ruolo, è possibile selezionare una tariffa di fatturazione oraria per tale ruolo. Puoi creare più tariffe di fatturazione orarie specifiche per una società. Ogni tariffa di fatturazione è valida per un intervallo di date specifico.

A livello di progetto, è possibile abilitare un&#39;opzione per consentire alle tariffe di fatturazione a livello di società di sostituire le tariffe a livello di progetto. Per ulteriori informazioni, vedere [Sostituire le tariffe di fatturazione a livello di progetto con le tariffe di fatturazione a livello di società](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

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
   <td> <p>Accesso amministrativo alle società se non si è amministratori di sistema</p>
   <p>Modifica accesso ai dati finanziari</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sostituisci o modifica una tariffa di fatturazione stabilita utilizzata per una mansione specifica

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Aziende]**.
1. Individua l&#39;azienda a cui è assegnata la mansione.
1. Fare clic sul nome della società nell&#39;elenco.
1. Fai clic su **[!UICONTROL Tariffe di fatturazione]** nel pannello a sinistra.
1. Fai clic su **[!UICONTROL Aggiungi tariffa di fatturazione] > [!UICONTROL Nuova tariffa di fatturazione]** oppure scegli una tariffa esistente da modificare.
1. Nella finestra di dialogo [!UICONTROL Nuova tariffa di fatturazione], seleziona una [!UICONTROL **mansione**] per definire la tariffa di fatturazione per.

   La [!UICONTROL **tariffa di fatturazione predefinita**] visualizza la tariffa a livello di sistema per questa mansione.

   ![Finestra di dialogo Nuova tariffa di fatturazione](assets/date-effective-billing-rates-for-company.png)

1. Nel campo [!DNL **Tariffe di fatturazione 1**] immettere la tariffa di fatturazione. Quindi, fai clic su [!UICONTROL **Salva**] per sostituire una volta la tariffa di fatturazione.

   Oppure

   Fai clic su [!UICONTROL **Aggiungi tariffa**] per aggiungere altre tariffe di fatturazione con date di validità.

1. (Condizionale) Se si stanno aggiungendo più tariffe di fatturazione, inserire le seguenti informazioni:

   * **[!UICONTROL Tariffe di fatturazione 1], 2, ecc.**: valore della tariffa di fatturazione per il periodo di tempo.
   * **[!UICONTROL Data inizio]**: la data in cui la tariffa diventa effettiva.
   * **[!UICONTROL Data di fine]**: la data in cui termina la tariffa.

     La tariffa di fatturazione 1 non avrà una data di inizio e l&#39;ultima tariffa di fatturazione non avrà una data di fine. Alcune date vengono aggiunte automaticamente. Ad esempio, se la tariffa di fatturazione 1 non ha una data di fine e si aggiunge la tariffa di fatturazione 2 con una data di inizio del 1° maggio 2023, alla tariffa di fatturazione 1 viene aggiunta una data di fine del 30 aprile 2023 in modo che non esistano spazi vuoti.

1. Fai clic su [!UICONTROL **Salva**].

   >[!NOTE]
   >
   >I tassi di ruolo modificati nel progetto avranno effetto solo su tale progetto. I tassi modificati a livello aziendale avranno un impatto su tutti i progetti. Per ulteriori informazioni, vedere [Panoramica sull&#39;override delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
