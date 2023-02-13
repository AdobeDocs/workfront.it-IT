---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti
description: Puoi creare filtri, viste e raggruppamenti predefiniti, quindi renderli disponibili agli utenti della tua organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puoi creare filtri, viste e raggruppamenti predefiniti, quindi renderli disponibili agli utenti della tua organizzazione.

Quando crei filtri, viste e raggruppamenti predefiniti come descritto in questo articolo, gli utenti con cui li condividi possono sfruttarli quando visualizzano i loro elenchi. Gli utenti possono creare filtri, visualizzazioni e raggruppamenti personalizzati in base a quelli creati, ma non possono modificarli direttamente.

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

## Creare filtri, viste o raggruppamenti predefiniti

{{step-1-to-setup}}

1. Effettua una delle seguenti operazioni, a seconda che tu stia creando o modificando un filtro, una visualizzazione o un raggruppamento:

   * Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Filtri]**.

   * Fai clic su **[!UICONTROL Interfaccia] >** **[!UICONTROL Viste]**.

   * Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Raggruppamenti]**.

1. Se stai creando un filtro, una visualizzazione o un raggruppamento, fai clic su **[!UICONTROL Aggiungi filtro]**, **[!UICONTROL Aggiungi visualizzazione]** oppure **[!UICONTROL Aggiungi raggruppamento]**, quindi selezionare il tipo di oggetto a cui si desidera associare il nuovo filtro, vista o raggruppamento.

   Oppure

   Se stai modificando un filtro, una visualizzazione o un raggruppamento esistente, selezionalo, quindi fai clic sul pulsante **[!UICONTROL Modifica]** icona ![Icona Modifica](assets/edit-icon.png).

1. Configura il filtro, la visualizzazione o il raggruppamento.

   Per informazioni sulle opzioni disponibili, consulta uno dei seguenti articoli:

   * [Panoramica dei filtri in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Panoramica delle visualizzazioni in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Panoramica sui raggruppamenti in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Fai clic su **[!UICONTROL Salva]** nell&#39;angolo in basso a sinistra.

Puoi rendere il filtro, la visualizzazione o il raggruppamento disponibili agli utenti nel sistema. Per ulteriori informazioni sulla condivisione di filtri, visualizzazioni o raggruppamenti con altri utenti, consulta la sezione . [Rendere disponibili agli utenti filtri, visualizzazioni o raggruppamenti](#make-filters-views-or-groupings-available-to-users) in questo articolo.


## Mostrare o nascondere filtri, viste o raggruppamenti disponibili nel modello di layout

È possibile scegliere di mostrare o nascondere filtri, viste o raggruppamenti dal modello di layout. I filtri visibili sono disponibili per tutti gli utenti a livello di sistema. È possibile utilizzare un modello di layout per nascondere i filtri visibili per utenti o gruppi specifici.

>[!NOTE]
>
>Se un utente utilizza attivamente un filtro, una visualizzazione o un raggruppamento e un amministratore lo disabilita, l&#39;utente dispone comunque dell&#39;accesso fino a quando non sceglie un nuovo filtro, visualizzazione o raggruppamento. Dopo aver scelto un nuovo filtro, visualizzazione o raggruppamento, non sarà più possibile ripristinare il filtro, la visualizzazione o il raggruppamento nascosti.

Per visualizzare o nascondere filtri, viste o raggruppamenti disponibili nel modello di layout:

1. Fai clic su **[!UICONTROL Interfaccia]**, quindi fai clic su una delle seguenti opzioni: **[!UICONTROL Filtri]**, **[!UICONTROL Viste]** oppure **[!UICONTROL Raggruppamenti]**.

1. (Condizionale) Seleziona il filtro, la visualizzazione o il raggruppamento che desideri rendere disponibile agli utenti, quindi fai clic su **[!UICONTROL Attiva a livello di sistema]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Se si desidera mantenere il filtro, la visualizzazione o il raggruppamento disponibili per la maggior parte degli utenti, ma nasconderlo ad altri, è possibile utilizzare il modello di layout. Per ulteriori informazioni, consulta [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Condizionale) Seleziona il filtro, la visualizzazione o il raggruppamento da nascondere agli utenti, quindi fai clic su **[!UICONTROL Disattiva a livello di sistema]**. Una volta disattivato, il filtro, la visualizzazione o il raggruppamento verranno nascosti dal modello di layout e dagli utenti in tutto il sistema.


## Rendere disponibili filtri, visualizzazioni o raggruppamenti per tutti gli utenti {#make-filters-views-or-groupings-available-to-users}

Questi passaggi spiegano come rendere disponibili filtri, visualizzazioni e raggruppamenti dalla sezione [!UICONTROL Condividi] nella finestra di dialogo [!UICONTROL Interfaccia] area [!UICONTROL Configurazione]. Questa impostazione funziona come un interruttore on/off per l’intero sistema, incluso il modello di layout.

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Interfaccia]**, quindi fai clic su una delle seguenti opzioni: **[!UICONTROL Filtri]**, **[!UICONTROL Viste]** oppure **[!UICONTROL Raggruppamenti]**.

1. Seleziona il filtro, la visualizzazione o il raggruppamento che desideri rendere disponibili agli utenti, quindi fai clic sul pulsante **[!UICONTROL Condividi]** icona ![Icona Condividi](assets/share-icon.png) per aprire [!UICONTROL Accesso filtro], [!UICONTROL Visualizza accesso]oppure [!UICONTROL Accesso al raggruppamento] modulo.
1. (Condizionale) Per rendere disponibile il filtro, la visualizzazione o il raggruppamento a tutti gli utenti del sistema, fai clic sul pulsante **[!UICONTROL Ingranaggio]** menu a discesa ![](assets/gear-menu-for-sharing-items.png), quindi fai clic su **[!UICONTROL Rendere visibile il sistema a livello di sistema]**. Ora tutti gli utenti del sistema possono visualizzare il filtro, la visualizzazione o il raggruppamento.

   Oppure

   Inizia a digitare il nome di utenti, team, ruoli, gruppi o aziende specifici con cui condividere il filtro, la visualizzazione o il raggruppamento, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   Per ulteriori informazioni sulla condivisione, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Fai clic su **[!UICONTROL Salva]**.

   Gli utenti specificati possono ora visualizzare il filtro, la visualizzazione o il raggruppamento predefiniti quando visualizzano il tipo di oggetto a cui è stato associato.

## Eliminare filtri, visualizzazioni e raggruppamenti

{{step-1-to-setup}}

1. Effettua una delle seguenti operazioni, a seconda che si stia eliminando un filtro, una visualizzazione o un raggruppamento:

   * Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Filtri]**

   * Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Viste]**

   * Fai clic su **[!UICONTROL Interfaccia]** > **[!UICONTROL Raggruppamenti]**

1. Seleziona uno o più elementi nell’elenco, quindi fai clic sul pulsante **[!UICONTROL Elimina]** icona ![Icona Elimina](assets/delete.png).
1. Per informazioni dettagliate sulla configurazione di un filtro, di una visualizzazione o di un raggruppamento, consulta uno degli articoli seguenti.

   * [Panoramica dei filtri in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Panoramica delle visualizzazioni in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Panoramica sui raggruppamenti in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
