---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurare le preferenze di gestione delle risorse
description: In qualità di amministratore di  [!DNL Adobe Workfront] , puoi configurare le preferenze di gestione delle risorse per il tuo sistema. Queste preferenze di Gestione risorse determinano il modo in cui vengono calcolati la disponibilità o la capacità dell'utente e l'FTE per gli strumenti di pianificazione e pianificazione delle risorse  [!DNL Workfront] .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Configura preferenze [!UICONTROL Gestione risorse]

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

In qualità di amministratore di [!DNL Adobe Workfront], puoi configurare le [!UICONTROL preferenze di gestione delle risorse] per il tuo sistema. Queste preferenze determinano il modo in cui vengono calcolati l&#39;ora utente o la disponibilità o la capacità FTE per gli strumenti di pianificazione e pianificazione delle risorse [!DNL Workfront].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni prese in considerazione nel calcolo della capacità di un utente

Nel calcolare la capacità di un utente, Workfront prende in considerazione le seguenti informazioni:

* Il numero di ore pianificate, come definito nella Pianificazione dell&#39;utente o nella Pianificazione predefinita del sistema Workfront.
* Eccezioni pianificazione (a seconda della pianificazione utilizzata, possono essere eccezioni della pianificazione dell&#39;utente o associate alla pianificazione predefinita di Workfront).
* Indisponibilità dell&#39;utente.
* Valore dell&#39;equivalente a tempo pieno ([!UICONTROL FTE]) dell&#39;utente o del sistema [!DNL Workfront]. Il [!UICONTROL FTE] è uguale a 1 quando l&#39;utente lavora a tempo pieno, come definito nella pianificazione.
* Il valore di [!UICONTROL Tempo di lavoro] per l&#39;utente, che si riferisce al tempo che l&#39;utente trascorre sul lavoro correlato al progetto. Non sono compresi i tempi di lavoro, come riunioni e corsi di formazione. Il [!UICONTROL Tempo di lavoro] è uguale a 1 quando l&#39;utente è disponibile a lavorare per l&#39;intero tempo come indicato dal [!UICONTROL FTE] o dalla pianificazione, il che significa che non trascorre tempo su lavori non correlati al progetto, come riunioni o corsi di formazione.


Per informazioni sulla pianificazione e la programmazione delle risorse in [!DNL Workfront], vedere [Introduzione a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configura preferenze [!UICONTROL Gestione risorse]

>[!NOTE]
>
>Poiché si tratta di un&#39;impostazione globale, questa selezione influisce su tutti i calcoli per l&#39;intero sistema, per tutti gli utenti, in tutti gli strumenti di gestione delle risorse.

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Gestione risorse]**.
1. Selezionare uno dei metodi seguenti per calcolare la disponibilità degli utenti in [!DNL Workfront]:

   * **La pianificazione predefinita**: [!DNL Workfront] utilizza la pianificazione predefinita del sistema e il singolo FTE dell&#39;utente per calcolare le ore disponibili dell&#39;utente negli strumenti di gestione delle risorse.

     Per ulteriori informazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) e [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Quando questa opzione è selezionata, Workfront calcola le ore disponibili dell&#39;utente utilizzando la formula seguente:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Ad esempio, se la pianificazione predefinita è di 40 ore alla settimana, l&#39;FTE nel profilo dell&#39;utente è 0,5, l&#39;utente ha 1 ora di inattività al giorno e il [!UICONTROL Tempo di lavoro] nel profilo dell&#39;utente è 0,5 e l&#39;utente è disponibile per il lavoro effettivo del progetto per 9,5 ore alla settimana.
     >
     >Se l’utente ha 1 ora di inattività in un giorno, le ore disponibili verranno calcolate come segue:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



     <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **La pianificazione dell&#39;utente**: [!DNL Workfront] utilizza la pianificazione dell&#39;utente e la [!UICONTROL pianificazione predefinita] del sistema per calcolare il valore di [!UICONTROL FTE] disponibile dell&#39;utente negli strumenti di gestione delle risorse. Le ore disponibili vengono calcolate solo in base alla pianificazione dell&#39;utente e il valore di [!UICONTROL FTE] dell&#39;utente viene ignorato. Questa è l&#39;impostazione predefinita.

     Per ulteriori informazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) e [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Se l&#39;utente non è associato a una pianificazione, le ore disponibili per l&#39;utente vengono calcolate utilizzando solo la [!UICONTROL pianificazione predefinita].

     Le ore disponibili per l’utente vengono calcolate con la seguente formula:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Il valore di [!UICONTROL FTE] disponibile per l&#39;utente viene calcolato con la formula seguente:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Ad esempio, se la [!UICONTROL pianificazione predefinita] è di 40 ore settimanali, la pianificazione dell&#39;utente è di 30 ore settimanali, l&#39;orario di lavoro [!UICONTROL dell&#39;utente] è 0,5 e l&#39;FTE [!UICONTROL &#x200B; dell&#39;utente è 0,35.]
     >
     >Se l&#39;utente ha 2 ore di inattività in un giorno, le sue [!UICONTROL FTE] settimanali disponibili verranno calcolate come segue:
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Fai clic su **[!UICONTROL Salva]**.
