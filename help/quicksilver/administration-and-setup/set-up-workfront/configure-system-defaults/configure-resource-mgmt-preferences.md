---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurare le preferenze di Gestione risorse
description: Come un [!DNL Adobe Workfront] amministratore è possibile configurare le Preferenze di Gestione risorse per il sistema. Queste preferenze di Gestione risorse determinano il modo in cui vengono calcolati la disponibilità o la capacità utente e l'FTE per [!DNL Workfront] strumenti di pianificazione e pianificazione delle risorse.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Configura [!UICONTROL Gestione risorse] preferenze

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Come un [!DNL Adobe Workfront] amministratore è possibile configurare [!UICONTROL Gestione risorse] Preferenze per il sistema. Queste preferenze determinano il modo in cui vengono calcolati l’ora dell’utente, la disponibilità o la capacità FTE per [!DNL Workfront] strumenti di pianificazione e pianificazione delle risorse.

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Livello di accesso Amministratore di sistema</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>:

Se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Informazioni prese in considerazione nel calcolo della capacità di un utente

Nel calcolare la capacità di un utente, Workfront prende in considerazione le seguenti informazioni:

* Workfront Il numero di ore pianificate, come definito nella Pianificazione dell&#39;utente o nel [!UICONTROL Pianificazione predefinita]
* [!UICONTROL Pianificazione] [!UICONTROL Eccezioni] (a seconda di quale [!UICONTROL Pianificazione] possono essere le eccezioni della pianificazione dell&#39;utente o quelle associate alla [!DNL Workfront] [!UICONTROL Pianificazione predefinita])
* Indisponibilità dell&#39;utente
* Il valore dell&#39;equivalente a tempo pieno ([!UICONTROL FTE]) dell&#39;utente o dell&#39;utente [!DNL Workfront] di rete. Il [!UICONTROL FTE] è uguale a 1 quando l’utente lavora a tempo pieno, come definito nella pianificazione.
* Il valore di [!UICONTROL Orario di lavoro] per l’utente che fa riferimento al tempo trascorso dall’utente sul lavoro relativo al progetto. Non sono compresi i tempi di lavoro, come riunioni e corsi di formazione. Il [!UICONTROL Orario di lavoro] è uguale a 1 quando l’utente è disponibile per lavorare tutto il tempo come indicato da [!UICONTROL FTE] o la pianificazione, il che significa che non trascorrono tempo su lavori non correlati al progetto, come riunioni o corsi di formazione.


Per informazioni sulle risorse di pianificazione e programmazione in [!DNL Workfront], vedi [Introduzione alla gestione delle risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configura [!UICONTROL Gestione risorse] preferenze

>[!NOTE]
>
>Poiché si tratta di un&#39;impostazione globale, questa selezione influisce su tutti i calcoli per l&#39;intero sistema, per tutti gli utenti, in tutti gli strumenti di gestione delle risorse.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Clic **[!UICONTROL Gestione risorse]**.
1. Selezionare uno dei metodi seguenti per calcolare la disponibilità degli utenti in [!DNL Workfront]:

   * **Lo Schedule Predefinito**: [!DNL Workfront] utilizza la pianificazione predefinita del sistema e il singolo FTE dell’utente per calcolare le ore disponibili dell’utente negli strumenti di gestione delle risorse.

      Per ulteriori informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Per ulteriori informazioni su come individuare il valore del [!UICONTROL FTE], vedi  [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcola le ore disponibili di un utente utilizzando la formula seguente quando l’amministratore di Workfront sceglie [!UICONTROL Pianificazione predefinita]:


      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


      >[!INFO]
      >
      >Ad esempio, se la pianificazione predefinita è di 40 ore alla settimana, l’FTE nel profilo dell’utente è 0,5, l’utente ha 1 ora di inattività in un giorno e il [!UICONTROL Orario di lavoro] nel profilo dell’utente è 0,5, l’utente è disponibile per il lavoro effettivo del progetto per 9,5 ore alla settimana.
      >
      >Se l’utente ha 1 ora di inattività in un giorno, le ore disponibili verranno calcolate come segue:
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`

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

   * **La pianificazione dell&#39;utente**: [!DNL Workfront] utilizza la pianificazione dell&#39;utente e [!UICONTROL Pianificazione predefinita] del sistema per calcolare il valore Disponibile [!UICONTROL FTE] valore dell’utente negli strumenti di gestione delle risorse. Le ore disponibili vengono calcolate solo in base alla pianificazione dell&#39;utente. Il valore della proprietà [!UICONTROL FTE] dell’utente viene ignorata. Questa è l&#39;impostazione predefinita.

      Per ulteriori informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Per ulteriori informazioni sulle [!UICONTROL Pianificazione], vedi  [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Se l&#39;utente non è associato a una pianificazione, le Ore disponibili per l&#39;utente vengono calcolate utilizzando solo [!UICONTROL Pianificazione predefinita].

      Le ore disponibili per l’utente vengono calcolate con la seguente formula:


      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


      Disponibile [!UICONTROL FTE] per l’utente viene calcolato con la seguente formula:


      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


      >[!INFO]
      >
      >Ad esempio, se [!UICONTROL Pianificazione predefinita] è di 40 ore alla settimana, la pianificazione dell’utente è di 30 ore alla settimana e il [!UICONTROL Orario di lavoro] è 0,5 [!UICONTROL FTE] dell&#39;utente è 0,35.
      >
      >Se l’utente ha 2 ore di ferie in un giorno, le loro Settimane disponibili [!UICONTROL FTE] viene calcolato come segue:
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`

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
