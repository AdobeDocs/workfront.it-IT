---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurare gli aggiornamenti di sistema
description: Workfront genera aggiornamenti automatici di sistema nell'area [!UICONTROL Aggiornamenti] di un oggetto per registrare le modifiche eseguite dagli utenti sull'oggetto. In qualità di  [!DNL Workfront] amministratore, puoi configurare i campi oggetto e le azioni [!DNL Workfront] da monitorare per registrare gli aggiornamenti del sistema.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 8%

---

# Configurare gli aggiornamenti di sistema

[!DNL Adobe Workfront] genera aggiornamenti automatici di sistema nell&#39;area [!UICONTROL Aggiornamenti] di un oggetto per registrare i seguenti eventi:

* Modifiche apportate dagli utenti in un campo oggetto
* Azioni eseguite dagli utenti su un oggetto

Questi aggiornamenti di sistema includono i seguenti tipi di informazioni:

* La modifica apportata
* Nome dell&#39;utente che ha apportato la modifica
* Ora e data della modifica

Per ulteriori informazioni sugli aggiornamenti del sistema, vedere [Aggiornamenti monitorati dal sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

In qualità di amministratore [!DNL Workfront], puoi configurare i campi oggetto e le azioni [!DNL Workfront] di cui tenere traccia per registrare gli aggiornamenti di sistema.

Ad esempio, [!DNL Workfront] potrebbe tenere traccia di tutte le modifiche apportate dagli utenti ai nomi dei problemi nel sistema. Qualsiasi modifica del nome del problema viene quindi visualizzata come aggiornamento di sistema nell&#39;area [!UICONTROL Aggiornamenti] del problema.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   Oppure
   <p>Corrente: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Determinare i campi [!DNL Workfront] tracciati per un tipo di oggetto

È possibile determinare quali informazioni [!DNL Workfront] tiene traccia quando gli utenti modificano le informazioni associate a un determinato tipo di oggetto nell&#39;intera interfaccia [!DNL Workfront]. A tale scopo, aggiungere o rimuovere i campi di cui si desidera tenere traccia in [!DNL Workfront] per il tipo di oggetto.

>[!NOTE]
>
>* [!DNL Workfront] non è in grado di tenere traccia e registrare gli aggiornamenti sui campi personalizzati calcolati.
>* Puoi personalizzare l’aggiornamento del sistema per progetti, attività, problemi, portfolio, programmi e utenti. Non è possibile personalizzare l&#39;aggiornamento di sistema per modelli, documenti o schede orario, ma [!DNL Workfront] registra gli aggiornamenti di sistema per questi oggetti.
>



* [Aggiungi i campi di cui vuoi tenere traccia [!DNL Workfront] ](#add-fields-you-want-workfront-to-track)
* [Rimuovere i campi che non si desidera tracciare](#remove-fields-that-you-don-t-want-tracked)

### Aggiungi i campi di cui vuoi tenere traccia [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

È possibile aggiungere i campi di cui si desidera tenere traccia in [!DNL Workfront] per un particolare tipo di oggetto nell&#39;interfaccia [!DNL Workfront]. Quando gli utenti modificano le informazioni in tale campo, [!DNL Workfront] registra le informazioni sulla modifica come aggiornamento di sistema nell&#39;area [!UICONTROL Aggiornamenti] per l&#39;oggetto.

>[!NOTE]
>
>Nei feed di aggiornamento è possibile tenere traccia di un massimo di 300 campi incorporati e personalizzati. Se tieni traccia del numero massimo di campi e desideri tenere traccia di campi aggiuntivi non visualizzati nella scheda secondaria [!UICONTROL Tutti i campi], devi prima rimuovere alcuni dei campi tracciati per poter tenere traccia dei nuovi campi. Per ulteriori informazioni sulla rimozione dei campi dai campi di aggiornamento, vedere [Rimuovere i campi che non si desidera tenere traccia](#remove-fields-that-you-don-t-want-tracked).

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. &#x200B;Fare clic su **[!UICONTROL Aggiungi campi]**, quindi sull&#39;oggetto che si desidera tracciare.

1. Nella casella **[!UICONTROL Aggiorna feed]** visualizzata&#x200B; iniziare a digitare un campo predefinito (standard) o personalizzato per l&#39;oggetto, quindi fare clic su per selezionarlo quando viene visualizzato nell&#39;elenco.

   Se [!DNL Workfront] sta già tenendo traccia del campo, non è possibile aggiungerlo una seconda volta dall&#39;elenco.

1. Dopo aver aggiunto tutti i campi di cui si desidera tenere traccia in [!DNL Workfront], fare clic su **[!UICONTROL Aggiungi campi]**.

   I campi incorporati aggiunti vengono visualizzati nella scheda secondaria **[!UICONTROL Campi incorporati]**.

   I campi personalizzati aggiunti vengono visualizzati nella scheda secondaria **[!UICONTROL Campi personalizzati]**.

   La scheda secondaria **[!UICONTROL Tutti i campi]** mostra sia i campi incorporati che quelli personalizzati che vengono tracciati.

### Rimuovere i campi che non si desidera tracciare {#remove-fields-that-you-don-t-want-tracked}

È possibile rimuovere i campi di cui non si desidera tenere traccia per un particolare tipo di oggetto nell&#39;interfaccia [!DNL Workfront].

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

1. Fare clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Nella scheda **[!UICONTROL Campi tracciati]**, selezionare la scheda secondaria **[!UICONTROL Tutti i campi]**.

   Questo mostra sia i campi incorporati che quelli personalizzati che sono attualmente tracciati.

1. Selezionare il campo di cui si desidera interrompere il rilevamento, quindi fare clic su **[!UICONTROL Rimuovi]**.

1. Nella casella **[!UICONTROL Rimuovi campo]** visualizzata fare clic su **[!UICONTROL Sì, rimuovi]** per confermare.

Eventuali aggiornamenti sui campi tracciati in precedenza vengono mantenuti nell&#39;area [!UICONTROL Aggiornamenti] in cui sono stati registrati.

## Determinare le azioni [!DNL Workfront] tracciate per un tipo di oggetto

È possibile fare in modo che [!DNL Workfront] tenga traccia delle azioni seguenti che gli utenti possono eseguire sugli oggetti in tutta l&#39;interfaccia [!DNL Workfront].

Ad esempio, [!DNL Workfront] può registrare un aggiornamento ogni volta che un utente cambia un&#39;assegnazione a un&#39;attività o a un problema. La modifica viene quindi visualizzata come aggiornamento del sistema nell&#39;area [!UICONTROL Aggiornamenti] per l&#39;attività o il problema.

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

Per configurare le azioni di cui tenere traccia [!DNL Workfront]:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

1. Fare clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Fare clic sulla scheda **[!UICONTROL Azioni]**.

1. Seleziona un’azione per abilitarla o deseleziona un’azione per disabilitarla.
1. Fai clic su **[!UICONTROL Salva]**.

Quando disattivi un&#39;azione, qualsiasi aggiornamento registrato in precedenza su tale azione viene mantenuto nell&#39;area [!UICONTROL Aggiornamenti] in cui è stato registrato.
