---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurare l’integrazione di Experience Manager Assets Essentials
description: Collega il tuo lavoro con i contenuti in Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Configurare l’integrazione di Experience Manager Assets Essentials

Collega il tuo lavoro con i contenuti in Experience Manager Assets Essentials&#x200B;:

* Invio di risorse e metadati da Adobe Workfront a Experience Manager Assets Essentials&#x200B;
* Collega le risorse da Experience Manager Assets Essentials ai tuoi progetti e attività in Workfront&#x200B;
* Semplificare i flussi di lavoro di controllo delle versioni per le risorse inviate a Experience Manager Assets Essentials

>[!NOTE]
>
>È inoltre possibile connettere più archivi Experience Manager Assets a un ambiente Workfront o più ambienti Workfront a un archivio Experience Manager Assets per più ID organizzazione. Segui le istruzioni di configurazione in questo articolo per ogni integrazione da configurare.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] piano
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licenza
   </td>
   <td><p>Corrente: [!UICONTROL Plan]</p>
   <p>Nuovo: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] licenza
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Prodotto
   </td>
   <td>Devi disporre di Experience Manager Assets Essentials e devi essere aggiunto al prodotto come utente nell’Admin Console.
   </td>
  </tr>
  <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare l’integrazione

{{step-1-to-setup}}

1. Seleziona **Documenti** ![icona documenti](assets/document-icon.png) nel pannello a sinistra, quindi seleziona **Integrazione Experience Manager**.
1. Selezionare **Aggiungi integrazione Experience Manager**.
1. Specifica quanto segue:

   <table>
   <tr>
      <td><strong>Nome</strong>
      </td>
      <td>Immettere il nome che si desidera venga visualizzato dagli utenti nel pulsante Aggiungi nuovo nell'area Documenti.
      </td>
   </tr>
   <tr>
      <td><strong>URL di navigazione</strong>
      </td>
      <td>Il sistema compila automaticamente l’URL di navigazione. Questo URL viene utilizzato per creare un collegamento all’istanza degli Assets Essentials della tua organizzazione dal menu principale per un accesso rapido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Archivio Experience Manager Assets</strong>
      </td>
      <td>
      Il sistema compila automaticamente l'archivio Experienci Manager associato all'ID organizzazione.
      </td>
   </tr>
   </table>

1. Fai clic su **Salva** o passa alla sezione [Configura metadati (facoltativo)](#set-up-metadata-optional) in questo articolo.


## Configurazione metadati (facoltativo)

Mappa i dati oggetto Workfront ai campi degli elementi multimediali delle risorse in Experience Manager Assets. I metadati vengono mappati quando una risorsa viene inviata da Workfront per la prima volta.


### Prerequisiti

Prima di iniziare, è necessario

* Configura uno schema metadati in Experience Manager Assets Essentials come descritto in [Configura la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Facoltativo) Configura i campi modulo personalizzati in Workfront. Workfront dispone di molti campi personalizzati incorporati che è possibile utilizzare. Tuttavia, puoi anche creare campi personalizzati. Per ulteriori informazioni, vedere [Progettare un modulo con Progettazione moduli](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campi Workfront e Experience Manager Assets supportati

### Parola chiave AEM

È possibile mappare qualsiasi campo supportato da Workfront a una parola chiave in Experience Manager Assets Essentials.

Per collegare un campo a una parola chiave, selezionare `xcm:keywords` nel menu a discesa del campo Experience Manager Assets nell&#39;area di mappatura dei metadati.

Per mappare più campi di testo a riga singola alle parole chiave, immettere un elenco separato da virgole dei valori delle parole chiave nel lato Workfront della mappatura metadati e `xcm:keywords` nel lato Experience Manager Assets. Ogni valore di campo viene mappato su una parola chiave separata. È possibile utilizzare un campo calcolato per combinare più campi Workfront in un unico campo di testo separato da virgole.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Risorse

I metadati vengono mappati quando una risorsa viene inviata da Workfront per la prima volta. La prima volta che una risorsa viene inviata a Experience Manager Assets Essentials, i documenti con i campi incorporati o personalizzati vengono mappati automaticamente sui campi specificati.

1. Nella colonna **Campo Workfront** scegliere un campo Workfront predefinito o personalizzato.

   >[!NOTE]
   >
   >È possibile mappare un singolo campo Workfront a più campi Experience Manager Assets. Non puoi mappare più campi Workfront a un singolo campo Experience Manager Assets.

1. Nel campo **Experience Manager**, scegli un campo Experience Manager Assets.

   Per associare un campo Workfront a un tag Experience Manager Assets, selezionare `xcm:keywords`.

1. Ripetere i passaggi 1 e 2 in base alle esigenze.
   ![abilita metadati](assets/metadata-assets-essentials.png)
1. Fai clic su **Salva** o passa alla sezione [Configura cartelle collegate (facoltativo)](#set-up-linked-folders-optional) in questo articolo.


## Configurare le cartelle collegate (facoltativo)

{{setup-linked-folder}}
