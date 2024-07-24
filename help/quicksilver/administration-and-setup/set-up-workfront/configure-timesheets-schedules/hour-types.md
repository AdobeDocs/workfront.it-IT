---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gestire i tipi di lavoro
description: È possibile associare i tipi di ore alle ore inserite. I tipi di ore sono etichette utilizzate per definire le ore inserite.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 212dda4289e4d29dbfbff0dbdc55315215b5ad91
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 1%

---

# Gestire i tipi di lavoro

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

È possibile associare i tipi di ore alle ore inserite. I tipi di ore sono etichette utilizzate per definire le ore inserite.

Esistono due set di tipi di ore:

* **Tipi di lavoro specifici per il progetto**: tempo impiegato per l&#39;accesso a progetti, attività e problemi. I tipi di lavoro specifici del progetto possono essere associati alle ore inserite in qualsiasi punto di [!DNL Adobe Workfront], dove è possibile registrare il tempo per progetti, attività e problemi.

  Quando si registra l&#39;ora in [!DNL Workfront], i tipi di ora specifici del progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente.

  Sono sempre disponibili i seguenti tipi di lavoro predefiniti specifici per il progetto:

   * Ore di Progetto
   * Ore di Attività
   * Tempo del problema

  L&#39;amministratore [!DNL Workfront] determina quali tipi di ore specifiche del progetto sono rese disponibili, come descritto in [Definire i tipi di ore e la disponibilità](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Se si abilita qualsiasi tipo di ora specifico del progetto nel sistema [!DNL Workfront], è necessario abilitare almeno un tipo di ora specifico del progetto in ogni progetto del sistema. Non è possibile abilitare un tipo di ora specifico per il progetto a livello di sistema e non sono disponibili tipi di ora specifici per il progetto a livello di progetto.

* **Tipi di lavoro generali**: le ore generali non possono essere associate a un progetto, un&#39;attività o un problema e vengono registrate direttamente in una scheda orario.

Per informazioni sulle ore di registrazione e sulla loro associazione ai tipi di ore, vedere [Tempo di registrazione](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano [!UICONTROL Adobe Workfront]</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p>
   <p>Corrente: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p> <p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipi di lavoro incorporati

Workfront viene fornito con un set di tipi di ora incorporati. Questi tipi di lavoro non possono essere modificati e non possono essere nascosti.

I tipi di ore forniti con [!DNL Workfront] sono:

* **[!UICONTROL Malattia]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Le ore di malattia non possono essere conteggiate come ricavi.
* **[!UICONTROL Ferie]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Il tempo di vacanza non può essere conteggiato come reddito.
* **[!UICONTROL Costi comuni generali]**: un tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Tuttavia, può essere conteggiato come ricavo nel processo di pianificazione del progetto.
* **[!UICONTROL Ora progetto]**: tipo di ora generale che può essere associato solo alle ore inserite in un progetto.
* **[!UICONTROL Ora attività]**: tipo di ora generale che può essere associato solo alle ore inserite in un&#39;attività.
* **[!UICONTROL Ora problema]**: tipo di ora generale che può essere associato solo alle ore inserite in un problema.

## Crea tipi di lavoro

In qualità di amministratore [!DNL Workfront], puoi creare nuovi tipi di lavoro per la tua organizzazione a livello sia di sistema che di progetto. Dopo aver creato i tipi di ore a livello di sistema e di progetto, gli utenti possono definire i tipi di ore disponibili per progetti e utenti specifici. Per ulteriori informazioni, vedere [Definire i tipi di ore e la disponibilità](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Per creare nuovi tipi di ore:

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Timesheet &amp; Hours]** > **[!UICONTROL Hour Types]**.

1. Fai clic su **[!UICONTROL Nuovo tipo di ora].**
1. Specifica le seguenti informazioni nel modulo **[!UICONTROL New Hour Type]**:

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
      <td> <p>Definisci se il tipo di ora è generale o specifico per il progetto selezionando l’ambito corretto nel menu a discesa.</p> <p>I tipi di lavoro generali sono visibili solo nelle schede orario e non possono essere associati a progetti, attività o problemi.</p> <p><b>IMPORTANTE</b>: se si dispone di un Tipo di Ora personalizzato che è [!UICONTROL Specifico per Progetto], modificarlo in [!UICONTROL Generale], tutte le Attività, i Problemi e le Ore di Progetto esistenti vengono impostate sui relativi tipi predefiniti di sistema.</p> </td> 
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

   **[!UICONTROL Conta come ricavi]**: selezionare questa opzione se si desidera che la voce delle ore associata a questo tipo di ore influisca sui calcoli dei ricavi.

1. Fai clic su **[!UICONTROL Crea tipo di lavoro].**

## Disattiva i tipi di lavoro

Se i tipi di ore diventano obsoleti e non si desidera più che gli utenti associno le ore immesse, è possibile disattivare i tipi di ore.

La disattivazione dei tipi di ora nasconde i tipi di ora in qualsiasi punto di [!DNL Workfront] in cui i tipi di ora sono visibili.

Per disattivare un tipo di ora:

{{step-1-to-setup}}

1. Espandi **[!UICONTROL Preferenze Ore e Timesheet]**, quindi fai clic su **[!UICONTROL Tipi di lavoro]**.

1. Selezionare il tipo di ora che si desidera disattivare.

1. Fare clic su **[!UICONTROL Disattiva]**.
