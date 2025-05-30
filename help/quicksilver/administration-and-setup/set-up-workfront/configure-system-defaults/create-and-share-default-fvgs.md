---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare, modificare e condividere filtri, visualizzazioni e raggruppamenti a livello di sistema
description: Puoi creare filtri, viste e raggruppamenti predefiniti, quindi renderli disponibili agli utenti dell’organizzazione.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 4fbf88c544cd56887e6f6f36d7aabfa0668a2a05
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Creare, modificare e condividere filtri, viste e raggruppamenti a livello di sistema

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puoi creare filtri, viste e raggruppamenti e renderli disponibili agli utenti a livello di sistema all’interno della tua organizzazione.

Quando crei filtri, viste e raggruppamenti a livello di sistema come descritto in questo articolo, gli utenti con cui li condividi possono sfruttarli durante la visualizzazione dei loro elenchi. Gli utenti possono creare filtri, viste e raggruppamenti personalizzati in base a quelli creati, ma non possono modificarli direttamente.

Tieni presente che i filtri, le viste e i raggruppamenti creati a livello di sistema sono diversi da quelli predefiniti creati automaticamente da Adobe Workfront. Impossibile modificare o eliminare i filtri, le visualizzazioni e i raggruppamenti predefiniti.

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
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare filtri, viste o raggruppamenti

{{step-1-to-setup}}


1. Fai clic su **[!UICONTROL Interfaccia]**, quindi su uno dei seguenti elementi: **[!UICONTROL Filtri]**, **[!UICONTROL Visualizzazioni]** o **[!UICONTROL Raggruppamenti]**.

1. Se stai creando un filtro, una visualizzazione o un raggruppamento, fai clic su **[!UICONTROL Aggiungi filtro]**, **[!UICONTROL Aggiungi visualizzazione]** o **[!UICONTROL Aggiungi raggruppamento]**, quindi seleziona il tipo di oggetto a cui vuoi associare il nuovo filtro, la nuova visualizzazione o il nuovo raggruppamento.

   Oppure

   Se stai modificando un filtro, una visualizzazione o un raggruppamento esistente, selezionalo, quindi fai clic sull&#39;icona **[!UICONTROL Modifica]** ![Modifica icona](assets/edit-icon.png).

1. Configura il filtro, la visualizzazione o il raggruppamento.

   Per informazioni sulle opzioni disponibili, consulta uno dei seguenti articoli:

   * [Panoramica filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Panoramica delle visualizzazioni in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Panoramica sui raggruppamenti in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo inferiore sinistro.

È possibile rendere il filtro, la visualizzazione o il raggruppamento disponibili agli utenti del sistema. Per ulteriori informazioni sulla condivisione di filtri, visualizzazioni o raggruppamenti con altri utenti, vedere la sezione [Rendere disponibili agli utenti filtri, visualizzazioni o raggruppamenti](#make-filters-views-or-groupings-available-to-users) in questo articolo.


## Rendi filtri, viste o raggruppamenti disponibili a tutti gli utenti {#make-filters-views-or-groupings-available-to-users}

È possibile scegliere di mostrare o nascondere filtri, viste o raggruppamenti nel sistema. I filtri visibili sono disponibili per tutti gli utenti del sistema. Questa impostazione funziona come un interruttore on/off per l’intero sistema, incluso il modello di layout.

Per nascondere filtri, viste o raggruppamenti a utenti specifici, è consigliabile utilizzare un modello di layout anziché disattivarli a livello di sistema.

>[!NOTE]
>
>* Se un utente utilizza attivamente un filtro, una visualizzazione o un raggruppamento e poi un amministratore lo disabilita, l’utente può comunque accedervi finché non sceglie un nuovo filtro, una visualizzazione o un raggruppamento. Dopo averne scelto uno nuovo, non potranno più tornare a quello nascosto.
>* Se tutti i filtri, le viste e i raggruppamenti sono limitati tramite il modello di layout o disabilitati a livello di sistema, l’utente visualizzerà le opzioni predefinite, in quanto il sistema deve visualizzare qualcosa.

Per mostrare o nascondere filtri, viste o raggruppamenti:

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Interfaccia]**, quindi su uno dei seguenti elementi: **[!UICONTROL Filtri]**, **[!UICONTROL Visualizzazioni]** o **[!UICONTROL Raggruppamenti]**.

1. (Condizionale) Selezionare il filtro, la visualizzazione o il raggruppamento che si desidera rendere disponibile agli utenti, quindi fare clic su **[!UICONTROL Abilita a livello di sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Se si desidera mantenere il filtro, la visualizzazione o il raggruppamento disponibili per la maggior parte degli utenti, ma nasconderli ad altri, è possibile utilizzare il modello di layout. Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condizionale) Selezionare il filtro, la visualizzazione o il raggruppamento che si desidera nascondere agli utenti, quindi fare clic su **[!UICONTROL Disattiva a livello di sistema]**. Il filtro, la visualizzazione o il raggruppamento ora sono nascosti sia dal modello di layout che dagli utenti nel sistema.


## Condividere filtri, visualizzazioni o raggruppamenti personalizzati con utenti specifici

Questi passaggi spiegano come condividere filtri, visualizzazioni e raggruppamenti personalizzati con utenti specifici utilizzando la finestra di dialogo di condivisione nell&#39;area [!UICONTROL Interfaccia] in [!UICONTROL Configurazione]. È possibile concedere l&#39;accesso in visualizzazione o in gestione a filtri, viste e raggruppamenti creati dall&#39;utente o da altri utenti. Non è possibile condividere i valori predefiniti di sistema con gli utenti.


{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Interfaccia]**, quindi su uno dei seguenti elementi: **[!UICONTROL Filtri]**, **[!UICONTROL Visualizzazioni]** o **[!UICONTROL Raggruppamenti]**.

1. Seleziona il filtro, la visualizzazione o il raggruppamento che desideri condividere, quindi fai clic sull&#39;icona **[!UICONTROL Condividi]** ![Condividi icona](assets/share-icon.png).
1. Inizia a digitare il nome di utenti, team, ruoli, gruppi o società specifici con cui condividere il filtro, la visualizzazione o il raggruppamento, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   Per ulteriori informazioni sulla condivisione, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Scegli **Visualizza** o **Gestisci** accanto al nome dell&#39;utente, del team, della mansione, del gruppo o della società. Per ottimizzare le autorizzazioni, fai clic sull’icona del cursore e regola le autorizzazioni.

   ![perfezionare le autorizzazioni](assets/fine-tune-permissions.png)

1. Fai clic su **[!UICONTROL Salva]**. Gli utenti specificati possono ora interagire con il filtro, la visualizzazione o il raggruppamento quando visualizzano il tipo di oggetto a cui è associato.


## Eliminare filtri, viste e raggruppamenti

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Interfaccia]**, quindi su uno dei seguenti elementi: **[!UICONTROL Filtri]**, **[!UICONTROL Visualizzazioni]** o **[!UICONTROL Raggruppamenti]**.

1. Seleziona uno o più elementi nell&#39;elenco, quindi fai clic sull&#39;icona **[!UICONTROL Elimina]** ![Elimina](assets/delete.png).

1. Nella finestra di dialogo **Elimina** visualizzata, fare clic su **Sì, Elimina**.
