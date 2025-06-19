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
source-git-commit: f7cb314067d105d5534f4be356024aea8e8f9a28
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 8%

---

# Configurare gli aggiornamenti di sistema

<!-- Audited: 6/2025 -->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
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

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Determinare i campi [!DNL Workfront] tracciati per un tipo di oggetto

È possibile determinare quali informazioni [!DNL Workfront] tiene traccia quando gli utenti modificano le informazioni associate a un determinato tipo di oggetto nell&#39;intera interfaccia [!DNL Workfront]. A tale scopo, aggiungere o rimuovere i campi di cui si desidera tenere traccia in [!DNL Workfront] per il tipo di oggetto.

>[!NOTE]
>
>* [!DNL Workfront] non può tenere traccia e registrare gli aggiornamenti sui campi personalizzati calcolati.
>* Puoi personalizzare l’aggiornamento del sistema per progetti, attività, problemi, portfolio, programmi e utenti. Non è possibile personalizzare l&#39;aggiornamento di sistema per modelli, documenti o schede orario, ma [!DNL Workfront] registra gli aggiornamenti di sistema per questi oggetti.
>


### Aggiungi i campi di cui vuoi tenere traccia [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

È possibile aggiungere i campi di cui si desidera tenere traccia in [!DNL Workfront] per un particolare tipo di oggetto nell&#39;interfaccia [!DNL Workfront]. Quando gli utenti modificano le informazioni in tale campo, [!DNL Workfront] registra le informazioni sulla modifica come aggiornamento di sistema nell&#39;area [!UICONTROL Aggiornamenti] per l&#39;oggetto.

>[!NOTE]
>
>Nei feed di aggiornamento è possibile tenere traccia di un massimo di 300 campi incorporati e personalizzati. Se tieni traccia del numero massimo di campi e desideri tenere traccia di campi aggiuntivi non visualizzati nella scheda secondaria [!UICONTROL Tutti i campi], devi prima rimuovere alcuni dei campi tracciati per poter tenere traccia dei nuovi campi. Per ulteriori informazioni sulla rimozione dei campi dai campi di aggiornamento, vedere [Rimuovere i campi che non si desidera tenere traccia](#remove-fields-you-don-t-want-tracked).

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Interfaccia]**, quindi su **[!UICONTROL Aggiorna feed]**.
1. (Facoltativo) Nella scheda **Campi tracciati**, fai clic su una delle seguenti schede secondarie, a seconda dei tipi di campi che desideri tracciare nel feed di aggiornamento:

   * **Campi predefiniti**: visualizza un elenco di campi predefiniti.
   * **Campi personalizzati**: visualizza un elenco di campi personalizzati. È necessario creare i campi personalizzati prima che siano disponibili nell’elenco.
   * **Tutti i campi**: visualizza un elenco di campi predefiniti e personalizzati.

1. Fai clic su **[!UICONTROL Aggiungi campi]**, quindi seleziona l&#39;oggetto che desideri tracciare dal menu a discesa.

   La selezione manuale dei campi non è disponibile per tutti gli oggetti con un&#39;area Aggiornamenti.

   Selezionare i campi per i seguenti oggetti:

   * Progetto
   * Attività
   * Problema
   * Portfolio
   * Programma
   * Utente

   Viene visualizzata la casella **Aggiungi campi** per ogni oggetto selezionato.
1. Nella casella **Aggiungi campi**, inizia a digitare un campo predefinito (standard) o personalizzato per l&#39;oggetto, quindi selezionalo quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Se [!DNL Workfront] sta già tenendo traccia del campo, non è possibile aggiungerlo una seconda volta dall&#39;elenco.

1. Dopo aver aggiunto tutti i campi di cui si desidera tenere traccia in [!DNL Workfront], fare clic su **[!UICONTROL Aggiungi campi]**.
I campi incorporati aggiunti vengono visualizzati nella scheda secondaria **[!UICONTROL Campi incorporati]** e i campi personalizzati nella scheda secondaria **[!UICONTROL Campi personalizzati]**.
La scheda secondaria **[!UICONTROL Tutti i campi]** mostra sia i campi incorporati che quelli personalizzati di cui [!DNL Workfront] tiene traccia.

<!-- replace the above when releasing to Preview: 

