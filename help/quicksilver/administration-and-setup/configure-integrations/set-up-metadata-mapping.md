---
title: Impostare la mappatura dei metadati
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: I metadati sono informazioni descrittive associate a un documento. È possibile impostare [!DNL Adobe Workfront] per includere metadati con documenti inviati a [!DNL Workfront] applicazioni.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Impostare la mappatura dei metadati

I metadati sono informazioni descrittive associate a un documento. È possibile impostare [!DNL Adobe Workfront] per includere metadati con documenti inviati a [!DNL Workfront] applicazioni.

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
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni su [!DNL Workfront] metadati

Metadati per i documenti in [!DNL Workfront] può includere informazioni quali il nome del progetto correlato, la descrizione dell’attività o la data di completamento pianificata. As a [!DNL Workfront] amministratore, puoi configurare [!DNL Workfront] per includere metadati con documenti inviati da [!DNL Workfront] ai seguenti [!DNL Workfront] applicazioni:

* [!DNL Workfront DAM]

Prima di poter inviare i metadati con i documenti, è necessario specificare o mappare i metadati che si desidera includere. Puoi mappare qualsiasi campo utilizzato in [!DNL Workfront]. Una volta impostata la mappatura dei metadati, tutti i documenti vengono caricati in un [!DNL Workfront] L&#39;applicazione includerà i metadati mappati.

Quando un utente invia un documento da [!DNL Workfront] a un [!DNL Workfront] , i metadati mappati vengono trasferiti lungo il documento. Mentre la versione del documento in [!DNL Workfront] applicazione collegata a [!DNL Workfront], le modifiche apportate ai metadati del documento in [!DNL Workfront] non vengono riflessi nei metadati del documento in [!DNL Workfront] applicazione. Se un campo mappato in [!DNL Workfront] è stato modificato, è necessario inviare una nuova versione del documento con i metadati aggiornati [!DNL Workfront] applicazione.

>[!NOTE]
>
>È possibile mappare i metadati solo in una direzione: da [!DNL Workfront] a [!DNL Workfront DAM]. Metadati per i documenti collegati a [!DNL Workfront] da [!DNL Workfront DAM] non può essere trasferito a Workfront.

Puoi mappare lo stesso [!DNL Workfront] campi di vari metadati in [!DNL Workfront DAM], ma non è possibile utilizzare un campo di metadati in una di queste applicazioni per più [!DNL Workfront] campi di metadati.

Per configurare più [!DNL Workfront] campi da esportare in un campo di metadati in una [!DNL Workfront] applicazione, crea un campo personalizzato calcolato in [!DNL Workfront] per visualizzare tutti i singoli campi personalizzati di un oggetto. Quindi, mappa il valore calcolato [!DNL Workfront] a un campo di metadati nel [!DNL Workfront] applicazione. Per ulteriori informazioni sui campi personalizzati calcolati, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Prima di poter mappare i campi per il processo di mappatura dei metadati, è necessario abilitare l’applicazione in [!DNL Workfront]. Per ulteriori informazioni, consulta [Configurare le integrazioni dei documenti](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configura [!DNL Workfront] per inviare metadati

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

   ![](assets/metadata-mapping.png)

1. In **[!UICONTROL Seleziona campo di origine per la mappatura]** , inizia a digitare il nome del campo Workfront che desideri mappare [!DNL Workfront DAM], quindi selezionala quando la visualizzi nell&#39;elenco.
1. In **[!UICONTROL Seleziona campo di destinazione per la mappatura]** , selezionare il campo che si desidera compilare con le informazioni nella casella selezionata [!DNL Workfront] campo.

1. Clic **[!UICONTROL Aggiungi mappatura]**.

   Il campo mappato viene visualizzato nei campi mappati elencati nella parte inferiore della pagina.

1. Ripetere i passaggi 5 e 6 fino ad aggiungere tutti i [!DNL Workfront] campi e corrispondenti [!DNL Workfront DAM] campi.

## Elimina campi mappati

1. Accedi a [!DNL Workfront] come amministratore.
1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello sinistro fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Mappatura metadati]**.

1. Nell&#39;elenco dei campi mappati selezionare i campi che si desidera rimuovere dalla mappatura dei metadati.
1. Clic **[!UICONTROL Elimina]**.

   I campi designati non vengono più mappati. Ora, quando un utente invia un documento da [!DNL Workfront] a [!DNL Workfront DAM], i metadati contenuti nei campi eliminati non vengono trasferiti con il documento.

   Un documento inviato prima dell&#39;eliminazione dei campi mappati mantiene i metadati originali inviati con esso, inclusi i metadati per i campi eliminati.
