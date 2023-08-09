---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurare gli aggiornamenti di sistema
description: Workfront genera aggiornamenti automatici di sistema nel [!UICONTROL Aggiornamenti] per registrare le modifiche apportate dagli utenti all'oggetto. As a [!DNL Workfront] dell'utente, è possibile configurare i campi oggetto e le azioni [!DNL Workfront] traccia per registrare gli aggiornamenti di sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 7%

---

# Configurare gli aggiornamenti di sistema

[!DNL Adobe Workfront] genera aggiornamenti automatici di sistema nel [!UICONTROL Aggiornamenti] per registrare i seguenti eventi:

* Modifiche apportate dagli utenti in un campo oggetto
* Azioni eseguite dagli utenti su un oggetto

Questi aggiornamenti di sistema includono la modifica apportata, il nome dell&#39;utente che ha apportato la modifica e l&#39;ora e la data della modifica.

Per ulteriori informazioni sugli aggiornamenti del sistema, vedere [Aggiornamenti monitorati dal sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

As a [!DNL Workfront] dell&#39;utente, è possibile configurare i campi oggetto e le azioni [!DNL Workfront] traccia per registrare gli aggiornamenti di sistema.

Ad esempio, potresti avere [!DNL Workfront] tenere traccia di tutte le modifiche apportate dagli utenti ai nomi dei problemi nel sistema. Qualsiasi modifica del nome del problema viene quindi visualizzata come aggiornamento di sistema sul [!UICONTROL Aggiornamenti] area.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determinare quali campi [!DNL Workfront] tracce per un tipo di oggetto

È possibile determinare quali informazioni [!DNL Workfront] tiene traccia di quando gli utenti modificano le informazioni associate a un determinato tipo di oggetto nell&#39;intero [!DNL Workfront] di rete. Per eseguire questa operazione, aggiungere o rimuovere i campi desiderati [!DNL Workfront] per tenere traccia di quel tipo di oggetto.

>[!NOTE]
>
>* [!DNL Workfront] non può tenere traccia e registrare gli aggiornamenti sui campi personalizzati calcolati.
>* Puoi personalizzare l’aggiornamento del sistema per progetti, attività, problemi, portfolio, programmi e utenti. Non è possibile personalizzare l&#39;aggiornamento di sistema per modelli, documenti o schede orario, ma [!DNL Workfront] registra gli aggiornamenti di sistema per questi oggetti.
>



* [Aggiungere i campi desiderati [!DNL Workfront] da tracciare](#add-fields-you-want-workfront-to-track)
* [Rimuovere i campi che non si desidera tracciare](#remove-fields-that-you-don-t-want-tracked)

### Aggiungere i campi desiderati [!DNL Workfront] da tracciare {#add-fields-you-want-workfront-to-track}

È possibile aggiungere i campi desiderati [!DNL Workfront] per tenere traccia di un particolare tipo di oggetto in tutto il [!DNL Workfront] di rete. Quando gli utenti modificano le informazioni in quel campo, [!DNL Workfront] registra le informazioni sulla modifica come aggiornamento di sistema in [!UICONTROL Aggiornamenti] dell&#39;oggetto.

>[!NOTE]
>
>Nei feed di aggiornamento è possibile tenere traccia di un massimo di 300 campi incorporati e personalizzati. Se tieni traccia del numero massimo di campi e desideri tenere traccia di campi aggiuntivi che non vengono visualizzati nel [!UICONTROL Tutti i campi] Scheda secondaria, per tenere traccia dei nuovi campi è innanzitutto necessario rimuovere alcuni campi tracciati. Per ulteriori informazioni sulla rimozione di campi dai campi di aggiornamento, vedere [Rimuovere i campi che non si desidera tracciare](#remove-fields-that-you-don-t-want-tracked).

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. &#x200B;Clic **[!UICONTROL Aggiungi campi]**, quindi fare clic sull&#39;oggetto da tracciare.

1. In&#x200B; **[!UICONTROL Aggiorna feed]** che viene visualizzata, inizia a digitare un campo predefinito (standard) o un campo personalizzato per l’oggetto, quindi fai clic su per selezionarlo quando viene visualizzato nell’elenco.

   Se [!DNL Workfront] sta già tracciando il campo, non puoi aggiungerlo una seconda volta dall’elenco.

1. Dopo aver aggiunto tutti i campi desiderati [!DNL Workfront] per tracciare, fai clic su **[!UICONTROL Aggiungi campi]**.

   I campi incorporati aggiunti vengono visualizzati in **[!UICONTROL Campi incorporati]** scheda secondaria.

   I campi personalizzati aggiunti vengono visualizzati in **[!UICONTROL Campi personalizzati]** scheda secondaria.

   Il **[!UICONTROL Tutti i campi]** scheda secondaria mostra sia i campi incorporati che quelli personalizzati che vengono tracciati.

### Rimuovere i campi che non si desidera tracciare {#remove-fields-that-you-don-t-want-tracked}

È possibile rimuovere i campi di cui non si desidera tenere traccia per un particolare tipo di oggetto in tutto il [!DNL Workfront] di rete.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Il giorno **[!UICONTROL Campi tracciati]** , seleziona la scheda **[!UICONTROL Tutti i campi]** scheda secondaria.

   Questo mostra sia i campi incorporati che quelli personalizzati che sono attualmente tracciati.

1. Seleziona il campo di cui vuoi interrompere il tracciamento, quindi fai clic su **[!UICONTROL Rimuovi]**.

1. In **[!UICONTROL Rimuovi campo]** visualizzata, fare clic su **[!UICONTROL Sì, rimuovi]** per confermare.

Eventuali aggiornamenti sui campi tracciati in precedenza vengono mantenuti nel [!UICONTROL Aggiornamenti] area in cui sono stati registrati.

## Determinare quali azioni [!DNL Workfront] tracce per un tipo di oggetto

Puoi avere [!DNL Workfront] tenere traccia delle azioni seguenti che gli utenti possono eseguire sugli oggetti in tutto il [!DNL Workfront] di rete.

Ad esempio, puoi avere [!DNL Workfront] registrare un aggiornamento ogni volta che un utente modifica un’assegnazione di un’attività o di un problema. La modifica viene quindi visualizzata come aggiornamento di sistema nel [!UICONTROL Aggiornamenti] dell’attività o del problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Azione</strong> </th> 
   <th><strong>Oggetti</strong> </th> 
   <th><strong>Stato predefinito</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Assegnazione cambiata</td> 
   <td>Attività, problemi</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Linea di base eliminata</td> 
   <td>Progetti</td> 
   <td> <p>Disabilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Record fatturazione creato o eliminato</td> 
   <td>Progetti</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Documento creato o eliminato</td> 
   <td>Progetti, attività, problemi, portafogli, programmi</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Spesa creata o eliminata</td> 
   <td>Progetti, attività</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Ora registrata o eliminata</td> 
   <td>Progetti, attività, problemi</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Problema eliminato</td> 
   <td>Progetti</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Attività eliminata</td> 
   <td>Progetti</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>L'accesso di un utente è cambiato</td> 
   <td>Progetti, attività, problemi, documenti, portafogli, programmi</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
  <tr> 
   <td>Abbona oggetto commento</td> 
   <td>Progetti, attività, problemi</td> 
   <td> <p>Abilitato</p> </td> 
  </tr> 
 </tbody> 
</table>

Per configurare le azioni desiderate [!DNL Workfront] per tenere traccia di:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Fai clic su **[!UICONTROL Azioni]** scheda.

1. Seleziona un’azione per abilitarla o deseleziona un’azione per disabilitarla.
1. Fai clic su **[!UICONTROL Salva]**.

Quando disattivi un’azione, eventuali aggiornamenti registrati in precedenza su tale azione vengono mantenuti in [!UICONTROL Aggiornamenti] area in cui è stato registrato.