1. In the panel on the left, click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.
1. (Optional) In the <span class="preview">**Tracked fields** tab</span>, click one of the following subtabs, depending on which types of fields you want to track in the update feed:

   * <span class="preview">**Built-in fields**</span>: Displays a list of built-in fields.
   * <span class="preview">**Custom fields**</span>: Displays a list of custom fields. You must create the custom fields before they are available in the list. 
   * <span class="preview">**All fields**</span>: Displays a list of both built-in and custom fields. 

1. Click <span class="preview">**[!UICONTROL Add fields]**,</span> then select the object that you want to be tracked from the drop-down. 

   Manually selecting fields is not available for all the objects that have an Updates area.

   Select from fields for the following objects:

      * Project
      * Task
      * Issue
      * Portfolio
      * Program
      * User

   The <span class="preview">**Add fields** </span> box opens, for each object selected.
1. In the <span class="preview">**Add fields** </span> box, start typing either a built-in (standard) field or a custom field for the object, then select it when it appears in the list.

   >[!NOTE]
   >
   >If [!DNL Workfront] is already tracking the field, you can't add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, <span class="preview"> click **[!UICONTROL Add]**.
   The built-in fields that you added show under the **[!UICONTROL Built-in fields]** subtab, and the custom fields show under the **[!UICONTROL Custom fields]** subtab.
   The **[!UICONTROL All fields]** subtab shows both the built-in and the custom fields that [!DNL Workfront] tracks.</span>

-->

### Rimuovi i campi che non desideri tracciare {#remove-fields-you-don-t-want-tracked}

È possibile rimuovere i campi di cui non si desidera tenere traccia per un particolare tipo di oggetto nell&#39;interfaccia [!DNL Workfront].

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Interfaccia]**, quindi su **[!UICONTROL Aggiorna feed]**.

1. Nella scheda **[!UICONTROL Campi tracciati]**, selezionare la scheda secondaria **[!UICONTROL Tutti i campi]**. Vengono visualizzati sia i campi incorporati che quelli personalizzati attualmente tracciati.

1. Seleziona il campo di cui vuoi interrompere il tracciamento, quindi fai clic su **[!UICONTROL Rimuovi]**.


<!--replace above at Preview release with this:

1. On the <span class="preview">**[!UICONTROL Tracked fields]** tab</span>, select the **[!UICONTROL All fields]** subtab. Both the built-in and custom fields that are currently being tracked display.

1. Select the field you want to stop tracking, then click the <span class="preview">**[!UICONTROL Remove]** icon ![Remove icon](assets/remove-icon.png).</span>

-->

1. Nella casella **[!UICONTROL Rimuovi campo]** visualizzata fare clic su **[!UICONTROL Sì, rimuovi]** per confermare.

   Eventuali aggiornamenti sui campi tracciati in precedenza vengono mantenuti nell&#39;area [!UICONTROL Aggiornamenti] in cui sono stati registrati.

## Determinare le azioni [!DNL Workfront] tracciate per un tipo di oggetto

È possibile avere [!DNL Workfront] azioni di tracciamento eseguite dagli utenti sugli oggetti nell&#39;interfaccia [!DNL Workfront].

Ad esempio, [!DNL Workfront] può registrare un aggiornamento ogni volta che un utente cambia un&#39;assegnazione a un&#39;attività o a un problema.

La modifica viene quindi visualizzata come aggiornamento del sistema nell&#39;area [!UICONTROL Aggiornamenti] per l&#39;attività o il problema.

Nella tabella seguente sono descritte le azioni che è possibile tenere traccia degli oggetti in [!DNL Workfront]:

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

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Interfaccia]**, quindi su **[!UICONTROL Aggiorna feed]**.

1. Fare clic sulla scheda **[!UICONTROL Azioni]**.

1. Seleziona la casella di controllo di un’azione per abilitarla o deselezionala per disabilitarla.
1. Fai clic su **[!UICONTROL Salva]**.

   Quando disattivi un&#39;azione, qualsiasi aggiornamento registrato in precedenza su tale azione viene mantenuto nell&#39;area [!UICONTROL Aggiornamenti] in cui è stato registrato. [!DNL Workfront] interrompe la registrazione di nuovi aggiornamenti per l&#39;azione disabilitata.
