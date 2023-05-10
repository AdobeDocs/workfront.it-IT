---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurare l’integrazione Experience Manager Assets Essentials
description: Collega il tuo lavoro con i contenuti in Experience Manager Assets Essentials - EDIT ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 9965ec9f436724e438fbbc5977f22761cc673878
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 4%

---

# Configurare l’integrazione Experience Manager Assets Essentials

Collega il tuo lavoro con i contenuti di Experience Manager Assets Essentials &#x200B;:

* &#x200B; push di risorse e metadati da Adobe Workfront a Experience Manager Assets Essentials
* Collegare le risorse da Experience Manager Assets Essentials ai tuoi progetti e attività in Workfront &#x200B;
* Facilitare i flussi di lavoro di controllo delle versioni per le risorse inviate ad Experience Manager Assets Essentials

Puoi anche collegare più archivi Experience Manager Assets a un ambiente Workfront o a più ambienti Workfront a un archivio Experience Manager Assets in tutti gli ID organizzazione. Segui le istruzioni di configurazione riportate in questo articolo per ogni integrazione che desideri configurare.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table>
  <tr>
   <td><strong>piano Adobe Workfront*</strong>
   </td>
   <td>Qualsiasi
   </td>
  </tr>
  <tr>
   <td><strong>Licenze Adobe Workfront*</strong>
   </td>
   <td>Piano
   </td>
  </tr>
  <tr>
   <td><strong>licenza di Experience Manager</strong>
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td><strong>Prodotto</strong>
   </td>
   <td>È necessario disporre di Experience Manager Assets Essentials e devi essere aggiunto al prodotto come utente nell'Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configurazioni a livello di accesso</strong>
   </td>
   <td>Devi essere un amministratore Workfront. Per informazioni sugli amministratori di Workfront, consulta <strong>Concedere a un utente pieno accesso amministrativo</strong>.
   </td>
  </tr>
</table>


*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.


## Configurare l’integrazione

1. Fai clic sul pulsante **Menu principale** nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione**.
1. Seleziona  **Documenti** ![icona documenti](assets/document-icon.png) nel pannello a sinistra, seleziona **Integrazione Experience Manager**.
1. Seleziona **Aggiungi integrazione Experience Manager**.
1. Specifica quanto segue:

   <table>
   <tr>
      <td><strong>Nome</strong>
      </td>
      <td>Immettere il nome che gli utenti dovranno visualizzare nel pulsante Aggiungi nuovo nell'area Documenti.
      </td>
   </tr>
   <tr>
      <td><strong>URL di navigazione</strong>
      </td>
      <td>Il sistema popola automaticamente l'URL di navigazione. Questo URL viene utilizzato per collegarsi all’istanza Assets Essentials della tua organizzazione dal menu principale per un accesso rapido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Archivio Experience Manager Assets</strong>
      </td>
      <td>
      Il sistema popola automaticamente l'archivio Experience Manager associato al tuo ID organizzazione.
      </td>
   </tr>
   </table>

1. Fai clic su **Salva** o passare alla [Impostazione dei metadati (opzionale)](#set-up-metadata-optional) in questo articolo.


## Impostazione dei metadati (opzionale)

Mappa i dati oggetto Workfront ai campi degli elementi multimediali delle risorse in Experience Manager Assets. I metadati vengono mappati quando una risorsa viene trasmessa la prima volta da Workfront.


### Prerequisiti

Prima di iniziare, devi

* Configurare uno schema di metadati in Experience Manager Assets Essentials come spiegato in [Configurare la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Facoltativo) Configura campi modulo personalizzati in Workfront. Workfront dispone di molti campi personalizzati incorporati che è possibile utilizzare. Tuttavia, puoi anche creare campi personalizzati. Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Campi Workfront e Experience Manager Assets supportati**

**Parola chiave AEM**

È possibile mappare qualsiasi campo supportato da Workfront su una parola chiave in Experience Manager Assets Essentials.

Per collegare un campo a una parola chiave, seleziona `dc:subject` nell’elenco a discesa Campo Experience Manager Assets nell’area di mappatura metadati.

Per mappare più campi di testo a riga singola su parole chiave, immetti un elenco separato da virgole dei valori delle parole chiave nel lato Workfront della mappatura metadati e `dc:subject` sul lato Experience Manager Assets. Ogni valore di campo è associato a una parola chiave separata. È possibile utilizzare un campo calcolato per combinare più campi Workfront in un singolo campo di testo separato da virgole.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### Risorse

I metadati vengono mappati quando una risorsa viene inviata da Workfront per la prima volta. I documenti con campi incorporati o personalizzati vengono mappati automaticamente sui campi specificati al primo invio di una risorsa a Experience Manager Assets Essentials.

1. In **Campo Workfront** scegliere un campo Workfront integrato o personalizzato.
   >[!NOTE]
   >
   >È possibile mappare un singolo campo Workfront su più campi Experience Manager Assets. Non è possibile mappare più campi Workfront su un singolo campo Experience Manager Assets.
1. In **Experience Manager** scegliere un campo Experience Manager Assets.

   Per mappare un campo Workfront a un tag Experience Manager Assets, seleziona `dc:subject`.
1. Ripetere i passaggi 1 e 2 come necessario.
   ![abilitare i metadati](assets/metadata-assets-essentials.png)
1. Fai clic su **Salva** o passare alla [Imposta cartelle collegate (facoltativo)](#set-up-linked-folders-optional) in questo articolo.


## Imposta cartelle collegate (facoltativo)

{{setup-linked-folder}}
