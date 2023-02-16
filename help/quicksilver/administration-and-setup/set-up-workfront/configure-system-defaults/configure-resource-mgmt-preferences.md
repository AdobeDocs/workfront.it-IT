---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurare le preferenze di Gestione risorse
description: Come [!DNL Adobe Workfront] amministratore è possibile configurare le preferenze di gestione delle risorse per il sistema. Queste preferenze di Gestione delle risorse determinano in che modo la disponibilità o la capacità dell'utente e gli FTE vengono calcolati per [!DNL Workfront] strumenti di pianificazione e pianificazione delle risorse.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Configura [!UICONTROL Gestione risorse] preferenze

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Anteprima.</span>

Come [!DNL Adobe Workfront] amministratore puoi configurare le [!UICONTROL Gestione risorse] Preferenze del sistema. Queste preferenze determinano il modo in cui vengono calcolate la disponibilità o la capacità dell’utente in ore o FTE per [!DNL Workfront] strumenti di pianificazione e pianificazione delle risorse.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Livello di accesso amministratore di sistema</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>:

Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Informazioni prese in considerazione nel calcolo della capacità di un utente

Nel calcolo della capacità di un utente, Workfront tiene conto delle seguenti informazioni:

* Il numero di ore pianificate, come definito nella pianificazione dell&#39;utente o nel sistema Workfront [!UICONTROL Pianificazione predefinita]
* [!UICONTROL Pianificazione] [!UICONTROL Eccezioni] (a seconda di quale [!UICONTROL Pianificazione] viene utilizzato, può essere l&#39;eccezione della pianificazione dell&#39;utente o quelle associate al [!DNL Workfront] [!UICONTROL Pianificazione predefinita])
* Tempo di inattività dell&#39;utente
* Il valore dell&#39;equivalente a tempo pieno ([!UICONTROL FTE]) dell&#39;utente o del [!DNL Workfront] sistema. La [!UICONTROL FTE] è uguale a 1 quando l’utente lavora a tempo pieno, come definito nella pianificazione.
* <span class="preview">Il valore di [!UICONTROL Tempo di lavoro] per l’utente che fa riferimento al tempo che l’utente trascorre sul lavoro relativo al progetto. Questo non include i tempi di overhead, come riunioni e formazione. La [!UICONTROL Tempo di lavoro] è uguale a 1 quando l&#39;utente è disponibile per il lavoro per l&#39;intero periodo di tempo indicato dal [!UICONTROL FTE] o il programma, il che significa che non trascorrono del tempo in lavori non legati al progetto come riunioni o formazioni.</span>

Per informazioni sulla pianificazione e la pianificazione delle risorse in [!DNL Workfront], vedi [Guida introduttiva a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configura [!UICONTROL Gestione risorse] preferenze

>[!NOTE]
>
>Poiché si tratta di un’impostazione globale, questa selezione influisce su tutti i calcoli per l’intero sistema, per tutti gli utenti, in tutti gli strumenti di gestione delle risorse.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Fai clic su **[!UICONTROL Gestione risorse]**.
1. Selezionare uno dei metodi seguenti per calcolare la disponibilità degli utenti in [!DNL Workfront]:

   * **Pianificazione predefinita**: [!DNL Workfront] utilizza la pianificazione predefinita del sistema e il singolo FTE dell’utente per calcolare le ore disponibili dell’utente negli strumenti di gestione delle risorse.

      Per ulteriori informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Per ulteriori informazioni su come individuare il valore del [!UICONTROL FTE], vedi  [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcola le ore disponibili di un utente utilizzando la seguente formula quando l’amministratore di Workfront sceglie la [!UICONTROL Pianificazione predefinita]:


      Nell’ambiente di produzione:

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > Ad esempio, se [!UICONTROL Pianificazione predefinita] è di 40 ore alla settimana e il [!UICONTROL FTE] nel profilo dell’utente è 0,5, l’utente è disponibile per lavorare 20 ore alla settimana.
      >Se l’utente ha un’ora di inattività al giorno, le ore disponibili vengono calcolate come segue:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```

      <div class="preview">

      Nell’ambiente Anteprima:

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >Ad esempio, se la pianificazione predefinita è di 40 ore alla settimana, l’ETP nel profilo dell’utente è di 0,5, l’utente ha 1 ora di inattività un giorno e l’intervallo di tempo è pari a [!UICONTROL Tempo di lavoro] il profilo dell’utente è 0,5 e l’utente è disponibile per il lavoro effettivo del progetto per 9,5 ore alla settimana.
      >
      >Se l’utente ha un’ora di inattività al giorno, le ore disponibili vengono calcolate come segue:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>


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

   * **Pianificazione dell&#39;utente**: [!DNL Workfront] utilizza la pianificazione dell&#39;utente e [!UICONTROL Pianificazione predefinita] del sistema di calcolo della [!UICONTROL FTE] valore dell’utente negli strumenti di gestione delle risorse. Le ore disponibili vengono calcolate solo in base alla pianificazione dell’utente. Il valore del [!UICONTROL FTE] dell’utente viene ignorato. Questa è l’impostazione predefinita.

      Per ulteriori informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Per ulteriori informazioni su [!UICONTROL Pianificazione], vedi  [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Se l’utente non è associato a una pianificazione, le ore disponibili per l’utente vengono calcolate utilizzando solo il [!UICONTROL Pianificazione predefinita].

      Nell’ambiente di produzione:


      Le ore disponibili per l&#39;utente sono calcolate con la seguente formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```

      Disponibile [!UICONTROL FTE] per l&#39;utente viene calcolata dalla seguente formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Ad esempio, se [!UICONTROL Pianificazione predefinita] è di 40 ore alla settimana e il programma dell&#39;utente è di 30 ore alla settimana, [!UICONTROL FTE] dell’utente è 0,70.
      >  
      >Se l’utente ha 2 ore di tempo libero su un giorno, il Settimanale disponibile [!UICONTROL FTE] sono calcolati come segue:
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <div class="preview">

      Nell’ambiente Anteprima:

      Le ore disponibili per l&#39;utente vengono calcolate con la seguente formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      Disponibile [!UICONTROL FTE] per l&#39;utente viene calcolata dalla seguente formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Ad esempio, se [!UICONTROL Pianificazione predefinita] è di 40 ore a settimana, la pianificazione dell&#39;utente è di 30 ore a settimana e l&#39;orario [!UICONTROL Tempo di lavoro] è pari a 0,5 [!UICONTROL FTE] dell’utente è 0,35.
      >
      >Se l’utente ha 2 ore di tempo libero su un giorno, il Settimanale disponibile [!UICONTROL FTE] sono calcolati come segue:
      >
      >
      ```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```

      </div>

1. Fai clic su **[!UICONTROL Salva]**.
