---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti
description: Puoi creare filtri, viste e raggruppamenti predefiniti, quindi renderli disponibili agli utenti dell’organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puoi creare filtri, viste e raggruppamenti predefiniti, quindi renderli disponibili agli utenti dell’organizzazione.

Quando crei filtri, viste e raggruppamenti predefiniti come descritto in questo articolo, gli utenti con cui li condividi possono sfruttarli durante la visualizzazione dei loro elenchi. Gli utenti possono creare filtri, viste e raggruppamenti personalizzati in base a quelli creati, ma non possono modificare direttamente quelli creati.

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

## Creare filtri, viste o raggruppamenti predefiniti

{{step-1-to-setup}}

1. Effettua una delle seguenti operazioni, a seconda che tu stia creando o modificando un filtro, una vista o un raggruppamento:

   * Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Filtri]**.

   * Clic **[!UICONTROL Interfaccia] >** **[!UICONTROL Visualizzazioni]**.

   * Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Raggruppamenti]**.

1. Per creare un filtro, una visualizzazione o un raggruppamento, fare clic su **[!UICONTROL Aggiungi filtro]**, **[!UICONTROL Aggiungi visualizzazione]**, o **[!UICONTROL Aggiungi raggruppamento]**, quindi selezionare il tipo di oggetto a cui si desidera associare il nuovo filtro, la nuova visualizzazione o il nuovo raggruppamento.

   Oppure

   Se stai modificando un filtro, una visualizzazione o un raggruppamento esistente, selezionalo, quindi fai clic sul pulsante **[!UICONTROL Modifica]** icona ![Icona Modifica](assets/edit-icon.png).

1. Configura il filtro, la visualizzazione o il raggruppamento.

   Per informazioni sulle opzioni disponibili, consulta uno dei seguenti articoli:

   * [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Panoramica delle visualizzazioni in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Panoramica sui raggruppamenti in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Clic **[!UICONTROL Salva]** nell&#39;angolo inferiore sinistro.

È possibile rendere il filtro, la visualizzazione o il raggruppamento disponibili agli utenti del sistema. Per ulteriori informazioni sulla condivisione di filtri, viste o raggruppamenti con altri utenti, consulta la sezione [Rendere disponibili agli utenti filtri, visualizzazioni o raggruppamenti](#make-filters-views-or-groupings-available-to-users) in questo articolo.


## Mostrare o nascondere i filtri, le visualizzazioni o i raggruppamenti disponibili nel modello di layout

È possibile scegliere di mostrare o nascondere filtri, viste o raggruppamenti dal modello di layout. I filtri visibili sono disponibili per tutti gli utenti a livello di sistema. È possibile utilizzare un modello di layout per nascondere i filtri visibili per utenti o gruppi specifici.

>[!NOTE]
>
>Se un utente utilizza attivamente un filtro, una visualizzazione o un raggruppamento e poi un amministratore lo disabilita, l’utente può comunque accedervi finché non sceglie un nuovo filtro, una visualizzazione o un raggruppamento. Dopo aver scelto un nuovo filtro, una nuova vista o un nuovo raggruppamento, non sarà più possibile ripristinare il filtro, la vista o il raggruppamento nascosto.

Per mostrare o nascondere i filtri, le visualizzazioni o i raggruppamenti disponibili nel modello di layout:

1. Clic **[!UICONTROL Interfaccia]**, quindi fare clic su una delle opzioni seguenti: **[!UICONTROL Filtri]**, **[!UICONTROL Visualizzazioni]**, o **[!UICONTROL Raggruppamenti]**.

1. (Condizionale) Seleziona il filtro, la visualizzazione o il raggruppamento che desideri rendere disponibile agli utenti, quindi fai clic su **[!UICONTROL Abilita a livello di sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Se si desidera mantenere il filtro, la visualizzazione o il raggruppamento disponibili per la maggior parte degli utenti, ma nasconderli ad altri utenti, è possibile utilizzare il modello di layout. Per ulteriori informazioni, consulta [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condizionale) Seleziona il filtro, la visualizzazione o il raggruppamento che desideri nascondere agli utenti, quindi fai clic su **[!UICONTROL Disattiva a livello di sistema]**. Una volta disattivato, il filtro, la vista o il raggruppamento saranno nascosti dal modello di layout e dagli utenti nel sistema.


## Rendi filtri, viste o raggruppamenti disponibili a tutti gli utenti {#make-filters-views-or-groupings-available-to-users}

Questi passaggi spiegano come rendere disponibili filtri, viste e raggruppamenti da [!UICONTROL Condividi] finestra di dialogo in [!UICONTROL Interfaccia] area in [!UICONTROL Configurazione]. Questa impostazione funziona come un interruttore on/off per l’intero sistema, incluso il modello di layout.

{{step-1-to-setup}}

1. Clic **[!UICONTROL Interfaccia]**, quindi fare clic su una delle opzioni seguenti: **[!UICONTROL Filtri]**, **[!UICONTROL Visualizzazioni]**, o **[!UICONTROL Raggruppamenti]**.

1. Selezionare il filtro, la visualizzazione o il raggruppamento che si desidera rendere disponibile agli utenti, quindi fare clic sul pulsante **[!UICONTROL Condividi]** icona ![Icona Condividi](assets/share-icon.png) per aprire [!UICONTROL Filtra accesso], [!UICONTROL Accesso visualizzazione], o [!UICONTROL Accesso al raggruppamento] modulo.
1. (Condizionale) Per rendere il filtro, la visualizzazione o il raggruppamento disponibili a tutti gli utenti del sistema, fare clic sul pulsante **[!UICONTROL Ingranaggio]** menu a discesa ![](assets/gear-menu-for-sharing-items.png), quindi fai clic su **[!UICONTROL Rendi visibile a livello di sistema]**. Tutti gli utenti del sistema possono ora visualizzare il filtro, la vista o il raggruppamento.

   Oppure

   Inizia a digitare il nome di utenti, team, ruoli, gruppi o società specifici con cui condividere il filtro, la visualizzazione o il raggruppamento, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   Per ulteriori informazioni sulla condivisione, consulta [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Fai clic su **[!UICONTROL Salva]**.

   Gli utenti specificati possono ora visualizzare il filtro, la visualizzazione o il raggruppamento predefinito quando visualizzano il tipo di oggetto a cui è associato.

## Eliminare filtri, viste e raggruppamenti

{{step-1-to-setup}}

1. Effettua una delle seguenti operazioni, a seconda che tu stia eliminando un filtro, una vista o un raggruppamento:

   * Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Filtri]**

   * Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Visualizzazioni]**

   * Clic **[!UICONTROL Interfaccia]** > **[!UICONTROL Raggruppamenti]**

1. Seleziona uno o più elementi nell’elenco, quindi fai clic sul pulsante **[!UICONTROL Elimina]** icona ![Icona Elimina](assets/delete.png).
1. Per informazioni dettagliate sulla configurazione di un filtro, di una vista o di un raggruppamento, vedere uno degli articoli seguenti.

   * [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Panoramica delle visualizzazioni in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Panoramica sui raggruppamenti in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
