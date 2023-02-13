---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurare gli aggiornamenti di sistema
description: Workfront genera aggiornamenti automatici di sistema in un oggetto [!UICONTROL Aggiornamenti] per registrare le modifiche apportate dall'utente all'oggetto. Come [!DNL Workfront] amministratore, è possibile configurare i campi e le azioni oggetto [!DNL Workfront] traccia per registrare gli aggiornamenti del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# Configurare gli aggiornamenti di sistema

[!DNL Adobe Workfront] genera aggiornamenti automatici di sistema in un oggetto [!UICONTROL Aggiornamenti] area per registrare i seguenti eventi:

* Modifica le modifiche apportate dagli utenti in un campo oggetto
* Azioni eseguite dagli utenti su un oggetto

Questi aggiornamenti di sistema includono la modifica apportata, il nome dell’utente che ha apportato la modifica e l’ora e la data della modifica.

Come [!DNL Workfront] amministratore, è possibile configurare i campi e le azioni oggetto [!DNL Workfront] traccia per registrare gli aggiornamenti del sistema.

Ad esempio, [!DNL Workfront] tiene traccia di tutte le modifiche apportate dagli utenti ai nomi dei problemi in tutto il sistema. Qualsiasi modifica del nome del problema viene visualizzata come un aggiornamento del sistema sul [!UICONTROL Aggiornamenti] area.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determinare quali campi [!DNL Workfront] traccia un tipo di oggetto

È possibile determinare quali informazioni [!DNL Workfront] tiene traccia quando gli utenti modificano le informazioni associate a un determinato tipo di oggetto per l&#39;intero [!DNL Workfront] interfaccia. Per eseguire questa operazione, aggiungere o rimuovere i campi desiderati [!DNL Workfront] per tenere traccia del tipo di oggetto specificato.

>[!NOTE]
>
>* [!DNL Workfront] impossibile tenere traccia e registrare gli aggiornamenti sui campi personalizzati calcolati.
>* Puoi personalizzare l’aggiornamento del sistema per progetti, attività, problemi, portfolio, programmi e utenti. Non è possibile personalizzare l&#39;aggiornamento del sistema per modelli, documenti o fogli presenze, ma [!DNL Workfront] registra gli aggiornamenti del sistema per questi oggetti.
>




* [Aggiungi i campi desiderati [!DNL Workfront] tracciare](#add-fields-you-want-workfront-to-track)
* [Rimuovere i campi che non si desidera tracciare](#remove-fields-that-you-don-t-want-tracked)

### Aggiungi i campi desiderati [!DNL Workfront] tracciare {#add-fields-you-want-workfront-to-track}

È possibile aggiungere i campi desiderati [!DNL Workfront] per tenere traccia di un particolare tipo di oggetto in tutta la [!DNL Workfront] interfaccia. Quando gli utenti modificano le informazioni in quel campo, [!DNL Workfront] registra informazioni sulla modifica come aggiornamento del sistema nella [!UICONTROL Aggiornamenti] area dell&#39;oggetto.

>[!NOTE]
>
>Puoi tenere traccia fino a 300 campi incorporati e personalizzati nei feed di aggiornamento. Se tieni traccia del numero massimo di campi e desideri tenere traccia di campi aggiuntivi che non vengono visualizzati nella [!UICONTROL Tutti i campi] Sottoscheda, devi prima rimuovere alcuni dei campi tracciati per tenere traccia dei nuovi campi. Per ulteriori informazioni sulla rimozione dei campi dai campi di aggiornamento, vedi [Rimuovere i campi che non si desidera tracciare](#remove-fields-that-you-don-t-want-tracked).

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Clic &#x200B; **[!UICONTROL Aggiungi campi]**, quindi fare clic sull&#39;oggetto da tracciare.

1. Nel &#x200B; **[!UICONTROL Aggiorna feed]** casella visualizzata, inizia a digitare un campo predefinito (standard) o un campo personalizzato per l’oggetto, quindi fai clic su per selezionarlo quando viene visualizzato nell’elenco.

   Se [!DNL Workfront] sta già tracciando il campo, non puoi aggiungerlo una seconda volta dall’elenco.

1. Dopo aver aggiunto tutti i campi desiderati [!DNL Workfront] per tenere traccia, fai clic su **[!UICONTROL Aggiungi campi]**.

   I campi incorporati aggiunti vengono visualizzati nella sezione **[!UICONTROL Campi incorporati]** sottoscheda .

   I campi personalizzati aggiunti vengono visualizzati nella sezione **[!UICONTROL Campi personalizzati]** sottoscheda .

   La **[!UICONTROL Tutti i campi]** la sottoscheda mostra i campi incorporati e personalizzati che vengono tracciati.

### Rimuovere i campi che non si desidera tracciare {#remove-fields-that-you-don-t-want-tracked}

È possibile rimuovere i campi che non si desidera che il sistema tenga traccia di un particolare tipo di oggetto in tutto il [!DNL Workfront] interfaccia.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Sulla **[!UICONTROL Campi tracciati]** seleziona la scheda **[!UICONTROL Tutti i campi]** sottoscheda .

   Mostra i campi incorporati e personalizzati attualmente in corso di tracciamento.

1. Seleziona il campo da interrompere, quindi fai clic su **[!UICONTROL Rimuovi]**.

1. In **[!UICONTROL Rimuovi campo]** casella visualizzata, fai clic su **[!UICONTROL Sì, Rimuovi]** per confermare.

Eventuali aggiornamenti relativi ai campi tracciati in precedenza vengono mantenuti nella sezione [!UICONTROL Aggiornamenti] area in cui sono stati registrati.

## Determinare quali azioni [!DNL Workfront] traccia un tipo di oggetto

Può [!DNL Workfront] tenere traccia delle seguenti azioni che gli utenti possono eseguire sugli oggetti in tutta la [!DNL Workfront] interfaccia.

Ad esempio, puoi avere [!DNL Workfront] registra un aggiornamento ogni volta che un utente modifica un&#39;assegnazione a un&#39;attività o a un problema. La modifica viene quindi visualizzata come un aggiornamento del sistema nel [!UICONTROL Aggiornamenti] area dell&#39;attività o del problema.

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
   <td>Record di fatturazione creato o eliminato</td> 
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

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Aggiorna feed]**.

1. Fai clic sul pulsante **[!UICONTROL Azioni]** scheda .

1. Seleziona un’azione per attivarla o deseleziona un’azione per disattivarla.
1. Fai clic su **[!UICONTROL Salva]**.

Quando disattivi un’azione, qualsiasi aggiornamento registrato in precedenza relativo a tale azione viene mantenuto nel [!UICONTROL Aggiornamenti] area in cui è stato registrato.
