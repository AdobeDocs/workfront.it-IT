---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gestione dei tipi di ora
description: È possibile associare i tipi di ora alle voci dell'ora. I tipi di ora sono etichette utilizzate per definire le voci orarie.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Gestione dei tipi di ora

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

È possibile associare i tipi di ora alle voci dell&#39;ora. I tipi di ora sono etichette utilizzate per definire le voci orarie.

Esistono due set di tipi di ora:

* **Tipi di ora specifici del progetto**: Si tratta di progetti, attività e problemi registrati nel tempo. I tipi di ora specifici del progetto possono essere associati alle voci orarie in qualsiasi punto [!DNL Adobe Workfront] in cui è possibile registrare il tempo per progetti, attività e problemi.

   Durante l&#39;accesso [!DNL Workfront], i tipi di ora specifici per il progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente.

   Sono sempre disponibili i seguenti tipi di ora predefiniti per specifici progetti:

   * Ore di Progetto
   * Ore di Attività
   * Ore problema

   La [!DNL Workfront] l’amministratore determina quali tipi di ora specifici del progetto vengono resi disponibili, come descritto in [Definire i tipi di ora e la disponibilità per i fogli presenze](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >Se attivi qualsiasi tipo di ora specifico per il progetto nel [!DNL Workfront] in ogni progetto del sistema deve essere abilitato almeno un tipo di ora specifico per il progetto. Non è possibile abilitare un tipo di ora specifico per il progetto a livello di sistema e non sono disponibili tipi di ora specifici per il progetto a livello di progetto.

* **Tipi di ora generali**: Le ore generali non possono essere associate a un progetto, un&#39;attività o un problema e vengono registrate direttamente in una scheda attività. Per ulteriori informazioni sul tempo di registrazione, vedi [Tempo di log](../../../timesheets/create-and-manage-timesheets/log-time.md).

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di ora incorporati

Workfront viene fornito con un set di tipi di ora incorporati. Non è possibile modificare questi tipi di ora e non è possibile nasconderli.

I tipi di ora che vengono con [!DNL Workfront] sono:

* **[!UICONTROL Ora legale]**: Tipo di ora generale che non può essere associato alle voci orarie in un progetto, un&#39;attività o un problema.
* **[!UICONTROL Tempo di vacanza]**: Tipo di ora generale che non può essere associato alle voci orarie in un progetto, un&#39;attività o un problema.
* **[!UICONTROL Residenti nazionali]**: Tipo di ora generale che non può essere associato alle voci orarie in un progetto, un&#39;attività o un problema. Tuttavia, può essere conteggiato come ricavo nel processo di pianificazione del progetto.
* **[!UICONTROL Ora del progetto]**: Tipo di ora generale che può essere associato solo alle voci orarie di un progetto.
* **[!UICONTROL Ora attività]**: Tipo di ora generale che può essere associato solo alle voci orarie di un&#39;attività.
* **[!UICONTROL Ora del problema]**:Tipo di ora generale che può essere associato solo alle voci di ora in un problema.

## Crea tipi di ora

Come [!DNL Workfront] amministratore, puoi creare nuovi tipi di ora per la tua organizzazione a livello di sistema e di progetto. Dopo aver creato tipi di ora a livello di sistema e di progetto, gli utenti possono definire quali tipi di ora sono disponibili per progetti e utenti specifici. Per ulteriori informazioni, consulta la sezione [Definire i tipi di ora e la disponibilità per i fogli presenze](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Per creare nuovi tipi di ora:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Scheda attività e ore]** > **[!UICONTROL Tipi di ore]**.

1. Fai clic su **[!UICONTROL Nuovo tipo ora].**
1. Specifica le seguenti informazioni sul **[!UICONTROL Nuovo tipo ora]** modulo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Assegnare alla nuova ora un nome facilmente riconoscibile nel sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Aggiungi una descrizione per il tipo di ora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ambito [!UICONTROL]</td> 
      <td> <p>Definisci se il tipo di ora è un tipo di ora generale o specifico per il progetto selezionando l’ambito corretto nel menu a discesa.</p> <p>I tipi di ora generale sono visibili solo nei fogli presenze e non possono essere associati a progetti, attività o problemi.</p> <p><b>IMPORTANTE</b>: Se si dispone di un tipo di ora personalizzato specifico per il progetto, lo si cambia in Generale, tutti gli orari esistenti per l'attività, i problemi e il progetto vengono impostati sui tipi predefiniti di sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Conta Come Ricavo]</td> 
      <td>Selezionare questa opzione se si desidera che l'ora associata a questo tipo di ora influisca sui calcoli dei ricavi.</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Conteggio come ricavi]**: Selezionare questa opzione se si desidera che l&#39;ora associata a questo tipo di ora influisca sui calcoli dei ricavi.

1. Fai clic su **[!UICONTROL Crea tipo ora].**

## Disattiva i tipi di ora

Se i tipi di ora diventano obsoleti e non si desidera più che gli utenti associino le loro voci orarie, è possibile disattivare i tipi di ora.

La disattivazione dei tipi di ora nasconde i tipi di ora da qualsiasi punto [!DNL Workfront] dove sono visibili i tipi di ora.

Per disattivare un tipo ora:

1. Fai clic su **[!UICONTROL Configurazione]** vicino all&#39;angolo superiore destro di [!DNL Adobe Workfront] sulla barra di navigazione globale.

1. Espandi **[!UICONTROL Preferenze scheda attività e ora]**, quindi fai clic su **[!UICONTROL Tipi di ore]**.

1. Seleziona il tipo di ora da disattivare.

1. Fai clic su **[!UICONTROL Disattiva]**.
