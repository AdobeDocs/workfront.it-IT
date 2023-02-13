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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Configura [!UICONTROL Gestione risorse] preferenze

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Come [!DNL Adobe Workfront] amministratore puoi configurare le [!UICONTROL Gestione risorse] Preferenze del sistema. Queste preferenze determinano in che modo la disponibilità o la capacità dell’utente e gli FTE vengono calcolati per [!DNL Workfront] strumenti di pianificazione e pianificazione delle risorse.

Per informazioni sulla pianificazione e la pianificazione delle risorse in [!DNL Workfront], vedi [Guida introduttiva a Gestione risorse](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisiti di accesso

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
   <td> <p>Livello di accesso amministratore di sistema</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configura [!UICONTROL Gestione risorse] preferenze

>[!NOTE]
>
>Poiché si tratta di un’impostazione globale, questa selezione influisce su tutti i calcoli per l’intero sistema, per tutti gli utenti, in tutti gli strumenti di gestione delle risorse e per tutti i pool di risorse.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Fai clic su **[!UICONTROL Gestione risorse]**.
1. Selezionare uno dei metodi seguenti per calcolare la disponibilità degli utenti in [!DNL Workfront]:

   * **Pianificazione predefinita**: [!DNL Workfront] utilizza la pianificazione predefinita del sistema e il singolo FTE dell&#39;utente per calcolare le ore disponibili dell&#39;utente negli strumenti di gestione delle risorse.\

      Per ulteriori informazioni sulle pianificazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Per ulteriori informazioni sul valore dell’FTE utente, consulta  [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcola le ore disponibili di un utente utilizzando la seguente formula quando l’amministratore di Workfront sceglie la pianificazione predefinita:

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Esempio:**\
      Ad esempio, se la pianificazione predefinita è di 40 ore alla settimana e l’ETP nel profilo dell’utente è di 0,5, l’utente può lavorare 20 ore alla settimana.

      Se l’utente ha un’ora di inattività al giorno, le ore disponibili vengono calcolate come segue:

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

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

   * **Pianificazione dell&#39;utente**: [!DNL Workfront] utilizza la pianificazione dell’utente e la pianificazione predefinita del sistema per calcolare il valore FTE disponibile dell’utente negli strumenti di gestione delle risorse. Le ore disponibili vengono calcolate solo in base alla pianificazione dell’utente. Il valore dell’FTE dell’utente viene ignorato. Questa è l’impostazione predefinita.

      >[!NOTE]
      >
      >Se l’utente non è associato a una pianificazione, le ore disponibili per l’utente vengono calcolate utilizzando la pianificazione predefinita.

      L’FTE disponibile per l’utente viene calcolato dalla seguente formula:

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Esempio:** Ad esempio, se la pianificazione predefinita è di 40 ore a settimana e la pianificazione dell’utente è di 30 ore a settimana, l’ETP dell’utente sarà 0,75.

      Se l’utente dispone di 2 ore di inattività al giorno, l’ETP disponibile settimanalmente verrà calcolato come segue:

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Fai clic su **[!UICONTROL Salva]**.
