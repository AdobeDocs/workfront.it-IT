---
title: Configurare la mappatura dei metadati
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: I metadati sono informazioni descrittive associate a un documento. Puoi impostare  [!DNL Adobe Workfront]  per includere metadati con documenti inviati ad  [!DNL Workfront]  applicazioni.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# Configurare la mappatura dei metadati

I metadati sono informazioni descrittive associate a un documento. È possibile configurare [!DNL Adobe Workfront] per includere metadati con documenti inviati alle applicazioni [!DNL Workfront].

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
   <td> <p>Devi essere un amministratore [!DNL Workfront]. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sui metadati [!DNL Workfront]

I metadati per i documenti in [!DNL Workfront] possono includere informazioni quali il nome del progetto, la descrizione dell&#39;attività o la data di completamento pianificata correlati. In qualità di amministratore di [!DNL Workfront], puoi configurare [!DNL Workfront] per includere metadati con documenti inviati da [!DNL Workfront] alle seguenti applicazioni [!DNL Workfront]:

* [!DNL Workfront DAM]

Prima di poter inviare i metadati con i documenti, è necessario specificare o mappare i metadati che si desidera includere. È possibile mappare qualsiasi campo utilizzato in [!DNL Workfront]. Dopo aver configurato la mappatura dei metadati, tutti i documenti caricati in un&#39;applicazione [!DNL Workfront] includeranno i metadati mappati.

Quando un utente invia un documento da [!DNL Workfront] a un&#39;applicazione [!DNL Workfront], i metadati mappati vengono trasferiti lungo il documento. Mentre la versione del documento nell&#39;applicazione [!DNL Workfront] è collegata a [!DNL Workfront], le modifiche apportate ai metadati del documento in [!DNL Workfront] non vengono applicate ai metadati del documento nell&#39;applicazione [!DNL Workfront]. Se un campo mappato in [!DNL Workfront] viene modificato, è necessario inviare una nuova versione del documento con i metadati aggiornati all&#39;applicazione [!DNL Workfront].

>[!NOTE]
>
>È possibile mappare i metadati solo in una direzione: da [!DNL Workfront] a [!DNL Workfront DAM]. Impossibile trasferire in Workfront i metadati per i documenti collegati a [!DNL Workfront] da [!DNL Workfront DAM].

È possibile mappare lo stesso campo [!DNL Workfront] a vari campi di metadati in [!DNL Workfront DAM], ma non è possibile utilizzare un campo di metadati in nessuna di queste applicazioni per più campi di metadati [!DNL Workfront].

Per configurare più campi [!DNL Workfront] da esportare in un campo di metadati in un&#39;applicazione [!DNL Workfront], creare innanzitutto un campo personalizzato calcolato in [!DNL Workfront] per visualizzare tutti i singoli campi personalizzati di un oggetto. Quindi, mappare il campo [!DNL Workfront] calcolato a un campo di metadati nell&#39;applicazione [!DNL Workfront]. Per ulteriori informazioni sui campi personalizzati calcolati, vedere [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Prima di poter mappare i campi per il processo di mappatura dei metadati, è necessario abilitare l&#39;applicazione in [!DNL Workfront]. Per ulteriori informazioni, vedere [Configurare le integrazioni dei documenti](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configura [!DNL Workfront] per inviare metadati

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

   ![](assets/metadata-mapping.png)

1. Nella casella **[!UICONTROL Seleziona campo Source per mappatura]**, inizia a digitare il nome del campo Workfront che desideri mappare a [!DNL Workfront DAM], quindi selezionalo quando lo visualizzi nell&#39;elenco.
1. Nella casella **[!UICONTROL Seleziona campo di destinazione per mappatura]**, selezionare il campo che si desidera compilare con le informazioni nel campo [!DNL Workfront] selezionato.

1. Fare clic su **[!UICONTROL Aggiungi mapping]**.

   Il campo mappato viene visualizzato nei campi mappati elencati nella parte inferiore della pagina.

1. Ripetere i passaggi 5 e 6 fino ad aggiungere tutti i campi [!DNL Workfront] desiderati e i campi [!DNL Workfront DAM] corrispondenti.

## Elimina campi mappati

1. Accedere a [!DNL Workfront] come amministratore.
1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

1. Nell&#39;elenco dei campi mappati selezionare i campi che si desidera rimuovere dalla mappatura dei metadati.
1. Fare clic su **[!UICONTROL Elimina]**.

   I campi designati non vengono più mappati. Ora, quando un utente invia un documento da [!DNL Workfront] a [!DNL Workfront DAM], i metadati contenuti nei campi eliminati non vengono trasferiti con il documento.

   Un documento inviato prima dell&#39;eliminazione dei campi mappati mantiene i metadati originali inviati con esso, inclusi i metadati per i campi eliminati.
