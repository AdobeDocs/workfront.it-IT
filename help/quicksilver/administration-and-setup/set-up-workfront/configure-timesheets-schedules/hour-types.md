---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gestire i tipi di lavoro
description: È possibile associare i tipi di ore alle ore inserite. I tipi di ore sono etichette utilizzate per definire le ore inserite.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Gestire i tipi di lavoro

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

È possibile associare i tipi di ore alle ore inserite. I tipi di ore sono etichette utilizzate per definire le ore inserite.

Esistono due set di tipi di ore:

* **Tipi di lavoro specifici per progetto**: tempo impiegato per l’accesso a progetti, attività e problemi. I tipi di ore specifici del progetto possono essere associati alle ore inserite ovunque in [!DNL Adobe Workfront] dove è possibile registrare il tempo per progetti, attività e problemi.

  Quando si effettua l’accesso [!DNL Workfront], i tipi di lavoro specifici per il progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente.

  Sono sempre disponibili i seguenti tipi di lavoro predefiniti specifici per il progetto:

   * Ore di Progetto
   * Ore di Attività
   * Tempo del problema

  Il [!DNL Workfront] l’amministratore determina quali tipi di ore specifici del progetto vengono resi disponibili, come descritto in [Definire i tipi di ore e la disponibilità per le schede orario](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Se si abilita qualsiasi tipo di ora specifica per il progetto nel [!DNL Workfront] di sistema, è necessario abilitare almeno un tipo di ora specifico per il progetto in ogni progetto del sistema. Non è possibile abilitare un tipo di ora specifico per il progetto a livello di sistema e non sono disponibili tipi di ora specifici per il progetto a livello di progetto.

* **Tipi di Ora Generali**: le ore generali non possono essere associate a un progetto, un’attività o un problema e vengono registrate direttamente in una scheda orario. Per ulteriori informazioni sull&#39;ora di registrazione, vedere [Tempo di connessione](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano [!UICONTROL Adobe Workfront]</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di lavoro incorporati

Workfront viene fornito con un set di tipi di ora incorporati. Questi tipi di lavoro non possono essere modificati e non possono essere nascosti.

I tipi di ora forniti con [!DNL Workfront] sono:

* **[!UICONTROL Ore Malattia]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Le ore di malattia non possono essere conteggiate come ricavi.
* **[!UICONTROL Tempo di vacanza]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Il tempo di vacanza non può essere conteggiato come reddito.
* **[!UICONTROL Costi generali]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Tuttavia, può essere conteggiato come ricavo nel processo di pianificazione del progetto.
* **[!UICONTROL Ora progetto]**: tipo di ora generale che può essere associato solo alle ore inserite in un progetto.
* **[!UICONTROL Ora attività]**: tipo di ora generale che può essere associato solo alle ore inserite in un&#39;attività.
* **[!UICONTROL Ora problema]**: tipo di ora generale che può essere associato solo alle ore inserite in un problema.

## Crea tipi di lavoro

As a [!DNL Workfront] amministratore, puoi creare nuovi tipi di ore per la tua organizzazione a livello di sistema e di progetto. Dopo aver creato i tipi di ore a livello di sistema e di progetto, gli utenti possono definire i tipi di ore disponibili per progetti e utenti specifici. Per ulteriori informazioni, vedere [Definire i tipi di ore e la disponibilità per le schede orario](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Per creare nuovi tipi di ore:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Timesheet e ore]** > **[!UICONTROL Tipi di Ora]**.

1. Clic **[!UICONTROL Nuovo Tipo di Ora].**
1. Specifica le seguenti informazioni su **[!UICONTROL Nuovo Tipo di Ora]** forma:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Assegna al nuovo tipo di ora un nome facilmente riconoscibile nel sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Aggiungi una descrizione per il tipo di ora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ambito]</td> 
      <td> <p>Definisci se il tipo di ora è generale o specifico per il progetto selezionando l’ambito corretto nel menu a discesa.</p> <p>I tipi di lavoro generali sono visibili solo nelle schede orario e non possono essere associati a progetti, attività o problemi.</p> <p><b>IMPORTANTE</b>: se hai un Tipo di Ora personalizzato che è [!UICONTROL Specifico del Progetto], poi lo cambi in [!UICONTROL Generale], tutte le Attività, i Problemi e le Ore del Progetto esistenti sono impostate sui loro tipi predefiniti di sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td><p>Selezionare questa opzione se si desidera che la voce relativa alle ore associata a questo tipo di ore influisca sui calcoli dei ricavi.</p>
      <p>Il tempo di malattia e il tempo di vacanza non possono essere conteggiati come ricavi.</p>
      <p><b>NOTA</b></p>
      <p>Quando i tipi di ore generali vengono conteggiati come ricavi, la tariffa di costo associata al profilo dell’utente che registra l’ora viene associata al costo orario.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Conta Come Reddito]**: seleziona questa opzione se desideri che la voce dell’ora associata a questo tipo di ora influisca sui calcoli dei ricavi.

1. Clic **[!UICONTROL Crea Tipo di Ora].**

## Disattiva i tipi di lavoro

Se i tipi di ore diventano obsoleti e non si desidera più che gli utenti associno le ore immesse, è possibile disattivare i tipi di ore.

La disattivazione dei tipi di ora nasconde i tipi di ora da qualsiasi punto di [!DNL Workfront] dove sono visibili i tipi di ora.

Per disattivare un tipo di ora:

1. Clic **[!UICONTROL Configurazione]** vicino all&#39;angolo superiore destro di [!DNL Adobe Workfront] sulla barra di navigazione globale.

1. Espandi **[!UICONTROL Preferenze Ore e Timesheet]**, quindi fai clic su **[!UICONTROL Tipi di Ora]**.

1. Selezionare il tipo di ora che si desidera disattivare.

1. Clic **[!UICONTROL Disattiva]**.
